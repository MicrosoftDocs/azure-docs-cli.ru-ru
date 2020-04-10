---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/01/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cca6f42f29467126553c6e8a332907b1ad1ebc74
ms.sourcegitcommit: 712c8ca6457552b6b7a8866c1370a6ec51d07f2c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "80525259"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="5debd-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5debd-103">Azure CLI release notes</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="5debd-104">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-104">April 01, 2020</span></span>

<span data-ttu-id="5debd-105">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="5debd-105">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-106">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-106">ACR</span></span>

* <span data-ttu-id="5debd-107">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-107">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-108">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-108">Profile</span></span>

* <span data-ttu-id="5debd-109">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="5debd-109">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="5debd-110">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-110">March 31, 2020</span></span>

<span data-ttu-id="5debd-111">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="5debd-111">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-112">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-112">ACR</span></span>

* <span data-ttu-id="5debd-113">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="5debd-113">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="5debd-114">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="5debd-114">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="5debd-115">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="5debd-115">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="5debd-116">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="5debd-116">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="5debd-117">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="5debd-117">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="5debd-118">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="5debd-118">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="5debd-119">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="5debd-119">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-120">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-120">AKS</span></span>

* <span data-ttu-id="5debd-121">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="5debd-121">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="5debd-122">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="5debd-122">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="5debd-123">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="5debd-123">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-124">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-124">AMS</span></span>

* <span data-ttu-id="5debd-125">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="5debd-125">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-126">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-126">AppConfig</span></span>

* <span data-ttu-id="5debd-127">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="5debd-127">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-128">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-128">AppService</span></span>

* <span data-ttu-id="5debd-129">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="5debd-129">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="5debd-130">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="5debd-130">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="5debd-131">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-131">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-132">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-132">ARM</span></span>

* <span data-ttu-id="5debd-133">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="5debd-133">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="5debd-134">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-134">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="5debd-135">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="5debd-135">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="5debd-136">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="5debd-136">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-137">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-137">Backup</span></span>

* <span data-ttu-id="5debd-138">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-138">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="5debd-139">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="5debd-139">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="5debd-140">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="5debd-140">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-141">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-141">Compute</span></span>

* <span data-ttu-id="5debd-142">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="5debd-142">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="5debd-143">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-143">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="5debd-144">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="5debd-144">az vm update: Support --workspace</span></span>
* <span data-ttu-id="5debd-145">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="5debd-145">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="5debd-146">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="5debd-146">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="5debd-147">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-147">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="5debd-148">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-148">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="5debd-149">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="5debd-149">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-150">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-150">Cosmos DB</span></span>

* <span data-ttu-id="5debd-151">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="5debd-151">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="5debd-152">Docker</span><span class="sxs-lookup"><span data-stu-id="5debd-152">Docker</span></span>

* <span data-ttu-id="5debd-153">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="5debd-153">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-154">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-154">Extension</span></span>

* <span data-ttu-id="5debd-155">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="5debd-155">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-156">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-156">HDInsight</span></span>

* <span data-ttu-id="5debd-157">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-157">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="5debd-158">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="5debd-158">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-159">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-159">IoT</span></span>

* <span data-ttu-id="5debd-160">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="5debd-160">Add codeowner</span></span>
* <span data-ttu-id="5debd-161">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="5debd-161">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="5debd-162">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="5debd-162">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5debd-163">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-163">IoTCentral</span></span>

* <span data-ttu-id="5debd-164">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-164">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-165">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-165">KeyVault</span></span>

* <span data-ttu-id="5debd-166">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-166">Support certificate backup/restore</span></span>
* <span data-ttu-id="5debd-167">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="5debd-167">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="5debd-168">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="5debd-168">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="5debd-169">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-169">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="5debd-170">Блокировка</span><span class="sxs-lookup"><span data-stu-id="5debd-170">Lock</span></span>

* <span data-ttu-id="5debd-171">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-171">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-172">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-172">Monitor</span></span>

* <span data-ttu-id="5debd-173">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="5debd-173">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="5debd-174">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5debd-174">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5debd-175">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5debd-175">NetAppFiles</span></span>

* <span data-ttu-id="5debd-176">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="5debd-176">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="5debd-177">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-177">Network</span></span>

* <span data-ttu-id="5debd-178">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="5debd-178">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="5debd-179">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5debd-179">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="5debd-180">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-180">support host names in application gateway listener</span></span>
* <span data-ttu-id="5debd-181">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="5debd-181">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="5debd-182">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="5debd-182">Support vpn gateway generation</span></span>
* <span data-ttu-id="5debd-183">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="5debd-183">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="5debd-184">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5debd-184">Packaging</span></span>

* <span data-ttu-id="5debd-185">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="5debd-185">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-186">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-186">Profile</span></span>

* <span data-ttu-id="5debd-187">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="5debd-187">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-188">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-188">RDBMS</span></span>

* <span data-ttu-id="5debd-189">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-189">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="5debd-190">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-190">March 10, 2020</span></span>

<span data-ttu-id="5debd-191">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="5debd-191">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-192">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-192">ACR</span></span>

* <span data-ttu-id="5debd-193">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="5debd-193">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="5debd-194">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="5debd-194">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="5debd-195">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="5debd-195">Add private link and CMK support</span></span>
* <span data-ttu-id="5debd-196">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="5debd-196">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-197">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-197">AKS</span></span>

* <span data-ttu-id="5debd-198">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5debd-198">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="5debd-199">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="5debd-199">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="5debd-200">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-200">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5debd-201">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="5debd-201">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="5debd-202">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="5debd-202">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="5debd-203">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-203">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5debd-204">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-204">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="5debd-205">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="5debd-205">add missing / in the dashboard url</span></span>
* <span data-ttu-id="5debd-206">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="5debd-206">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="5debd-207">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="5debd-207">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="5debd-208">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="5debd-208">az aks: Add aad session key support</span></span>
* <span data-ttu-id="5debd-209">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="5debd-209">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="5debd-210">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="5debd-210">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-211">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-211">AppConfig</span></span>

* <span data-ttu-id="5debd-212">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-212">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-213">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-213">AppService</span></span>

* <span data-ttu-id="5debd-214">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="5debd-214">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="5debd-215">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-215">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="5debd-216">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="5debd-216">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="5debd-217">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-217">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="5debd-218">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="5debd-218">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="5debd-219">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="5debd-219">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-220">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-220">ARM</span></span>

* <span data-ttu-id="5debd-221">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-221">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="5debd-222">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="5debd-222">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="5debd-223">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-223">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="5debd-224">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5debd-224">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="5debd-225">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-225">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="5debd-226">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5debd-226">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="5debd-227">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="5debd-227">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="5debd-228">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="5debd-228">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="5debd-229">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="5debd-229">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="5debd-230">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="5debd-230">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-231">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-231">CDN</span></span>

* <span data-ttu-id="5debd-232">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="5debd-232">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-233">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-233">Compute</span></span>

* <span data-ttu-id="5debd-234">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="5debd-234">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="5debd-235">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="5debd-235">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="5debd-236">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="5debd-236">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="5debd-237">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="5debd-237">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="5debd-238">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="5debd-238">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-239">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-239">Cosmos DB</span></span>

* <span data-ttu-id="5debd-240">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-240">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="5debd-241">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-241">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-242">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-242">KeyVault</span></span>

* <span data-ttu-id="5debd-243">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-243">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-244">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-244">Monitor</span></span>

* <span data-ttu-id="5debd-245">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-245">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-246">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-246">Network</span></span>

* <span data-ttu-id="5debd-247">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-247">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="5debd-248">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-248">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="5debd-249">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5debd-249">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="5debd-250">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="5debd-250">az network bastion: support bastion</span></span>
* <span data-ttu-id="5debd-251">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-251">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="5debd-252">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="5debd-252">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="5debd-253">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="5debd-253">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="5debd-254">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="5debd-254">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="5debd-255">Политика</span><span class="sxs-lookup"><span data-stu-id="5debd-255">Policy</span></span>

* <span data-ttu-id="5debd-256">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="5debd-256">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-257">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-257">RBAC</span></span>

* <span data-ttu-id="5debd-258">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="5debd-258">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-259">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-259">RDBMS</span></span>

* <span data-ttu-id="5debd-260">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-260">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="5debd-261">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="5debd-261">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="5debd-262">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="5debd-262">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="5debd-263">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-263">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="5debd-264">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-264">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="5debd-265">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-265">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="5debd-266">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-266">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="5debd-267">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="5debd-267">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-268">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-268">SQL</span></span>

* <span data-ttu-id="5debd-269">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="5debd-269">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="5debd-270">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="5debd-270">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="5debd-271">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="5debd-271">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="5debd-272">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="5debd-272">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-273">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-273">Storage</span></span>

* <span data-ttu-id="5debd-274">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="5debd-274">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="5debd-275">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="5debd-275">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="5debd-276">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="5debd-276">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="5debd-277">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-277">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="5debd-278">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="5debd-278">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="5debd-279">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-279">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="5debd-280">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="5debd-280">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="5debd-281">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="5debd-281">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="5debd-282">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-282">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="5debd-283">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-283">February 18, 2020</span></span>

<span data-ttu-id="5debd-284">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="5debd-284">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-285">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-285">ACR</span></span>

* <span data-ttu-id="5debd-286">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-286">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="5debd-287">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="5debd-287">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="5debd-288">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="5debd-288">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-289">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-289">ACS</span></span>

* <span data-ttu-id="5debd-290">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-290">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="5debd-291">Aladdin</span><span class="sxs-lookup"><span data-stu-id="5debd-291">Aladdin</span></span>

* <span data-ttu-id="5debd-292">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-292">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-293">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-293">AMS</span></span>

* <span data-ttu-id="5debd-294">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5debd-294">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-295">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-295">AppConfig</span></span>

* <span data-ttu-id="5debd-296">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="5debd-296">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="5debd-297">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-297">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="5debd-298">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="5debd-298">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-299">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-299">AppService</span></span>

* <span data-ttu-id="5debd-300">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="5debd-300">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="5debd-301">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="5debd-301">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="5debd-302">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="5debd-302">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-303">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-303">ARM</span></span>

* <span data-ttu-id="5debd-304">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="5debd-304">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="5debd-305">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="5debd-305">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-306">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-306">Backup</span></span>

* <span data-ttu-id="5debd-307">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="5debd-307">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="5debd-308">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="5debd-308">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-309">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-309">Compute</span></span>

* <span data-ttu-id="5debd-310">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="5debd-310">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="5debd-311">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="5debd-311">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="5debd-312">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="5debd-312">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="5debd-313">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-313">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="5debd-314">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-314">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="5debd-315">Eventhub</span><span class="sxs-lookup"><span data-stu-id="5debd-315">Eventhub</span></span>

* <span data-ttu-id="5debd-316">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="5debd-316">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-317">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-317">KeyVault</span></span>

* <span data-ttu-id="5debd-318">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="5debd-318">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="5debd-319">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-319">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="5debd-320">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="5debd-320">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="5debd-321">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-321">Network</span></span>

* <span data-ttu-id="5debd-322">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-322">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="5debd-323">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="5debd-323">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="5debd-324">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="5debd-324">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="5debd-325">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5debd-325">Packaging</span></span>

* <span data-ttu-id="5debd-326">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="5debd-326">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-327">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-327">Profile</span></span>

* <span data-ttu-id="5debd-328">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="5debd-328">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="5debd-329">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-329">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="5debd-330">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="5debd-330">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="5debd-331">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="5debd-331">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="5debd-332">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-332">Role</span></span>

* <span data-ttu-id="5debd-333">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="5debd-333">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-334">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-334">SQL</span></span>

* <span data-ttu-id="5debd-335">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="5debd-335">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-336">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-336">Storage</span></span>

* <span data-ttu-id="5debd-337">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="5debd-337">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="5debd-338">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-338">February 04, 2020</span></span>

<span data-ttu-id="5debd-339">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="5debd-339">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-340">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-340">ACS</span></span>

* <span data-ttu-id="5debd-341">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="5debd-341">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="5debd-342">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-342">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-343">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-343">ACR</span></span>

* <span data-ttu-id="5debd-344">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="5debd-344">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="5debd-345">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="5debd-345">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="5debd-346">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="5debd-346">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-347">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-347">AKS</span></span>

* <span data-ttu-id="5debd-348">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="5debd-348">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-349">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-349">AppConfig</span></span>

* <span data-ttu-id="5debd-350">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="5debd-350">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="5debd-351">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="5debd-351">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="5debd-352">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="5debd-352">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="5debd-353">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="5debd-353">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="5debd-354">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5debd-354">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-355">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-355">AppService</span></span>

* <span data-ttu-id="5debd-356">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="5debd-356">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="5debd-357">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-357">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-358">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-358">ARM</span></span>

* <span data-ttu-id="5debd-359">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-359">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="5debd-360">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="5debd-360">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="5debd-361">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="5debd-361">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="5debd-362">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-362">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="5debd-363">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-363">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5debd-364">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5debd-364">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5debd-365">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="5debd-365">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-366">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-366">BotService</span></span>

* <span data-ttu-id="5debd-367">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="5debd-367">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="5debd-368">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-368">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-369">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-369">CDN</span></span>

* <span data-ttu-id="5debd-370">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="5debd-370">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="5debd-371">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="5debd-371">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="5debd-372">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="5debd-372">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5debd-373">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="5debd-373">Deployment Manager</span></span>

* <span data-ttu-id="5debd-374">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-374">Add list operation for all resources.</span></span>
* <span data-ttu-id="5debd-375">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="5debd-375">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="5debd-376">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-376">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-377">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-377">IoT</span></span>

* <span data-ttu-id="5debd-378">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="5debd-378">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="5debd-379">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-379">IoT Central</span></span>

* <span data-ttu-id="5debd-380">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="5debd-380">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-381">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-381">Key Vault</span></span>

* <span data-ttu-id="5debd-382">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-382">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="5debd-383">Разное</span><span class="sxs-lookup"><span data-stu-id="5debd-383">Misc</span></span>

* <span data-ttu-id="5debd-384">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="5debd-384">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="5debd-385">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-385">Network</span></span>

* <span data-ttu-id="5debd-386">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="5debd-386">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="5debd-387">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="5debd-387">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="5debd-388">Политика</span><span class="sxs-lookup"><span data-stu-id="5debd-388">Policy</span></span>

* <span data-ttu-id="5debd-389">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="5debd-389">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="5debd-390">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="5debd-390">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-391">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-391">Profile</span></span>

* <span data-ttu-id="5debd-392">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="5debd-392">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-393">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-393">RBAC</span></span>

* <span data-ttu-id="5debd-394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="5debd-394">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="5debd-395">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5debd-395">Security</span></span>

* <span data-ttu-id="5debd-396">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-396">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-397">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-397">SQL</span></span>

* <span data-ttu-id="5debd-398">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="5debd-398">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="5debd-399">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-399">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="5debd-400">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="5debd-400">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="5debd-401">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="5debd-401">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="5debd-402">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-402">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="5debd-403">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="5debd-403">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-404">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-404">Storage</span></span>

* <span data-ttu-id="5debd-405">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-405">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="5debd-406">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-406">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="5debd-407">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="5debd-407">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="5debd-408">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5debd-408">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5debd-409">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5debd-409">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5debd-410">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5debd-410">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5debd-411">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-411">ServiceFabric</span></span>

* <span data-ttu-id="5debd-412">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="5debd-412">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="5debd-413">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-413">January 13, 2020</span></span>

<span data-ttu-id="5debd-414">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="5debd-414">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-415">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-415">Compute</span></span>

* <span data-ttu-id="5debd-416">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="5debd-416">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="5debd-417">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="5debd-417">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-418">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-418">Storage</span></span>

* <span data-ttu-id="5debd-419">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="5debd-419">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="5debd-420">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="5debd-420">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="5debd-421">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-421">January 07, 2020</span></span>

<span data-ttu-id="5debd-422">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="5debd-422">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-423">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-423">ACR</span></span>

* <span data-ttu-id="5debd-424">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="5debd-424">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="5debd-425">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="5debd-425">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-426">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-426">AppConfig</span></span>

* <span data-ttu-id="5debd-427">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-427">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="5debd-428">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-428">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="5debd-429">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="5debd-429">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-430">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-430">AppService</span></span>

* <span data-ttu-id="5debd-431">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="5debd-431">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="5debd-432">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="5debd-432">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="5debd-433">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="5debd-433">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-434">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-434">ARM</span></span>

* <span data-ttu-id="5debd-435">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="5debd-435">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-436">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-436">Backup</span></span>

* <span data-ttu-id="5debd-437">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="5debd-437">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="5debd-438">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="5debd-438">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="5debd-439">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="5debd-439">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-440">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-440">Compute</span></span>

* <span data-ttu-id="5debd-441">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5debd-441">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="5debd-442">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="5debd-442">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="5debd-443">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="5debd-443">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-444">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-444">HDInsight</span></span>

* <span data-ttu-id="5debd-445">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="5debd-445">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="5debd-446">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="5debd-446">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="5debd-447">Прочее</span><span class="sxs-lookup"><span data-stu-id="5debd-447">Misc.</span></span>

* <span data-ttu-id="5debd-448">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="5debd-448">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="5debd-449">Центры событий</span><span class="sxs-lookup"><span data-stu-id="5debd-449">Event Hubs</span></span>

* <span data-ttu-id="5debd-450">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="5debd-450">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="5debd-451">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-451">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="5debd-452">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-452">Service Bus</span></span>

* <span data-ttu-id="5debd-453">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="5debd-453">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="5debd-454">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="5debd-454">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-455">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-455">RBAC</span></span>

* <span data-ttu-id="5debd-456">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-456">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-457">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-457">Storage</span></span>

* <span data-ttu-id="5debd-458">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="5debd-458">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="5debd-459">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-459">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="5debd-460">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-460">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="5debd-461">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-461">December 17, 2019</span></span>

<span data-ttu-id="5debd-462">2.0.78</span><span class="sxs-lookup"><span data-stu-id="5debd-462">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-463">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-463">ACR</span></span>

* <span data-ttu-id="5debd-464">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-464">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-465">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-465">ACS</span></span>

* <span data-ttu-id="5debd-466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-466">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-467">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-467">AMS</span></span>

* <span data-ttu-id="5debd-468">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="5debd-468">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-469">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-469">AppConfig</span></span>

* <span data-ttu-id="5debd-470">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="5debd-470">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="5debd-471">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="5debd-471">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="5debd-472">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="5debd-472">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-473">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-473">AppService</span></span>

* <span data-ttu-id="5debd-474">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="5debd-474">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="5debd-475">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="5debd-475">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="5debd-476">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="5debd-476">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="5debd-477">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="5debd-477">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-478">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-478">ARM</span></span>

* <span data-ttu-id="5debd-479">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="5debd-479">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="5debd-480">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="5debd-480">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="5debd-481">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="5debd-481">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-482">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-482">Backup</span></span>

* <span data-ttu-id="5debd-483">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="5debd-483">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-484">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-484">BotService</span></span>

* <span data-ttu-id="5debd-485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="5debd-485">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="5debd-486">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="5debd-486">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="5debd-487">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="5debd-487">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="5debd-488">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="5debd-488">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="5debd-489">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="5debd-489">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="5debd-490">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="5debd-490">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="5debd-491">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="5debd-491">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="5debd-492">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="5debd-492">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="5debd-493">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="5debd-493">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-494">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-494">Compute</span></span>

* <span data-ttu-id="5debd-495">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-495">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="5debd-496">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="5debd-496">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="5debd-497">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="5debd-497">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="5debd-498">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="5debd-498">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="5debd-499">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="5debd-499">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="5debd-500">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="5debd-500">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="5debd-501">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-501">Core</span></span>

* <span data-ttu-id="5debd-502">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="5debd-502">Removed support for Python 3.4</span></span>
* <span data-ttu-id="5debd-503">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="5debd-503">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="5debd-504">DLS</span><span class="sxs-lookup"><span data-stu-id="5debd-504">DLS</span></span>

* <span data-ttu-id="5debd-505">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="5debd-505">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="5debd-506">Установка</span><span class="sxs-lookup"><span data-stu-id="5debd-506">Install</span></span>

* <span data-ttu-id="5debd-507">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="5debd-507">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-508">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-508">IOT</span></span>

* <span data-ttu-id="5debd-509">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="5debd-509">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="5debd-510">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="5debd-510">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-511">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-511">Key Vault</span></span>

* <span data-ttu-id="5debd-512">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="5debd-512">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="5debd-513">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="5debd-513">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="5debd-514">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="5debd-514">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="5debd-515">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="5debd-515">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="5debd-516">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="5debd-516">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-517">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-517">Network</span></span>

* <span data-ttu-id="5debd-518">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="5debd-518">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="5debd-519">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-519">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="5debd-520">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="5debd-520">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="5debd-521">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-521">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="5debd-522">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="5debd-522">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="5debd-523">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5debd-523">Packaging</span></span>

* <span data-ttu-id="5debd-524">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="5debd-524">Added back edge builds for pip install</span></span>
* <span data-ttu-id="5debd-525">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="5debd-525">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="5debd-526">Политика</span><span class="sxs-lookup"><span data-stu-id="5debd-526">Policy</span></span>

* <span data-ttu-id="5debd-527">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-527">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="5debd-528">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="5debd-528">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="5debd-529">Redis</span><span class="sxs-lookup"><span data-stu-id="5debd-529">Redis</span></span>

* <span data-ttu-id="5debd-530">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="5debd-530">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="5debd-531">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="5debd-531">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5debd-532">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-532">ServiceFabric</span></span>

* <span data-ttu-id="5debd-533">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="5debd-533">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="5debd-534">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="5debd-534">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-535">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-535">SQL</span></span>

* <span data-ttu-id="5debd-536">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="5debd-536">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-537">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-537">Storage</span></span>

* <span data-ttu-id="5debd-538">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-538">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="5debd-539">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="5debd-539">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="5debd-540">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-540">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="5debd-541">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="5debd-541">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="5debd-542">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="5debd-542">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="5debd-543">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-543">November 26, 2019</span></span>

<span data-ttu-id="5debd-544">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="5debd-544">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-545">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-545">ACR</span></span>

* <span data-ttu-id="5debd-546">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5debd-546">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5debd-547">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5debd-547">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5debd-548">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="5debd-548">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="5debd-549">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="5debd-549">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-550">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-550">AKS</span></span>

* <span data-ttu-id="5debd-551">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="5debd-551">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-552">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-552">AppConfig</span></span>

* <span data-ttu-id="5debd-553">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="5debd-553">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="5debd-554">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="5debd-554">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="5debd-555">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-555">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="5debd-556">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-556">AppService</span></span>

* <span data-ttu-id="5debd-557">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-557">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="5debd-558">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="5debd-558">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="5debd-559">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="5debd-559">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-560">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-560">Backup</span></span>

* <span data-ttu-id="5debd-561">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="5debd-561">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="5debd-562">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="5debd-562">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-563">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-563">Compute</span></span>

* <span data-ttu-id="5debd-564">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-564">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="5debd-565">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="5debd-565">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="5debd-566">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="5debd-566">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="5debd-567">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="5debd-567">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="5debd-568">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="5debd-568">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="5debd-569">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-569">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="5debd-570">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-570">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="5debd-571">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="5debd-571">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="5debd-572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5debd-572">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="5debd-573">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-573">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-574">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-574">IOT</span></span>

* <span data-ttu-id="5debd-575">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="5debd-575">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="5debd-576">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-576">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="5debd-577">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-577">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-578">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-578">Key Vault</span></span>

* <span data-ttu-id="5debd-579">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="5debd-579">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5debd-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5debd-580">NetAppFiles</span></span>

* <span data-ttu-id="5debd-581">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="5debd-581">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="5debd-582">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-582">Network</span></span>

* <span data-ttu-id="5debd-583">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="5debd-583">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="5debd-584">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="5debd-584">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="5debd-585">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="5debd-585">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="5debd-586">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="5debd-586">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="5debd-587">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="5debd-587">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="5debd-588">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="5debd-588">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="5debd-589">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5debd-589">Packaging</span></span>

* <span data-ttu-id="5debd-590">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="5debd-590">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="5debd-591">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="5debd-591">Added support for Python 3.8</span></span>
* <span data-ttu-id="5debd-592">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="5debd-592">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-593">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-593">Profile</span></span>

* <span data-ttu-id="5debd-594">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5debd-594">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="5debd-595">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="5debd-595">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="5debd-596">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="5debd-596">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="5debd-597">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-597">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="5debd-598">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="5debd-598">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-599">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-599">RBAC</span></span>

* <span data-ttu-id="5debd-600">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="5debd-600">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="5debd-601">Redis</span><span class="sxs-lookup"><span data-stu-id="5debd-601">Redis</span></span>

* <span data-ttu-id="5debd-602">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="5debd-602">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="5debd-603">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5debd-603">Reservations</span></span>

* <span data-ttu-id="5debd-604">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="5debd-604">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="5debd-605">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="5debd-605">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="5debd-606">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="5debd-606">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="5debd-607">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="5debd-607">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="5debd-608">Rest</span><span class="sxs-lookup"><span data-stu-id="5debd-608">Rest</span></span>
* <span data-ttu-id="5debd-609">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="5debd-609">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-610">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-610">SQL</span></span>

* <span data-ttu-id="5debd-611">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-611">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-612">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-612">Storage</span></span>

* <span data-ttu-id="5debd-613">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-613">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="5debd-614">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5debd-614">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="5debd-615">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="5debd-615">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="5debd-616">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="5debd-616">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="5debd-617">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-617">November 4, 2019</span></span>

<span data-ttu-id="5debd-618">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="5debd-618">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-619">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-619">ACR</span></span>

* <span data-ttu-id="5debd-620">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="5debd-620">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="5debd-621">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="5debd-621">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="5debd-622">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="5debd-622">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-623">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-623">AKS</span></span>

* <span data-ttu-id="5debd-624">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-624">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="5debd-625">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="5debd-625">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5debd-626">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5debd-626">AppConfig</span></span>

* <span data-ttu-id="5debd-627">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-627">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="5debd-628">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="5debd-628">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="5debd-629">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="5debd-629">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-630">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-630">AppService</span></span>

* <span data-ttu-id="5debd-631">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="5debd-631">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="5debd-632">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-632">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="5debd-633">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5debd-633">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="5debd-634">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="5debd-634">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="5debd-635">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-635">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-636">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-636">ARM</span></span>

* <span data-ttu-id="5debd-637">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="5debd-637">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="5debd-638">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-638">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-639">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-639">Backup</span></span>

* <span data-ttu-id="5debd-640">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="5debd-640">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-641">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-641">Compute</span></span>

* <span data-ttu-id="5debd-642">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="5debd-642">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="5debd-643">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="5debd-643">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="5debd-644">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="5debd-644">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="5debd-645">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="5debd-645">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="5debd-646">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="5debd-646">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="5debd-647">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-647">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="5debd-648">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5debd-648">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="5debd-649">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="5debd-649">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-650">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-650">CosmosDB</span></span>

* <span data-ttu-id="5debd-651">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5debd-651">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5debd-652">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5debd-652">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5debd-653">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-653">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5debd-654">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-654">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5debd-655">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-655">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5debd-656">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-656">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5debd-657">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5debd-657">Fixed typo in help message</span></span>
* <span data-ttu-id="5debd-658">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5debd-658">database: Added deprecation information</span></span>
* <span data-ttu-id="5debd-659">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5debd-659">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-660">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-660">IoT</span></span>

* <span data-ttu-id="5debd-661">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="5debd-661">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="5debd-662">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-662">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-663">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-663">Key Vault</span></span>

* <span data-ttu-id="5debd-664">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="5debd-664">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="5debd-665">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="5debd-665">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5debd-666">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5debd-666">NetAppFiles</span></span>

* <span data-ttu-id="5debd-667">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-667">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="5debd-668">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="5debd-668">This new API version includes:</span></span>

    - <span data-ttu-id="5debd-669">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="5debd-669">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="5debd-670">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="5debd-670">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="5debd-671">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="5debd-671">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="5debd-672">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="5debd-672">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="5debd-673">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-673">Network</span></span>

* <span data-ttu-id="5debd-674">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="5debd-674">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="5debd-675">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="5debd-675">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="5debd-676">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="5debd-676">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="5debd-677">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-677">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="5debd-678">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="5debd-678">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="5debd-679">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="5debd-679">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-680">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-680">Profile</span></span>

* <span data-ttu-id="5debd-681">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="5debd-681">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="5debd-682">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-682">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-683">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-683">RBAC</span></span>

* <span data-ttu-id="5debd-684">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="5debd-684">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5debd-685">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-685">ServiceFabric</span></span>

* <span data-ttu-id="5debd-686">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-686">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-687">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-687">SQL</span></span>

* <span data-ttu-id="5debd-688">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="5debd-688">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-689">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-689">Storage</span></span>

* <span data-ttu-id="5debd-690">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-690">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="5debd-691">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-691">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="5debd-692">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-692">October 15, 2019</span></span>

<span data-ttu-id="5debd-693">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="5debd-693">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-694">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-694">AKS</span></span>

* <span data-ttu-id="5debd-695">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-695">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="5debd-696">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-696">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-697">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-697">AMS</span></span>

* <span data-ttu-id="5debd-698">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-698">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="5debd-699">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="5debd-699">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-700">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-700">AppService</span></span>

* <span data-ttu-id="5debd-701">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="5debd-701">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="5debd-702">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5debd-702">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="5debd-703">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="5debd-703">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-704">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-704">ARM</span></span>

* <span data-ttu-id="5debd-705">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-705">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-706">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-706">Compute</span></span>

* <span data-ttu-id="5debd-707">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-707">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="5debd-708">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="5debd-708">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="5debd-709">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="5debd-709">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="5debd-710">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-710">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="5debd-711">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-711">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="5debd-712">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-712">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="5debd-713">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-713">Core</span></span>

* <span data-ttu-id="5debd-714">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="5debd-714">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-715">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-715">IoT</span></span>

* <span data-ttu-id="5debd-716">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="5debd-716">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-717">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-717">Monitor</span></span>

* <span data-ttu-id="5debd-718">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="5debd-718">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-719">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-719">Network</span></span>

* <span data-ttu-id="5debd-720">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="5debd-720">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="5debd-721">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-721">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-722">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-722">SQL</span></span>

* <span data-ttu-id="5debd-723">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5debd-723">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-724">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-724">Storage</span></span>

* <span data-ttu-id="5debd-725">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="5debd-725">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="5debd-726">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-726">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="5debd-727">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-727">September 24, 2019</span></span>

<span data-ttu-id="5debd-728">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="5debd-728">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-729">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-729">ACR</span></span>

* <span data-ttu-id="5debd-730">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="5debd-730">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="5debd-731">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-731">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-732">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-732">AKS</span></span>

* <span data-ttu-id="5debd-733">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="5debd-733">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="5debd-734">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="5debd-734">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="5debd-735">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-735">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-736">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-736">ARM</span></span>

* <span data-ttu-id="5debd-737">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-737">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-738">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-738">Compute</span></span>

* <span data-ttu-id="5debd-739">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-739">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5debd-740">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-740">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5debd-741">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="5debd-741">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="5debd-742">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="5debd-742">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="5debd-743">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5debd-743">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-744">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-744">Cosmos DB</span></span>

* <span data-ttu-id="5debd-745">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="5debd-745">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="5debd-746">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="5debd-746">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="5debd-747">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5debd-747">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5debd-748">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5debd-748">EventGrid</span></span>

* <span data-ttu-id="5debd-749">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="5debd-749">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-750">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-750">Key Vault</span></span>

* <span data-ttu-id="5debd-751">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-751">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-752">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-752">Monitor</span></span>

* <span data-ttu-id="5debd-753">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-753">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="5debd-754">Политика</span><span class="sxs-lookup"><span data-stu-id="5debd-754">Policy</span></span>

* <span data-ttu-id="5debd-755">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-755">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="5debd-756">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="5debd-756">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-757">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-757">Storage</span></span>

* <span data-ttu-id="5debd-758">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="5debd-758">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="5debd-759">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-759">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-760">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-760">ACR</span></span>

* <span data-ttu-id="5debd-761">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-761">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-762">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-762">AKS</span></span>

* <span data-ttu-id="5debd-763">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5debd-763">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="5debd-764">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-764">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="5debd-765">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-765">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-766">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-766">ARM</span></span>

* <span data-ttu-id="5debd-767">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="5debd-767">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-768">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-768">Batch</span></span>

* <span data-ttu-id="5debd-769">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="5debd-769">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="5debd-770">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="5debd-770">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="5debd-771">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="5debd-771">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="5debd-772">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="5debd-772">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="5debd-773">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="5debd-773">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="5debd-774">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="5debd-774">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="5debd-775">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="5debd-775">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-776">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-776">HDInsight</span></span>

* <span data-ttu-id="5debd-777">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5debd-777">GA release</span></span>
* <span data-ttu-id="5debd-778">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5debd-778">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-779">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-779">Key Vault</span></span>

* <span data-ttu-id="5debd-780">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="5debd-780">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="5debd-781">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="5debd-781">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="5debd-782">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-782">Network</span></span>

* <span data-ttu-id="5debd-783">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="5debd-783">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="5debd-784">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="5debd-784">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="5debd-785">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="5debd-785">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="5debd-786">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-786">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="5debd-787">Политика</span><span class="sxs-lookup"><span data-stu-id="5debd-787">Policy</span></span>

* <span data-ttu-id="5debd-788">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-788">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="5debd-789">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-789">August 27, 2019</span></span>

<span data-ttu-id="5debd-790">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="5debd-790">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-791">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-791">ACR</span></span>

* <span data-ttu-id="5debd-792">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="5debd-792">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="5debd-793">Управление API</span><span class="sxs-lookup"><span data-stu-id="5debd-793">API Management</span></span>

* <span data-ttu-id="5debd-794">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="5debd-794">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-795">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-795">AppService</span></span>

* <span data-ttu-id="5debd-796">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="5debd-796">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="5debd-797">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="5debd-797">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-798">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-798">Keyvault</span></span>

* <span data-ttu-id="5debd-799">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="5debd-799">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="5debd-800">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-800">Network</span></span>

* <span data-ttu-id="5debd-801">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-801">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="5debd-802">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="5debd-802">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="5debd-803">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="5debd-803">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="5debd-804">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="5debd-804">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-805">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-805">RBAC</span></span>

* <span data-ttu-id="5debd-806">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="5debd-806">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5debd-807">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-807">ServiceFabric</span></span>

* <span data-ttu-id="5debd-808">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="5debd-808">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="5debd-809">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="5debd-809">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="5debd-810">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="5debd-810">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="5debd-811">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="5debd-811">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="5debd-812">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="5debd-812">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="5debd-813">SignalR</span><span class="sxs-lookup"><span data-stu-id="5debd-813">SignalR</span></span>

* <span data-ttu-id="5debd-814">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="5debd-814">Added new commands:</span></span>
  * <span data-ttu-id="5debd-815">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="5debd-815">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="5debd-816">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="5debd-816">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="5debd-817">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="5debd-817">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="5debd-818">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="5debd-818">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-819">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-819">Storage</span></span>

* <span data-ttu-id="5debd-820">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="5debd-820">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="5debd-821">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-821">August 13, 2019</span></span>

<span data-ttu-id="5debd-822">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="5debd-822">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-823">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-823">AppService</span></span>

* <span data-ttu-id="5debd-824">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="5debd-824">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-825">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-825">BotService</span></span>

* <span data-ttu-id="5debd-826">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="5debd-826">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="5debd-827">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="5debd-827">CognitiveServices</span></span>

* <span data-ttu-id="5debd-828">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-828">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-829">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-829">Cosmos DB</span></span>

* <span data-ttu-id="5debd-830">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="5debd-830">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="5debd-831">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-831">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-832">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-832">HDInsight</span></span>

<span data-ttu-id="5debd-833">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="5debd-833">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="5debd-834">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="5debd-834">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="5debd-835">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="5debd-835">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="5debd-836">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="5debd-836">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="5debd-837">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="5debd-837">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="5debd-838">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-838">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="5debd-839">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="5debd-839">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="5debd-840">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="5debd-840">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="5debd-841">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="5debd-841">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="5debd-842">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="5debd-842">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="5debd-843">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="5debd-843">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="5debd-844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="5debd-844">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="5debd-845">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="5debd-845">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="5debd-846">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="5debd-846">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="5debd-847">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-847">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="5debd-848">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="5debd-848">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="5debd-849">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="5debd-849">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="5debd-850">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="5debd-850">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="5debd-851">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-851">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="5debd-852">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-852">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="5debd-853">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="5debd-853">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="5debd-854">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-854">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="5debd-855">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="5debd-855">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="5debd-856">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="5debd-856">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-857">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-857">Interactive</span></span>

* <span data-ttu-id="5debd-858">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="5debd-858">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="5debd-859">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5debd-859">Kubernetes</span></span>

* <span data-ttu-id="5debd-860">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="5debd-860">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-861">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-861">Network</span></span>

* <span data-ttu-id="5debd-862">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="5debd-862">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-863">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-863">Profile</span></span>

* <span data-ttu-id="5debd-864">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5debd-864">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5debd-865">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-865">ServiceFabric</span></span>

* <span data-ttu-id="5debd-866">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="5debd-866">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="5debd-867">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="5debd-867">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-868">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-868">Storage</span></span>

* <span data-ttu-id="5debd-869">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-869">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="5debd-870">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-870">July 30, 2019</span></span>

<span data-ttu-id="5debd-871">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="5debd-871">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-872">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-872">ACR</span></span>

* <span data-ttu-id="5debd-873">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="5debd-873">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="5debd-874">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-874">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-875">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-875">Appservice</span></span>

* <span data-ttu-id="5debd-876">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="5debd-876">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="5debd-877">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="5debd-877">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="5debd-878">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="5debd-878">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="5debd-879">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-879">Network</span></span>

* <span data-ttu-id="5debd-880">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="5debd-880">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="5debd-881">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="5debd-881">Fixes #9604.</span></span> <span data-ttu-id="5debd-882">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-882">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="5debd-883">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="5debd-883">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-884">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-884">RBAC</span></span>

* <span data-ttu-id="5debd-885">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-885">Added `user update` command</span></span>
* <span data-ttu-id="5debd-886">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="5debd-886">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="5debd-887">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-887">Use replacement argument `--id`</span></span>
* <span data-ttu-id="5debd-888">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-888">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-889">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-889">SQL</span></span>

* <span data-ttu-id="5debd-890">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="5debd-890">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-891">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-891">Storage</span></span>

* <span data-ttu-id="5debd-892">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="5debd-892">Added `storage remove` command</span></span>
* <span data-ttu-id="5debd-893">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-893">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-894">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-894">VM</span></span>

* <span data-ttu-id="5debd-895">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="5debd-895">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="5debd-896">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-896">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="5debd-897">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-897">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="5debd-898">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-898">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="5debd-899">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5debd-899">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="5debd-900">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-900">July 16, 2019</span></span>

<span data-ttu-id="5debd-901">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="5debd-901">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-902">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-902">Appservice</span></span>

* <span data-ttu-id="5debd-903">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="5debd-903">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="5debd-904">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="5debd-904">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="5debd-905">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-905">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="5debd-906">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-906">Core</span></span>

* <span data-ttu-id="5debd-907">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="5debd-907">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-908">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-908">Batch</span></span>

* <span data-ttu-id="5debd-909">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-909">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="5debd-910">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="5debd-910">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="5debd-911">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-911">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="5debd-912">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-912">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5debd-913">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5debd-913">Eventhubs</span></span>

* <span data-ttu-id="5debd-914">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-914">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-915">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-915">RDBMS</span></span>

* <span data-ttu-id="5debd-916">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="5debd-916">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="5debd-917">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-917">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="5debd-918">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="5debd-918">Relay</span></span>

* <span data-ttu-id="5debd-919">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="5debd-919">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="5debd-920">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-920">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5debd-921">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-921">Servicebus</span></span>

* <span data-ttu-id="5debd-922">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-922">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-923">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-923">Storage</span></span>

* <span data-ttu-id="5debd-924">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="5debd-924">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="5debd-925">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="5debd-925">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="5debd-926">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-926">July 2, 2019</span></span>

<span data-ttu-id="5debd-927">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="5debd-927">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="5debd-928">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-928">Core</span></span>

* <span data-ttu-id="5debd-929">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="5debd-929">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="5debd-930">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="5debd-930">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="5debd-931">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="5debd-931">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-932">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-932">ACR</span></span>

* <span data-ttu-id="5debd-933">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="5debd-933">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-934">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-934">Appservice</span></span>

* <span data-ttu-id="5debd-935">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-935">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="5debd-936">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-936">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="5debd-937">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5debd-937">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="5debd-938">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-938">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-939">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-939">Cosmos DB</span></span>

* <span data-ttu-id="5debd-940">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="5debd-940">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="5debd-941">DLS</span><span class="sxs-lookup"><span data-stu-id="5debd-941">DLS</span></span>

* <span data-ttu-id="5debd-942">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="5debd-942">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="5debd-943">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5debd-943">Feedback</span></span>

* <span data-ttu-id="5debd-944">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="5debd-944">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-945">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-945">HDInsight</span></span>

* <span data-ttu-id="5debd-946">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="5debd-946">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="5debd-947">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="5debd-947">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="5debd-948">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="5debd-948">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="5debd-949">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="5debd-949">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="5debd-950">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="5debd-950">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="5debd-951">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-951">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="5debd-952">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-952">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="5debd-953">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="5debd-953">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="5debd-954">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-954">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="5debd-955">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="5debd-955">Managed Services</span></span>

* <span data-ttu-id="5debd-956">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5debd-956">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-957">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-957">Profile</span></span>
* <span data-ttu-id="5debd-958">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="5debd-958">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-959">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-959">RBAC</span></span>

* <span data-ttu-id="5debd-960">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5debd-960">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="5debd-961">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="5debd-961">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="5debd-962">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-962">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="5debd-963">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="5debd-963">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-964">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-964">RDBMS</span></span>

* <span data-ttu-id="5debd-965">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-965">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-966">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-966">SQL</span></span>

* <span data-ttu-id="5debd-967">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-967">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-968">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-968">Storage</span></span>

* <span data-ttu-id="5debd-969">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="5debd-969">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="5debd-970">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="5debd-970">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="5debd-971">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-971">VM</span></span>

* <span data-ttu-id="5debd-972">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-972">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="5debd-973">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="5debd-973">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="5debd-974">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="5debd-974">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="5debd-975">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="5debd-975">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="5debd-976">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-976">June 18, 2019</span></span>

<span data-ttu-id="5debd-977">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="5debd-977">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="5debd-978">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-978">Core</span></span>

<span data-ttu-id="5debd-979">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5debd-979">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="5debd-980">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="5debd-980">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="5debd-981">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="5debd-981">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="5debd-982">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="5debd-982">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="5debd-983">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5debd-983">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="5debd-984">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="5debd-984">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="5debd-985">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="5debd-985">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-986">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-986">ACR</span></span>
* <span data-ttu-id="5debd-987">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="5debd-987">Added 'acr check-health' command</span></span>
* <span data-ttu-id="5debd-988">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-988">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-989">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-989">ACS</span></span>
* <span data-ttu-id="5debd-990">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="5debd-990">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-991">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-991">AMS</span></span>
* <span data-ttu-id="5debd-992">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="5debd-992">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-993">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-993">AppService</span></span>
* <span data-ttu-id="5debd-994">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="5debd-994">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="5debd-995">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5debd-995">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="5debd-996">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="5debd-996">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="5debd-997">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-997">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="5debd-998">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="5debd-998">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="5debd-999">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="5debd-999">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1000">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1000">Batch</span></span>
* <span data-ttu-id="5debd-1001">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="5debd-1001">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-1002">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-1002">BatchAI</span></span>
* <span data-ttu-id="5debd-1003">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="5debd-1003">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1004">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1004">BotService</span></span>
* <span data-ttu-id="5debd-1005">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="5debd-1005">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1006">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1006">CosmosDB</span></span>
* <span data-ttu-id="5debd-1007">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1007">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="5debd-1008">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1008">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="5debd-1009">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="5debd-1009">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="5debd-1010">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="5debd-1010">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5debd-1011">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5debd-1011">EventGrid</span></span>
* <span data-ttu-id="5debd-1012">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="5debd-1012">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="5debd-1013">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="5debd-1013">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="5debd-1014">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="5debd-1014">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="5debd-1015">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1015">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="5debd-1016">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1016">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-1017">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-1017">HDInsight</span></span>
* <span data-ttu-id="5debd-1018">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1018">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1019">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1019">IoT</span></span>
* <span data-ttu-id="5debd-1020">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1020">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="5debd-1021">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="5debd-1021">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1022">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1022">Network</span></span>
* <span data-ttu-id="5debd-1023">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="5debd-1023">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="5debd-1024">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1024">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="5debd-1025">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="5debd-1025">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="5debd-1026">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="5debd-1026">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1027">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1027">Resource</span></span>
* <span data-ttu-id="5debd-1028">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="5debd-1028">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="5debd-1029">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1029">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5debd-1030">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-1030">ServiceBus</span></span>
* <span data-ttu-id="5debd-1031">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1031">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1032">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1032">SQL</span></span>
* <span data-ttu-id="5debd-1033">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1033">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="5debd-1034">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1034">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="5debd-1035">SQLVm</span><span class="sxs-lookup"><span data-stu-id="5debd-1035">SQLVm</span></span>
* <span data-ttu-id="5debd-1036">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1036">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="5debd-1037">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-1037">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1038">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1038">Storage</span></span>
* <span data-ttu-id="5debd-1039">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1039">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="5debd-1040">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1040">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1041">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1041">VM</span></span>
* <span data-ttu-id="5debd-1042">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-1042">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="5debd-1043">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1043">June 4, 2019</span></span>

<span data-ttu-id="5debd-1044">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="5debd-1044">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1045">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1045">Core</span></span>
* <span data-ttu-id="5debd-1046">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="5debd-1046">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1047">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1047">ACR</span></span>
* <span data-ttu-id="5debd-1048">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="5debd-1048">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1049">ACS</span></span>
* <span data-ttu-id="5debd-1050">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1050">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="5debd-1051">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="5debd-1051">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1052">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1052">Batch</span></span>
* <span data-ttu-id="5debd-1053">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="5debd-1053">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1054">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1054">IoT</span></span>
* <span data-ttu-id="5debd-1055">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5debd-1055">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1056">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1056">Network</span></span>
* <span data-ttu-id="5debd-1057">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="5debd-1057">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="5debd-1058">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1058">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="5debd-1059">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1059">Resource</span></span>
* <span data-ttu-id="5debd-1060">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="5debd-1060">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1061">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1061">Role</span></span>
* <span data-ttu-id="5debd-1062">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1062">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-1063">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-1063">Compute</span></span>
* <span data-ttu-id="5debd-1064">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="5debd-1064">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="5debd-1065">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1065">May 21, 2019</span></span>

<span data-ttu-id="5debd-1066">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="5debd-1066">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1067">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1067">Core</span></span>
* <span data-ttu-id="5debd-1068">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1068">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="5debd-1069">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="5debd-1069">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="5debd-1070">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1070">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1071">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1071">ACR</span></span>
* <span data-ttu-id="5debd-1072">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="5debd-1072">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1073">ACS</span></span>
* <span data-ttu-id="5debd-1074">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="5debd-1074">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1075">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1075">AppService</span></span>
* <span data-ttu-id="5debd-1076">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="5debd-1076">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="5debd-1077">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="5debd-1077">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="5debd-1078">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1078">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="5debd-1079">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="5debd-1079">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="5debd-1080">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1080">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="5debd-1081">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1081">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="5debd-1082">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="5debd-1082">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1083">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1083">BotService</span></span>
* <span data-ttu-id="5debd-1084">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-1084">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="5debd-1085">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-1085">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-1086">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-1086">Consumption</span></span>
* <span data-ttu-id="5debd-1087">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1087">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1088">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1088">IoT</span></span>
* <span data-ttu-id="5debd-1089">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1089">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1090">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1090">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="5debd-1092">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="5debd-1092">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="5debd-1093">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1093">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1094">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-1094">RDBMS</span></span>
* <span data-ttu-id="5debd-1095">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1095">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-1096">RBAC</span><span class="sxs-lookup"><span data-stu-id="5debd-1096">RBAC</span></span>
* <span data-ttu-id="5debd-1097">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1097">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1098">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1098">Storage</span></span>
* <span data-ttu-id="5debd-1099">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1099">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="5debd-1100">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5debd-1100">Compute</span></span>
* <span data-ttu-id="5debd-1101">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5debd-1101">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="5debd-1102">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="5debd-1102">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="5debd-1103">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1103">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="5debd-1104">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="5debd-1104">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="5debd-1105">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1105">May 6, 2019</span></span>

<span data-ttu-id="5debd-1106">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="5debd-1106">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1107">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1107">ACS</span></span>
* <span data-ttu-id="5debd-1108">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1108">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="5debd-1109">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="5debd-1109">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="5debd-1110">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1110">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="5debd-1111">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1111">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1112">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1112">Appservice</span></span>
* <span data-ttu-id="5debd-1113">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5debd-1113">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="5debd-1114">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1114">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="5debd-1115">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1115">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="5debd-1116">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1116">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="5debd-1117">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1117">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="5debd-1118">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1118">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="5debd-1119">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1119">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="5debd-1120">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="5debd-1120">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="5debd-1121">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-1121">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="5debd-1122">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1122">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1123">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1123">Batch</span></span>
* <span data-ttu-id="5debd-1124">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1124">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1125">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1125">Botservice</span></span>
* <span data-ttu-id="5debd-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="5debd-1126">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="5debd-1127">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1127">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="5debd-1128">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1128">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="5debd-1129">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1129">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="5debd-1130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1130">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="5debd-1131">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1131">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="5debd-1132">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1132">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="5debd-1133">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1133">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="5debd-1134">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5debd-1134">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="5debd-1135">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5debd-1135">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="5debd-1136">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="5debd-1136">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="5debd-1137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1137">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="5debd-1138">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1138">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="5debd-1139">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="5debd-1139">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="5debd-1140">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1140">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="5debd-1141">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="5debd-1141">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="5debd-1142">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1142">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5debd-1143">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1143">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="5debd-1144">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="5debd-1144">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="5debd-1145">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1145">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5debd-1146">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1146">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="5debd-1147">Configure</span><span class="sxs-lookup"><span data-stu-id="5debd-1147">Configure</span></span>
* <span data-ttu-id="5debd-1148">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1148">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5debd-1149">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5debd-1149">Eventhubs</span></span>
* <span data-ttu-id="5debd-1150">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1150">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5debd-1151">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1151">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1152">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1152">Network</span></span>
* <span data-ttu-id="5debd-1153">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1153">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="5debd-1154">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5debd-1154">Policy Insights</span></span>
* <span data-ttu-id="5debd-1155">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1155">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1156">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1156">Role</span></span>
* <span data-ttu-id="5debd-1157">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="5debd-1157">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="5debd-1158">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-1158">Service Bus</span></span>
* <span data-ttu-id="5debd-1159">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1159">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5debd-1160">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1160">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="5debd-1161">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5debd-1161">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1162">SQL</span></span>
* <span data-ttu-id="5debd-1163">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1163">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1164">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1164">VM</span></span>
* <span data-ttu-id="5debd-1165">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-1165">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="5debd-1166">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-1166">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="5debd-1167">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1167">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="5debd-1168">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="5debd-1168">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="5debd-1169">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="5debd-1169">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="5debd-1170">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1170">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="5debd-1171">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1171">April 23, 2019</span></span>

<span data-ttu-id="5debd-1172">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="5debd-1172">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1173">ACS</span></span>
* <span data-ttu-id="5debd-1174">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1174">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="5debd-1175">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="5debd-1175">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-1176">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-1176">AMS</span></span>
* <span data-ttu-id="5debd-1177">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1177">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1178">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1178">AppService</span></span>
* <span data-ttu-id="5debd-1179">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1179">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="5debd-1180">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-1180">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="5debd-1181">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="5debd-1181">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="5debd-1182">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5debd-1182">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="5debd-1183">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1183">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="5debd-1184">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="5debd-1184">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="5debd-1185">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="5debd-1185">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="5debd-1186">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="5debd-1186">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="5debd-1187">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1187">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5debd-1188">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="5debd-1188">Deployment Manager</span></span>
* <span data-ttu-id="5debd-1189">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="5debd-1189">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="5debd-1190">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5debd-1190">Lab</span></span>
* <span data-ttu-id="5debd-1191">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1191">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1192">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1192">Network</span></span>
* <span data-ttu-id="5debd-1193">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="5debd-1193">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1194">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1194">Resource</span></span>
* <span data-ttu-id="5debd-1195">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1195">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="5debd-1196">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1196">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="5debd-1197">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="5debd-1197">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="5debd-1198">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="5debd-1198">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1199">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1199">SQL</span></span>
* <span data-ttu-id="5debd-1200">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5debd-1200">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="5debd-1201">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1201">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="5debd-1202">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1202">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="5debd-1203">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1203">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1204">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1204">Storage</span></span>
* <span data-ttu-id="5debd-1205">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1205">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1206">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1206">VM</span></span>
* <span data-ttu-id="5debd-1207">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1207">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="5debd-1208">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1208">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="5debd-1209">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="5debd-1209">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="5debd-1210">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1210">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1211">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1211">Core</span></span>
* <span data-ttu-id="5debd-1212">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="5debd-1212">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1213">ACR</span></span>
* <span data-ttu-id="5debd-1214">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="5debd-1214">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-1215">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-1215">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="5debd-1218">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1218">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="5debd-1219">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1219">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1220">AppService</span></span>
* <span data-ttu-id="5debd-1221">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1221">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="5debd-1222">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1222">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="5debd-1223">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1223">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="5debd-1224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-1224">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="5debd-1225">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1225">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="5debd-1226">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1226">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="5debd-1227">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-1227">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-1228">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-1228">CDN</span></span>
* <span data-ttu-id="5debd-1229">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1229">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="5debd-1230">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5debd-1230">Feedback</span></span>
* <span data-ttu-id="5debd-1231">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-1231">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="5debd-1232">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1232">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="5debd-1233">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="5debd-1233">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1234">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1234">Monitor</span></span>
* <span data-ttu-id="5debd-1235">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1235">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="5debd-1236">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1236">Network</span></span>
* <span data-ttu-id="5debd-1237">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1237">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="5debd-1238">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1238">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="5debd-1239">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1239">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="5debd-1240">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1240">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="5debd-1241">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="5debd-1241">PrivateDNS</span></span>
* <span data-ttu-id="5debd-1242">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1242">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1243">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1243">Resource</span></span>
* <span data-ttu-id="5debd-1244">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="5debd-1244">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1245">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1245">Role</span></span>
* <span data-ttu-id="5debd-1246">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="5debd-1246">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="5debd-1247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="5debd-1247">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1248">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1248">SQL</span></span>
* <span data-ttu-id="5debd-1249">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="5debd-1249">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1250">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1250">Storage</span></span>
* <span data-ttu-id="5debd-1251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1251">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="5debd-1252">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1252">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="5debd-1253">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="5debd-1253">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="5debd-1254">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5debd-1254">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="5debd-1255">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1255">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="5debd-1256">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1256">Core</span></span>
* <span data-ttu-id="5debd-1257">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1257">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="5debd-1258">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="5debd-1258">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="5debd-1259">Cloud</span><span class="sxs-lookup"><span data-stu-id="5debd-1259">Cloud</span></span>
* <span data-ttu-id="5debd-1260">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1260">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1261">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1261">ACR</span></span>
* <span data-ttu-id="5debd-1262">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1262">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="5debd-1263">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1263">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="5debd-1264">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="5debd-1264">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="5debd-1265">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1265">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1266">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1266">AppService</span></span>
* <span data-ttu-id="5debd-1267">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="5debd-1267">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="5debd-1268">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1268">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="5debd-1269">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1269">BOT Service</span></span>
* <span data-ttu-id="5debd-1270">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1270">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="5debd-1271">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="5debd-1271">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="5debd-1272">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1272">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="5debd-1273">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5debd-1273">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-1274">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-1274">CDN</span></span>
* <span data-ttu-id="5debd-1275">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1275">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="5debd-1276">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1276">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="5debd-1277">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1277">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5debd-1278">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5debd-1278">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1279">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1279">Cosmosdb</span></span>
* <span data-ttu-id="5debd-1280">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5debd-1280">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="5debd-1281">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5debd-1281">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-1282">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-1282">Interactive</span></span>
* <span data-ttu-id="5debd-1283">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="5debd-1283">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1284">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1284">Monitor</span></span>
* <span data-ttu-id="5debd-1285">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1285">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1286">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1286">Network</span></span>
* <span data-ttu-id="5debd-1287">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1287">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-1288">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-1288">Profile</span></span>
* <span data-ttu-id="5debd-1289">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1289">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="5debd-1290">Postgres</span><span class="sxs-lookup"><span data-stu-id="5debd-1290">Postgres</span></span> 
* <span data-ttu-id="5debd-1291">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1291">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="5debd-1292">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1292">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1293">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1293">Resource</span></span>
* <span data-ttu-id="5debd-1294">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1294">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="5debd-1295">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="5debd-1295">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="5debd-1296">График</span><span class="sxs-lookup"><span data-stu-id="5debd-1296">Graph</span></span>
* <span data-ttu-id="5debd-1297">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1297">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="5debd-1298">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1298">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="5debd-1299">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1299">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="5debd-1300">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="5debd-1300">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="5debd-1301">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="5debd-1301">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1302">носителей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1302">storage</span></span>
* <span data-ttu-id="5debd-1303">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1303">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="5debd-1304">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="5debd-1304">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="5debd-1305">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="5debd-1305">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="5debd-1306">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="5debd-1306">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1307">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1307">VM</span></span>
* <span data-ttu-id="5debd-1308">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1308">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="5debd-1309">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1309">March 12, 2019</span></span>

<span data-ttu-id="5debd-1310">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="5debd-1310">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1311">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1311">Core</span></span>

* <span data-ttu-id="5debd-1312">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="5debd-1312">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1313">ACR</span></span>

* <span data-ttu-id="5debd-1314">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1314">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1315">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1315">ACS</span></span>

* <span data-ttu-id="5debd-1316">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="5debd-1316">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="5debd-1317">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1317">AppService</span></span>

* <span data-ttu-id="5debd-1318">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-1318">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="5debd-1319">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1319">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="5debd-1320">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1320">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="5debd-1321">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="5debd-1321">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1322">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1322">Botservice</span></span>

* <span data-ttu-id="5debd-1323">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5debd-1323">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5debd-1324">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5debd-1324">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5debd-1325">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1325">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="5debd-1326">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="5debd-1326">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1327">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1327">Container</span></span>

* <span data-ttu-id="5debd-1328">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1328">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="5debd-1329">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-1329">EventHub</span></span>

* <span data-ttu-id="5debd-1330">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="5debd-1330">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="5debd-1331">Поиск</span><span class="sxs-lookup"><span data-stu-id="5debd-1331">Find</span></span>

* <span data-ttu-id="5debd-1332">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="5debd-1332">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-1333">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-1333">HDInsight</span></span>

* <span data-ttu-id="5debd-1334">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1334">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1335">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1335">Network</span></span>

* <span data-ttu-id="5debd-1336">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1336">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1337">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5debd-1337">Rdbms</span></span>

* <span data-ttu-id="5debd-1338">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1338">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1339">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1339">Role</span></span>

* <span data-ttu-id="5debd-1340">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1340">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="5debd-1341">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-1341">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5debd-1342">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-1342">Service Fabric</span></span>

* <span data-ttu-id="5debd-1343">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1343">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="5debd-1344">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1344">February 26, 2019</span></span>

<span data-ttu-id="5debd-1345">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="5debd-1345">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1346">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1346">Core</span></span>

* <span data-ttu-id="5debd-1347">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="5debd-1347">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1348">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1348">ACR</span></span>

* <span data-ttu-id="5debd-1349">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1349">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="5debd-1350">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-1350">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1351">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1351">ACS</span></span>

* <span data-ttu-id="5debd-1352">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1352">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1353">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1353">AppService</span></span>

* <span data-ttu-id="5debd-1354">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1354">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1355">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1355">Batch</span></span>
* <span data-ttu-id="5debd-1356">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1356">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="5debd-1357">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1357">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="5debd-1358">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1358">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="5debd-1359">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1359">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="5debd-1360">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="5debd-1360">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="5debd-1361">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-1361">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1362">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1362">CosmosDB</span></span>

* <span data-ttu-id="5debd-1363">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5debd-1363">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="5debd-1364">Kusto</span><span class="sxs-lookup"><span data-stu-id="5debd-1364">Kusto</span></span>

* <span data-ttu-id="5debd-1365">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="5debd-1365">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1366">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1366">Network</span></span>

* <span data-ttu-id="5debd-1367">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1367">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="5debd-1368">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1368">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="5debd-1369">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1369">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="5debd-1370">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1370">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="5debd-1371">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1371">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="5debd-1372">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1372">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="5debd-1373">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1373">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1374">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1374">Resource</span></span>

* <span data-ttu-id="5debd-1375">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-1375">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="5debd-1376">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1376">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="5debd-1377">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1377">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="5debd-1378">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1378">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="5debd-1379">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1379">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1380">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1380">Role</span></span>

* <span data-ttu-id="5debd-1381">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1381">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1382">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1382">VM</span></span>

* <span data-ttu-id="5debd-1383">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-1383">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="5debd-1384">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1384">February 12, 2019</span></span>

<span data-ttu-id="5debd-1385">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="5debd-1385">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1386">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1386">Core</span></span>

* <span data-ttu-id="5debd-1387">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="5debd-1387">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="5debd-1388">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-1388">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1389">ACR</span></span>
* <span data-ttu-id="5debd-1390">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1390">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="5debd-1391">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1391">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1392">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1392">ACS</span></span>
* <span data-ttu-id="5debd-1393">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5debd-1393">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="5debd-1394">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1394">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="5debd-1395">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="5debd-1395">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-1396">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-1396">AMS</span></span>
* <span data-ttu-id="5debd-1397">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1397">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="5debd-1398">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1398">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1399">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1399">Appservice</span></span>
* <span data-ttu-id="5debd-1400">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-1400">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="5debd-1401">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-1401">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="5debd-1402">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1402">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="5debd-1403">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-1403">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="5debd-1404">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1404">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1405">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1405">Botservice</span></span>
* <span data-ttu-id="5debd-1406">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1406">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="5debd-1407">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1407">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="5debd-1408">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1408">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="5debd-1409">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5debd-1409">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="5debd-1410">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1410">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="5debd-1411">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-1411">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="5debd-1412">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1412">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="5debd-1413">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-1413">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="5debd-1414">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="5debd-1414">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="5debd-1415">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="5debd-1415">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-1416">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-1416">Key Vault</span></span>
* <span data-ttu-id="5debd-1417">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1417">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1418">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1418">Monitor</span></span>
* <span data-ttu-id="5debd-1419">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1419">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1420">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1420">Network</span></span>
* <span data-ttu-id="5debd-1421">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="5debd-1421">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="5debd-1422">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1422">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="5debd-1423">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-1423">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="5debd-1424">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1424">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5debd-1425">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5debd-1425">Policy Insights</span></span>
* <span data-ttu-id="5debd-1426">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1426">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1427">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-1427">RDBMS</span></span>
* <span data-ttu-id="5debd-1428">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-1428">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="5debd-1429">Redis</span><span class="sxs-lookup"><span data-stu-id="5debd-1429">Redis</span></span>
* <span data-ttu-id="5debd-1430">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5debd-1430">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="5debd-1431">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5debd-1431">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="5debd-1432">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="5debd-1432">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="5debd-1433">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="5debd-1433">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="5debd-1434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1434">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="5debd-1435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="5debd-1435">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="5debd-1436">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5debd-1436">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1437">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1437">Role</span></span>
* <span data-ttu-id="5debd-1438">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1438">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5debd-1439">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1439">SQL VM</span></span>
* <span data-ttu-id="5debd-1440">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1440">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1441">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1441">VM</span></span>
* <span data-ttu-id="5debd-1442">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1442">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="5debd-1443">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1443">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="5debd-1444">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="5debd-1444">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="5debd-1445">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1445">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="5debd-1446">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1446">January 31, 2019</span></span>

<span data-ttu-id="5debd-1447">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="5debd-1447">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1448">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1448">Core</span></span>

* <span data-ttu-id="5debd-1449">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="5debd-1449">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="5debd-1450">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1450">January 28, 2019</span></span>

<span data-ttu-id="5debd-1451">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="5debd-1451">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1452">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1452">ACR</span></span>
* <span data-ttu-id="5debd-1453">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1453">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1454">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1454">ACS</span></span>
* <span data-ttu-id="5debd-1455">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1455">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5debd-1456">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="5debd-1456">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="5debd-1457">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1457">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-1458">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-1458">AMS</span></span>
* <span data-ttu-id="5debd-1459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1459">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="5debd-1460">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1460">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1461">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1461">Appservice</span></span>
* <span data-ttu-id="5debd-1462">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1462">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="5debd-1463">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-1463">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="5debd-1464">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5debd-1464">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1465">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1465">Container</span></span>
* <span data-ttu-id="5debd-1466">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1466">Added `container start` command</span></span>
* <span data-ttu-id="5debd-1467">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1467">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5debd-1468">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5debd-1468">EventGrid</span></span>
* <span data-ttu-id="5debd-1469">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1469">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="5debd-1470">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1470">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="5debd-1471">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-1471">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="5debd-1472">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="5debd-1472">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="5debd-1473">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-1473">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-1474">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-1474">HDInsight</span></span>
* <span data-ttu-id="5debd-1475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1475">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="5debd-1476">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1476">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="5debd-1477">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1477">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="5debd-1478">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="5debd-1478">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="5debd-1479">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1479">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="5debd-1480">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1480">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1481">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1481">IoT</span></span>
* <span data-ttu-id="5debd-1482">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="5debd-1482">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="5debd-1483">Kusto</span><span class="sxs-lookup"><span data-stu-id="5debd-1483">Kusto</span></span>
* <span data-ttu-id="5debd-1484">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5debd-1484">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1485">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1485">Monitor</span></span>
* <span data-ttu-id="5debd-1486">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-1486">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-1487">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-1487">Profile</span></span>
* <span data-ttu-id="5debd-1488">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1488">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1489">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1489">Network</span></span>
* <span data-ttu-id="5debd-1490">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1490">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="5debd-1491">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="5debd-1491">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1492">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1492">Resource</span></span>
* <span data-ttu-id="5debd-1493">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1493">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="5debd-1494">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1494">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="5debd-1495">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1495">SQL Virtual Machine</span></span>
* <span data-ttu-id="5debd-1496">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5debd-1496">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1497">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1497">Storage</span></span>
* <span data-ttu-id="5debd-1498">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="5debd-1498">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="5debd-1499">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="5debd-1499">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1500">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1500">VM</span></span>
* <span data-ttu-id="5debd-1501">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="5debd-1501">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="5debd-1502">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1502">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="5debd-1503">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1503">January 15, 2019</span></span>

<span data-ttu-id="5debd-1504">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="5debd-1504">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1505">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1505">ACR</span></span>
* <span data-ttu-id="5debd-1506">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="5debd-1506">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="5debd-1507">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5debd-1507">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="5debd-1508">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="5debd-1508">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="5debd-1509">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1509">ACS</span></span>
* <span data-ttu-id="5debd-1510">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="5debd-1510">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1511">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1511">Appservice</span></span>
* <span data-ttu-id="5debd-1512">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1512">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="5debd-1513">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1513">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="5debd-1514">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="5debd-1514">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="5debd-1515">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1515">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1516">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1516">Botservice</span></span>
* <span data-ttu-id="5debd-1517">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1517">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="5debd-1518">Configure</span><span class="sxs-lookup"><span data-stu-id="5debd-1518">Configure</span></span>
* <span data-ttu-id="5debd-1519">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1519">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1520">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1520">CosmosDB</span></span>
* <span data-ttu-id="5debd-1521">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="5debd-1521">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-1522">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-1522">HDInsight</span></span>
* <span data-ttu-id="5debd-1523">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="5debd-1523">Added commands for managing applications</span></span>
* <span data-ttu-id="5debd-1524">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1524">Added commands for managing script actions</span></span>
* <span data-ttu-id="5debd-1525">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="5debd-1525">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="5debd-1526">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1526">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="5debd-1527">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1527">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1528">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1528">Network</span></span>
* <span data-ttu-id="5debd-1529">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1529">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="5debd-1530">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="5debd-1530">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="5debd-1531">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-1531">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="5debd-1532">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1532">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1533">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1533">Role</span></span>
* <span data-ttu-id="5debd-1534">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5debd-1534">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="5debd-1535">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="5debd-1535">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="5debd-1536">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5debd-1536">Security</span></span>
* <span data-ttu-id="5debd-1537">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-1537">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1538">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1538">Storage</span></span>
* <span data-ttu-id="5debd-1539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="5debd-1539">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="5debd-1540">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1540">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="5debd-1541">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1541">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="5debd-1542">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1542">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="5debd-1543">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1543">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1544">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1544">VM</span></span>
* <span data-ttu-id="5debd-1545">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1545">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="5debd-1546">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1546">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5debd-1547">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1547">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="5debd-1548">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1548">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="5debd-1549">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1549">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="5debd-1550">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1550">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="5debd-1551">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1551">December 20, 2018</span></span>

<span data-ttu-id="5debd-1552">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="5debd-1552">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="5debd-1553">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1553">Appservice</span></span>
* <span data-ttu-id="5debd-1554">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="5debd-1554">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="5debd-1555">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5debd-1555">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="5debd-1556">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-1556">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5debd-1557">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-1557">IoTCentral</span></span>
* <span data-ttu-id="5debd-1558">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="5debd-1558">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1559">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1559">Role</span></span>
* <span data-ttu-id="5debd-1560">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1560">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1561">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1561">SQL</span></span>
* <span data-ttu-id="5debd-1562">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5debd-1562">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1563">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1563">VM</span></span>
* <span data-ttu-id="5debd-1564">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1564">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="5debd-1565">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1565">December 18, 2018</span></span>

<span data-ttu-id="5debd-1566">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="5debd-1566">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="5debd-1567">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1567">ACR</span></span>
* <span data-ttu-id="5debd-1568">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1568">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="5debd-1569">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="5debd-1569">Condensed the table layout for task list</span></span>
* <span data-ttu-id="5debd-1570">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="5debd-1570">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1571">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1571">ACS</span></span>
* <span data-ttu-id="5debd-1572">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1572">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5debd-1573">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="5debd-1573">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="5debd-1574">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5debd-1574">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="5debd-1575">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1575">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="5debd-1576">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1576">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="5debd-1577">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1577">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1578">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1578">Appservice</span></span>
* <span data-ttu-id="5debd-1579">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1579">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="5debd-1580">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1580">Botservice</span></span>
* <span data-ttu-id="5debd-1581">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1581">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="5debd-1582">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="5debd-1582">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="5debd-1583">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="5debd-1583">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="5debd-1584">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="5debd-1584">Reduced Kudu network calls</span></span>
* <span data-ttu-id="5debd-1585">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-1585">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-1586">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-1586">Consumption</span></span>
* <span data-ttu-id="5debd-1587">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1587">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1588">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1588">CosmosDB</span></span>
* <span data-ttu-id="5debd-1589">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="5debd-1589">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="5debd-1590">Maps</span><span class="sxs-lookup"><span data-stu-id="5debd-1590">Maps</span></span>
* <span data-ttu-id="5debd-1591">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="5debd-1591">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1592">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1592">Network</span></span>
* <span data-ttu-id="5debd-1593">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1593">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="5debd-1594">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="5debd-1594">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1595">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1595">Resource</span></span>
* <span data-ttu-id="5debd-1596">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1596">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="5debd-1597">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1597">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1598">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1598">Storage</span></span>
*  <span data-ttu-id="5debd-1599">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-1599">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1600">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1600">VM</span></span>
* <span data-ttu-id="5debd-1601">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1601">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="5debd-1602">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1602">December 4, 2018</span></span>

<span data-ttu-id="5debd-1603">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="5debd-1603">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="5debd-1604">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1604">Core</span></span>
* <span data-ttu-id="5debd-1605">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1605">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="5debd-1606">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="5debd-1606">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1607">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1607">Appservice</span></span>
* <span data-ttu-id="5debd-1608">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1608">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="5debd-1609">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="5debd-1609">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1610">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1610">Network</span></span>
* <span data-ttu-id="5debd-1611">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="5debd-1611">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1612">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1612">Role</span></span>
* <span data-ttu-id="5debd-1613">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1613">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="5debd-1614">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1614">VM</span></span>
* <span data-ttu-id="5debd-1615">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5debd-1615">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="5debd-1616">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="5debd-1616">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="5debd-1617">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="5debd-1617">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="5debd-1618">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="5debd-1618">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="5debd-1619">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1619">November 20, 2018</span></span>

<span data-ttu-id="5debd-1620">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="5debd-1620">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="5debd-1621">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1621">Core</span></span>
* <span data-ttu-id="5debd-1622">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="5debd-1622">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1623">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1623">ACR</span></span>
* <span data-ttu-id="5debd-1624">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="5debd-1624">Added context token to task step</span></span>
* <span data-ttu-id="5debd-1625">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-1625">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="5debd-1626">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1626">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1627">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-1627">Appservice</span></span>
* <span data-ttu-id="5debd-1628">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1628">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="5debd-1629">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1629">Updated the default `node_version`.</span></span> <span data-ttu-id="5debd-1630">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1630">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="5debd-1631">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="5debd-1631">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="5debd-1632">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5debd-1632">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5debd-1633">IotCentral</span><span class="sxs-lookup"><span data-stu-id="5debd-1633">IotCentral</span></span>
* <span data-ttu-id="5debd-1634">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5debd-1634">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-1635">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-1635">KeyVault</span></span>
* <span data-ttu-id="5debd-1636">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="5debd-1636">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1637">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1637">Network</span></span>
* <span data-ttu-id="5debd-1638">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1638">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="5debd-1639">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1639">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="5debd-1640">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="5debd-1640">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="5debd-1641">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1641">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1642">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5debd-1642">Rdbms</span></span>
* <span data-ttu-id="5debd-1643">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-1643">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="5debd-1644">RBAC:</span><span class="sxs-lookup"><span data-stu-id="5debd-1644">Rbac</span></span>
* <span data-ttu-id="5debd-1645">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1645">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="5debd-1646">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="5debd-1646">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="5debd-1647">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1647">Storage</span></span>
* <span data-ttu-id="5debd-1648">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-1648">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="5debd-1649">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1649">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="5debd-1650">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5debd-1650">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="5debd-1651">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1651">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1652">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1652">VM</span></span>
* <span data-ttu-id="5debd-1653">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="5debd-1653">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="5debd-1654">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1654">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="5debd-1655">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1655">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="5debd-1656">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="5debd-1656">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="5debd-1657">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1657">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="5debd-1658">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1658">Added `snapshot wait` command</span></span>
* <span data-ttu-id="5debd-1659">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1659">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="5debd-1660">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1660">November 6, 2018</span></span>

<span data-ttu-id="5debd-1661">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="5debd-1661">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1662">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1662">Core</span></span>
* <span data-ttu-id="5debd-1663">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="5debd-1663">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1664">ACR</span></span>
* <span data-ttu-id="5debd-1665">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="5debd-1665">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="5debd-1666">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="5debd-1666">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1667">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1667">ACS</span></span>
* <span data-ttu-id="5debd-1668">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1668">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="5debd-1669">Помощник</span><span class="sxs-lookup"><span data-stu-id="5debd-1669">Advisor</span></span>
* <span data-ttu-id="5debd-1670">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5debd-1670">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-1671">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-1671">AMS</span></span>
* <span data-ttu-id="5debd-1672">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="5debd-1672">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="5debd-1673">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="5debd-1673">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="5debd-1674">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1674">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="5debd-1675">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="5debd-1675">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="5debd-1676">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1676">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="5debd-1677">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1677">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="5debd-1678">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1678">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="5debd-1679">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1679">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="5debd-1680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1680">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="5debd-1681">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1681">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="5debd-1682">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1682">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="5debd-1683">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1683">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="5debd-1684">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="5debd-1684">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="5debd-1685">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="5debd-1685">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="5debd-1686">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1686">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="5debd-1687">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="5debd-1687">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="5debd-1688">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="5debd-1688">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1689">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1689">AppService</span></span>
* <span data-ttu-id="5debd-1690">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="5debd-1690">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="5debd-1691">Configure</span><span class="sxs-lookup"><span data-stu-id="5debd-1691">Configure</span></span>
* <span data-ttu-id="5debd-1692">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-1692">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1693">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1693">Container</span></span>
* <span data-ttu-id="5debd-1694">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="5debd-1694">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="5debd-1695">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5debd-1695">EventHub</span></span>
* <span data-ttu-id="5debd-1696">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1696">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-1697">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-1697">Interactive</span></span>
* <span data-ttu-id="5debd-1698">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="5debd-1698">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1699">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1699">Monitor</span></span>
* <span data-ttu-id="5debd-1700">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1700">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1701">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1701">Network</span></span>
* <span data-ttu-id="5debd-1702">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1702">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="5debd-1703">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5debd-1703">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="5debd-1704">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1704">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="5debd-1705">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-1705">Profile</span></span>
* <span data-ttu-id="5debd-1706">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1706">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1707">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-1707">RDBMS</span></span>
* <span data-ttu-id="5debd-1708">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-1708">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1709">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1709">Resource</span></span>
* <span data-ttu-id="5debd-1710">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1710">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1711">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1711">Role</span></span>
* <span data-ttu-id="5debd-1712">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1712">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="5debd-1713">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1713">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="5debd-1714">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="5debd-1714">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1715">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1715">Storage</span></span>
* <span data-ttu-id="5debd-1716">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1716">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1717">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1717">VM</span></span>
* <span data-ttu-id="5debd-1718">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="5debd-1718">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="5debd-1719">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-1719">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="5debd-1720">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="5debd-1720">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="5debd-1721">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="5debd-1721">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="5debd-1722">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-1722">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="5debd-1723">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1723">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="5debd-1724">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1724">October 23, 2018</span></span>

<span data-ttu-id="5debd-1725">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="5debd-1725">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1726">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1726">Core</span></span>
* <span data-ttu-id="5debd-1727">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1727">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="5debd-1728">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1728">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1729">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1729">ACR</span></span>
* <span data-ttu-id="5debd-1730">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="5debd-1730">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-1731">CDN</span></span>
* <span data-ttu-id="5debd-1732">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1732">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5debd-1733">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5debd-1733">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1734">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1734">Container</span></span>
* <span data-ttu-id="5debd-1735">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="5debd-1735">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="5debd-1736">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="5debd-1736">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="5debd-1737">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1737">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="5debd-1738">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1738">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="5debd-1739">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1739">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="5debd-1740">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1740">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="5debd-1741">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1741">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-1742">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-1742">CosmosDB</span></span>
* <span data-ttu-id="5debd-1743">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1743">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-1744">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-1744">Interactive</span></span>
* <span data-ttu-id="5debd-1745">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1745">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="5debd-1746">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-1746">IoT Central</span></span>
* <span data-ttu-id="5debd-1747">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5debd-1747">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="5debd-1748">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="5debd-1748">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1749">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1749">Monitor</span></span>
* <span data-ttu-id="5debd-1750">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="5debd-1750">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="5debd-1751">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1751">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="5debd-1752">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-1752">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5debd-1753">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-1753">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="5debd-1754">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1754">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="5debd-1755">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="5debd-1755">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="5debd-1756">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="5debd-1756">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="5debd-1757">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-1757">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5debd-1758">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-1758">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="5debd-1759">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1759">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1760">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1760">Network</span></span>
* <span data-ttu-id="5debd-1761">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5debd-1761">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="5debd-1762">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5debd-1762">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="5debd-1763">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-1763">ServiceBus</span></span>
* <span data-ttu-id="5debd-1764">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5debd-1764">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1765">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1765">SQL</span></span>
* <span data-ttu-id="5debd-1766">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5debd-1766">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1767">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1767">Storage</span></span>
* <span data-ttu-id="5debd-1768">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1768">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="5debd-1769">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="5debd-1769">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1770">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1770">VM</span></span>
* <span data-ttu-id="5debd-1771">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="5debd-1771">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="5debd-1772">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="5debd-1772">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="5debd-1773">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="5debd-1773">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="5debd-1774">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1774">October 16, 2018</span></span>

<span data-ttu-id="5debd-1775">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="5debd-1775">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1776">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1776">VM</span></span>
* <span data-ttu-id="5debd-1777">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-1777">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="5debd-1778">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1778">October 9, 2018</span></span>

<span data-ttu-id="5debd-1779">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="5debd-1779">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1780">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1780">Core</span></span>
* <span data-ttu-id="5debd-1781">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="5debd-1781">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1782">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1782">ACR</span></span>
* <span data-ttu-id="5debd-1783">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="5debd-1783">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1784">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1784">ACS</span></span>
* <span data-ttu-id="5debd-1785">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="5debd-1785">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="5debd-1786">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="5debd-1786">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="5debd-1787">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1787">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="5debd-1788">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1788">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1789">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1789">Container</span></span>
* <span data-ttu-id="5debd-1790">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1790">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="5debd-1791">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-1791">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="5debd-1792">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="5debd-1792">Event Hub</span></span>
* <span data-ttu-id="5debd-1793">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1793">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="5debd-1794">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5debd-1794">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="5debd-1795">Модули</span><span class="sxs-lookup"><span data-stu-id="5debd-1795">Extensions</span></span>
* <span data-ttu-id="5debd-1796">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="5debd-1796">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5debd-1797">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5debd-1797">HDInsight</span></span>
* <span data-ttu-id="5debd-1798">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-1798">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1799">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1799">IoT</span></span>
* <span data-ttu-id="5debd-1800">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1800">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-1801">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-1801">KeyVault</span></span>
* <span data-ttu-id="5debd-1802">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="5debd-1802">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1803">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1803">Network</span></span>
* <span data-ttu-id="5debd-1804">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1804">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="5debd-1805">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="5debd-1805">See #6052</span></span>
* <span data-ttu-id="5debd-1806">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1806">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="5debd-1807">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5debd-1807">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="5debd-1808">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1808">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="5debd-1809">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1809">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="5debd-1810">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1810">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="5debd-1811">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1811">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1812">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1812">Role</span></span>
* <span data-ttu-id="5debd-1813">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1813">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="5debd-1814">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1814">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="5debd-1815">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1815">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="5debd-1816">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="5debd-1816">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="5debd-1817">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-1817">Service Bus</span></span>
* <span data-ttu-id="5debd-1818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5debd-1818">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1819">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1819">VM</span></span>
* <span data-ttu-id="5debd-1820">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1820">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="5debd-1821">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1821">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="5debd-1822">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1822">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="5debd-1823">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1823">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="5debd-1824">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1824">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="5debd-1825">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="5debd-1825">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="5debd-1826">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1826">September 21, 2018</span></span>

<span data-ttu-id="5debd-1827">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="5debd-1827">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1828">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1828">ACR</span></span>
* <span data-ttu-id="5debd-1829">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-1829">Added ACR Task commands</span></span>
* <span data-ttu-id="5debd-1830">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="5debd-1830">Added quick run command</span></span>
* <span data-ttu-id="5debd-1831">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1831">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="5debd-1832">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-1832">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="5debd-1833">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="5debd-1833">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="5debd-1834">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1834">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1835">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1835">ACS</span></span>
* <span data-ttu-id="5debd-1836">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1836">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="5debd-1837">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1837">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1838">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1838">AppService</span></span>

* <span data-ttu-id="5debd-1839">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="5debd-1839">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="5debd-1840">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="5debd-1840">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="5debd-1841">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-1841">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="5debd-1842">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5debd-1842">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1843">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1843">Batch</span></span>
* <span data-ttu-id="5debd-1844">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="5debd-1844">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="5debd-1845">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1845">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="5debd-1846">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1846">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="5debd-1847">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="5debd-1847">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5debd-1848">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-1848">Batch AI</span></span> 
* <span data-ttu-id="5debd-1849">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1849">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5debd-1850">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5debd-1850">Cognitive Services</span></span>
* <span data-ttu-id="5debd-1851">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1851">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="5debd-1852">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1852">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="5debd-1853">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1853">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="5debd-1854">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1854">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="5debd-1855">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5debd-1855">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="5debd-1856">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1856">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1857">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1857">Container</span></span>
* <span data-ttu-id="5debd-1858">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1858">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="5debd-1859">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="5debd-1859">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="5debd-1860">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-1860">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="5debd-1861">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1861">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="5debd-1862">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5debd-1862">Datalake</span></span>
* <span data-ttu-id="5debd-1863">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-1863">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="5debd-1864">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="5debd-1864">Interactive Shell</span></span>
* <span data-ttu-id="5debd-1865">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-1865">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="5debd-1866">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1866">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1867">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1867">IoT</span></span>
* <span data-ttu-id="5debd-1868">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1868">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-1869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5debd-1869">Key Vault</span></span>
* <span data-ttu-id="5debd-1870">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="5debd-1870">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1871">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1871">Network</span></span>
* <span data-ttu-id="5debd-1872">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1872">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="5debd-1873">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-1873">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="5debd-1874">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="5debd-1874">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="5debd-1875">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1875">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="5debd-1876">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1876">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="5debd-1877">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1877">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="5debd-1878">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-1878">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="5debd-1879">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1879">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="5debd-1880">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1880">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="5debd-1881">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1881">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="5debd-1882">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1882">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="5debd-1883">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1883">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="5debd-1884">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1884">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="5debd-1885">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="5debd-1885">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="5debd-1886">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1886">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="5debd-1887">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5debd-1887">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="5debd-1888">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5debd-1888">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="5debd-1889">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5debd-1889">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-1890">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-1890">RDBMS</span></span>
* <span data-ttu-id="5debd-1891">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5debd-1891">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="5debd-1892">резервирование.</span><span class="sxs-lookup"><span data-stu-id="5debd-1892">Reservation</span></span>
* <span data-ttu-id="5debd-1893">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1893">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="5debd-1894">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="5debd-1894">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="5debd-1895">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="5debd-1895">Manage App</span></span>
* <span data-ttu-id="5debd-1896">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5debd-1896">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="5debd-1897">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5debd-1897">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="5debd-1898">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-1898">Role</span></span>
* <span data-ttu-id="5debd-1899">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="5debd-1899">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="5debd-1900">SignalR</span><span class="sxs-lookup"><span data-stu-id="5debd-1900">SignalR</span></span>
* <span data-ttu-id="5debd-1901">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-1901">First release</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1902">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1902">Storage</span></span>
* <span data-ttu-id="5debd-1903">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="5debd-1903">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="5debd-1904">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="5debd-1904">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1905">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1905">VM</span></span>
* <span data-ttu-id="5debd-1906">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="5debd-1906">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="5debd-1907">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1907">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="5debd-1908">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1908">August 28, 2018</span></span>

<span data-ttu-id="5debd-1909">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="5debd-1909">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1910">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1910">Core</span></span>

* <span data-ttu-id="5debd-1911">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5debd-1911">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="5debd-1912">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5debd-1912">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1913">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1913">ACR</span></span>

* <span data-ttu-id="5debd-1914">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5debd-1914">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="5debd-1915">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1915">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1916">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1916">ACS</span></span>

* <span data-ttu-id="5debd-1917">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1917">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="5debd-1918">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="5debd-1918">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-1919">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1919">AppService</span></span>

* <span data-ttu-id="5debd-1920">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="5debd-1920">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="5debd-1921">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="5debd-1921">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="5debd-1922">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1922">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-1923">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-1923">Backup</span></span>

* <span data-ttu-id="5debd-1924">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1924">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="5debd-1925">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1925">Bot Service</span></span>

* <span data-ttu-id="5debd-1926">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="5debd-1926">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5debd-1927">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5debd-1927">Cognitive Services</span></span>

* <span data-ttu-id="5debd-1928">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="5debd-1928">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-1929">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1929">IoT</span></span>

* <span data-ttu-id="5debd-1930">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="5debd-1930">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-1931">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-1931">Monitor</span></span>

* <span data-ttu-id="5debd-1932">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-1932">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="5debd-1933">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="5debd-1933">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5debd-1934">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-1934">Network</span></span>

* <span data-ttu-id="5debd-1935">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1935">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-1936">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-1936">Resource</span></span>

* <span data-ttu-id="5debd-1937">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1937">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1938">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1938">Storage</span></span>

* <span data-ttu-id="5debd-1939">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1939">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1940">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1940">VM</span></span>

* <span data-ttu-id="5debd-1941">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5debd-1941">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="5debd-1942">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1942">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="5debd-1943">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1943">Auguest 14, 2018</span></span>

<span data-ttu-id="5debd-1944">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="5debd-1944">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="5debd-1945">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-1945">Core</span></span>

* <span data-ttu-id="5debd-1946">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1946">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="5debd-1947">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="5debd-1947">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="5debd-1948">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="5debd-1948">Telemetry</span></span>

* <span data-ttu-id="5debd-1949">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5debd-1949">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1950">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1950">ACR</span></span>

* <span data-ttu-id="5debd-1951">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1951">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="5debd-1952">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1952">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1953">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1953">ACS</span></span>

* <span data-ttu-id="5debd-1954">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-1954">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="5debd-1955">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="5debd-1955">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="5debd-1956">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5debd-1956">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="5debd-1957">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5debd-1957">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="5debd-1958">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-1958">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="5debd-1959">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-1959">AppService</span></span>

* <span data-ttu-id="5debd-1960">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-1960">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="5debd-1961">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5debd-1961">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-1962">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-1962">BatchAI</span></span>

* <span data-ttu-id="5debd-1963">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="5debd-1963">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="5debd-1964">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1964">Container</span></span>

* <span data-ttu-id="5debd-1965">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="5debd-1965">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="5debd-1966">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-1966">IoT</span></span>

* <span data-ttu-id="5debd-1967">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1967">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="5debd-1968">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1968">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="5debd-1969">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-1969">Iot Central</span></span>

* <span data-ttu-id="5debd-1970">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="5debd-1970">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-1971">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-1971">KeyVault</span></span>


* <span data-ttu-id="5debd-1972">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="5debd-1972">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="5debd-1973">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-1973">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="5debd-1974">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="5debd-1974">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="5debd-1975">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1975">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="5debd-1976">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-1976">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="5debd-1977">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="5debd-1977">Relay</span></span>

* <span data-ttu-id="5debd-1978">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-1978">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-1979">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-1979">Sql</span></span>

* <span data-ttu-id="5debd-1980">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1980">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-1981">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-1981">Storage</span></span>

* <span data-ttu-id="5debd-1982">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="5debd-1982">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="5debd-1983">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="5debd-1983">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="5debd-1984">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="5debd-1984">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="5debd-1985">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="5debd-1985">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="5debd-1986">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="5debd-1986">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-1987">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-1987">VM</span></span>

* <span data-ttu-id="5debd-1988">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="5debd-1988">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="5debd-1989">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-1989">July 31, 2018</span></span>

<span data-ttu-id="5debd-1990">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="5debd-1990">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-1991">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-1991">ACR</span></span>

* <span data-ttu-id="5debd-1992">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1992">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="5debd-1993">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="5debd-1993">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-1994">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-1994">ACS</span></span>

* <span data-ttu-id="5debd-1995">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="5debd-1995">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-1996">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-1996">Batch</span></span>

* <span data-ttu-id="5debd-1997">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="5debd-1997">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="5debd-1998">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-1998">Container</span></span>

* <span data-ttu-id="5debd-1999">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-1999">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2000">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2000">Network</span></span>

* <span data-ttu-id="5debd-2001">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2001">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="5debd-2002">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2002">Resource</span></span>

* <span data-ttu-id="5debd-2003">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2003">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="5debd-2004">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="5debd-2004">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2005">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2005">Role</span></span>

* <span data-ttu-id="5debd-2006">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5debd-2006">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="5debd-2007">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="5debd-2007">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="5debd-2008">Поиск</span><span class="sxs-lookup"><span data-stu-id="5debd-2008">Search</span></span>

* <span data-ttu-id="5debd-2009">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="5debd-2009">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="5debd-2010">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-2010">Service Bus</span></span>

* <span data-ttu-id="5debd-2011">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5debd-2011">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="5debd-2012">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="5debd-2012">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="5debd-2013">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="5debd-2013">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="5debd-2014">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2014">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2015">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2015">Storage</span></span>

* <span data-ttu-id="5debd-2016">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2016">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="5debd-2017">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="5debd-2017">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2018">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2018">VM</span></span>

* <span data-ttu-id="5debd-2019">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="5debd-2019">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="5debd-2020">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2020">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="5debd-2021">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-2021">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="5debd-2022">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="5debd-2022">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="5debd-2023">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2023">July 18, 2018</span></span>

<span data-ttu-id="5debd-2024">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="5debd-2024">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2025">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2025">Core</span></span>

* <span data-ttu-id="5debd-2026">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="5debd-2026">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="5debd-2027">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="5debd-2027">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="5debd-2028">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5debd-2028">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2029">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2029">ACR</span></span>

* <span data-ttu-id="5debd-2030">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="5debd-2030">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="5debd-2031">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2031">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="5debd-2032">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2032">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="5debd-2033">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2033">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2034">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2034">ACS</span></span>

* <span data-ttu-id="5debd-2035">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="5debd-2035">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2036">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-2036">AppService</span></span>

* <span data-ttu-id="5debd-2037">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="5debd-2037">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2038">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2038">Batch</span></span>

* <span data-ttu-id="5debd-2039">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5debd-2039">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="5debd-2040">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="5debd-2040">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5debd-2041">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-2041">Batch AI</span></span>

* <span data-ttu-id="5debd-2042">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2042">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2043">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2043">Container</span></span>

* <span data-ttu-id="5debd-2044">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="5debd-2044">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="5debd-2045">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="5debd-2045">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2046">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2046">Network</span></span>

* <span data-ttu-id="5debd-2047">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2047">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="5debd-2048">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2048">Added `network nic wait`</span></span>
* <span data-ttu-id="5debd-2049">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5debd-2049">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="5debd-2050">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="5debd-2050">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="5debd-2051">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2051">Resource</span></span>

* <span data-ttu-id="5debd-2052">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2052">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="5debd-2053">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2053">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="5debd-2054">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2054">Added `deployment wait` command</span></span>
* <span data-ttu-id="5debd-2055">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="5debd-2055">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2056">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2056">SQL</span></span>

* <span data-ttu-id="5debd-2057">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2057">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="5debd-2058">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2058">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="5debd-2059">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2059">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2060">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2060">Storage</span></span>

* <span data-ttu-id="5debd-2061">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2061">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2062">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2062">VM</span></span>

* <span data-ttu-id="5debd-2063">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2063">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="5debd-2064">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2064">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="5debd-2065">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2065">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5debd-2066">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2066">July 3, 2018</span></span>

<span data-ttu-id="5debd-2067">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="5debd-2067">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-2068">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-2068">AKS</span></span>

* <span data-ttu-id="5debd-2069">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2069">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5debd-2070">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2070">July 3, 2018</span></span>

<span data-ttu-id="5debd-2071">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="5debd-2071">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2072">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2072">Core</span></span>

* <span data-ttu-id="5debd-2073">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2073">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2074">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2074">ACR</span></span>

* <span data-ttu-id="5debd-2075">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="5debd-2075">Added polling build status</span></span>
* <span data-ttu-id="5debd-2076">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5debd-2076">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="5debd-2077">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2077">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2078">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2078">ACS</span></span>

* <span data-ttu-id="5debd-2079">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2079">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="5debd-2080">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2080">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="5debd-2081">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2081">Updated options for `aks browse` command.</span></span> <span data-ttu-id="5debd-2082">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2082">Added `--listen-port` support</span></span>
* <span data-ttu-id="5debd-2083">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2083">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="5debd-2084">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="5debd-2084">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="5debd-2085">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2085">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2086">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-2086">AppService</span></span>

* <span data-ttu-id="5debd-2087">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2087">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="5debd-2088">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2088">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-2089">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2089">Backup</span></span>

* <span data-ttu-id="5debd-2090">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="5debd-2090">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-2091">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-2091">BatchAI</span></span>

* <span data-ttu-id="5debd-2092">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2092">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="5debd-2093">Cloud</span><span class="sxs-lookup"><span data-stu-id="5debd-2093">Cloud</span></span>

* <span data-ttu-id="5debd-2094">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2094">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2095">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2095">Container</span></span>

* <span data-ttu-id="5debd-2096">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2096">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="5debd-2097">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2097">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="5debd-2098">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="5debd-2098">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2099">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2099">Extension</span></span>

* <span data-ttu-id="5debd-2100">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2100">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2101">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2101">Network</span></span>

* <span data-ttu-id="5debd-2102">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="5debd-2102">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-2103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5debd-2103">Rdbms</span></span>

* <span data-ttu-id="5debd-2104">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2104">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2105">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2105">Resource</span></span>

* <span data-ttu-id="5debd-2106">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2106">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2107">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2107">VM</span></span>

* <span data-ttu-id="5debd-2108">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5debd-2108">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="5debd-2109">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2109">June 25, 2018</span></span>

<span data-ttu-id="5debd-2110">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="5debd-2110">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="5debd-2111">CLI</span><span class="sxs-lookup"><span data-stu-id="5debd-2111">CLI</span></span>

* <span data-ttu-id="5debd-2112">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2112">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5debd-2113">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2113">June 19, 2018</span></span>

<span data-ttu-id="5debd-2114">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5debd-2114">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2115">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2115">Core</span></span>

* <span data-ttu-id="5debd-2116">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2116">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2117">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2117">ACR</span></span>

* <span data-ttu-id="5debd-2118">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2118">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5debd-2119">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="5debd-2119">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2120">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2120">ACS</span></span>

* <span data-ttu-id="5debd-2121">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2121">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5debd-2122">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2122">Added `--update` support</span></span>
* <span data-ttu-id="5debd-2123">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2123">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5debd-2124">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2124">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5debd-2125">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2125">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5debd-2126">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2126">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5debd-2127">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2127">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5debd-2128">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2128">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2129">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-2129">AppService</span></span>

* <span data-ttu-id="5debd-2130">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="5debd-2130">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5debd-2131">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2131">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2132">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2132">Batch</span></span>

* <span data-ttu-id="5debd-2133">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2133">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5debd-2134">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-2134">Batch AI</span></span>

* <span data-ttu-id="5debd-2135">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="5debd-2135">Added support for workspaces.</span></span> <span data-ttu-id="5debd-2136">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2136">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5debd-2137">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2137">Added support for experiments.</span></span> <span data-ttu-id="5debd-2138">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="5debd-2138">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5debd-2139">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="5debd-2139">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5debd-2140">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2140">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5debd-2141">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2141">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5debd-2142">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2142">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="5debd-2143">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="5debd-2143">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5debd-2144">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2144">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5debd-2145">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2145">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5debd-2146">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2146">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5debd-2147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2147">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5debd-2148">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2148">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5debd-2149">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2149">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5debd-2150">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="5debd-2150">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5debd-2151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2151">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5debd-2152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="5debd-2152">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="5debd-2153">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="5debd-2153">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="5debd-2154">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="5debd-2154">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5debd-2155">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="5debd-2155">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5debd-2156">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="5debd-2156">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5debd-2157">Maps</span><span class="sxs-lookup"><span data-stu-id="5debd-2157">Maps</span></span>

* <span data-ttu-id="5debd-2158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2158">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2159">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2159">Network</span></span>

* <span data-ttu-id="5debd-2160">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="5debd-2160">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5debd-2161">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-2161">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5debd-2162">#6502</span><span class="sxs-lookup"><span data-stu-id="5debd-2162">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5debd-2163">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2163">Reservations</span></span>

* <span data-ttu-id="5debd-2164">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2164">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5debd-2165">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2165">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5debd-2166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2166">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5debd-2167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2167">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5debd-2168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2168">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5debd-2169">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2169">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2170">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2170">Role</span></span>

* <span data-ttu-id="5debd-2171">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5debd-2171">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2172">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2172">SQL</span></span>

* <span data-ttu-id="5debd-2173">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2173">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2174">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2174">Storage</span></span>

* <span data-ttu-id="5debd-2175">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-2175">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2176">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2176">VM</span></span>

* <span data-ttu-id="5debd-2177">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2177">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5debd-2178">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2178">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5debd-2179">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="5debd-2179">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5debd-2180">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2180">June 13, 2018</span></span>

<span data-ttu-id="5debd-2181">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5debd-2181">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2182">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2182">Core</span></span>

* <span data-ttu-id="5debd-2183">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="5debd-2183">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5debd-2184">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2184">June 13, 2018</span></span>

<span data-ttu-id="5debd-2185">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5debd-2185">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-2186">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-2186">AKS</span></span>

* <span data-ttu-id="5debd-2187">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="5debd-2187">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5debd-2188">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="5debd-2188">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="5debd-2189">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2189">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5debd-2190">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2190">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5debd-2191">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5debd-2191">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2192">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-2192">AppService</span></span>

* <span data-ttu-id="5debd-2193">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="5debd-2193">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5debd-2194">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2194">June 5, 2018</span></span>

<span data-ttu-id="5debd-2195">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5debd-2195">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2196">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2196">Interactive</span></span>

* <span data-ttu-id="5debd-2197">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="5debd-2197">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5debd-2198">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2198">June 5, 2018</span></span>

<span data-ttu-id="5debd-2199">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5debd-2199">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2200">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2200">Core</span></span>

* <span data-ttu-id="5debd-2201">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="5debd-2201">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5debd-2202">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2202">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2203">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2203">ACR</span></span>

* <span data-ttu-id="5debd-2204">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="5debd-2204">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5debd-2205">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2205">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5debd-2206">AKS</span><span class="sxs-lookup"><span data-stu-id="5debd-2206">AKS</span></span>

* <span data-ttu-id="5debd-2207">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2207">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2208">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2208">Batch</span></span>

* <span data-ttu-id="5debd-2209">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5debd-2209">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-2210">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-2210">IOT</span></span>

* <span data-ttu-id="5debd-2211">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="5debd-2211">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2212">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2212">Network</span></span>

* <span data-ttu-id="5debd-2213">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2213">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5debd-2214">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5debd-2214">Policy Insights</span></span>

* <span data-ttu-id="5debd-2215">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-2215">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5debd-2216">ARM</span><span class="sxs-lookup"><span data-stu-id="5debd-2216">ARM</span></span>

* <span data-ttu-id="5debd-2217">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2217">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2218">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2218">SQL</span></span>

* <span data-ttu-id="5debd-2219">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="5debd-2219">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5debd-2220">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="5debd-2220">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5debd-2221">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2221">Storage</span></span>

* <span data-ttu-id="5debd-2222">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2222">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2223">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2223">VM</span></span>

* <span data-ttu-id="5debd-2224">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2224">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5debd-2225">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2225">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5debd-2226">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2226">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5debd-2227">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2227">May 22, 2018</span></span>

<span data-ttu-id="5debd-2228">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5debd-2228">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2229">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2229">Core</span></span>

* <span data-ttu-id="5debd-2230">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2230">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2231">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2231">ACS</span></span>

* <span data-ttu-id="5debd-2232">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2232">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5debd-2233">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5debd-2233">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2234">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-2234">AppService</span></span>

* <span data-ttu-id="5debd-2235">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="5debd-2235">Improved generic update commands</span></span>
* <span data-ttu-id="5debd-2236">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2236">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2237">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2237">Container</span></span>

* <span data-ttu-id="5debd-2238">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="5debd-2238">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5debd-2239">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2239">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2240">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2240">Extension</span></span>

* <span data-ttu-id="5debd-2241">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2241">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2242">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2242">Interactive</span></span>

* <span data-ttu-id="5debd-2243">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2243">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5debd-2244">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2244">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-2245">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-2245">KeyVault</span></span>

* <span data-ttu-id="5debd-2246">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="5debd-2246">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2247">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2247">Network</span></span>

* <span data-ttu-id="5debd-2248">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="5debd-2248">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5debd-2249">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="5debd-2249">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2250">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2250">SQL</span></span>

* <span data-ttu-id="5debd-2251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="5debd-2251">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5debd-2252">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2252">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5debd-2253">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2253">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="5debd-2254">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="5debd-2254">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5debd-2255">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5debd-2255">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5debd-2256">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2256">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5debd-2257">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2257">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5debd-2258">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2258">`edition`.</span></span> <span data-ttu-id="5debd-2259">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2259">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5debd-2260">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2260">`elasticPoolName`.</span></span> <span data-ttu-id="5debd-2261">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2261">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5debd-2262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5debd-2262">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5debd-2263">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2263">`edition`.</span></span> <span data-ttu-id="5debd-2264">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2264">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5debd-2265">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2265">`dtu`.</span></span> <span data-ttu-id="5debd-2266">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2266">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5debd-2267">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2267">`databaseDtuMin`.</span></span> <span data-ttu-id="5debd-2268">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2268">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5debd-2269">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2269">`databaseDtuMax`.</span></span> <span data-ttu-id="5debd-2270">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2270">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5debd-2271">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2271">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5debd-2272">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2272">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2273">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2273">Storage</span></span>

* <span data-ttu-id="5debd-2274">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2274">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5debd-2275">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2275">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2276">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2276">VM</span></span>

* <span data-ttu-id="5debd-2277">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2277">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5debd-2278">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2278">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5debd-2279">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2279">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5debd-2280">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2280">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5debd-2281">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2281">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5debd-2282">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2282">May 7, 2018</span></span>

<span data-ttu-id="5debd-2283">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5debd-2283">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2284">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2284">Core</span></span>

* <span data-ttu-id="5debd-2285">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="5debd-2285">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5debd-2286">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2286">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5debd-2287">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2287">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5debd-2288">#5591</span><span class="sxs-lookup"><span data-stu-id="5debd-2288">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5debd-2289">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2289">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5debd-2290">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="5debd-2290">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5debd-2291">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="5debd-2291">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5debd-2292">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2292">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5debd-2293">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2293">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2294">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2294">ACR</span></span>

* <span data-ttu-id="5debd-2295">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-2295">Added ACR Build commands</span></span>
* <span data-ttu-id="5debd-2296">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5debd-2296">Improved resource not found error messages</span></span>
* <span data-ttu-id="5debd-2297">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5debd-2297">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5debd-2298">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="5debd-2298">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5debd-2299">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="5debd-2299">Improved repository commands error messages</span></span>
* <span data-ttu-id="5debd-2300">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2300">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2301">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2301">ACS</span></span>

* <span data-ttu-id="5debd-2302">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2302">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5debd-2303">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="5debd-2303">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5debd-2304">AMS</span><span class="sxs-lookup"><span data-stu-id="5debd-2304">AMS</span></span>

* <span data-ttu-id="5debd-2305">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-2305">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2306">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2306">Appservice</span></span>

* <span data-ttu-id="5debd-2307">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5debd-2307">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5debd-2308">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2308">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5debd-2309">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-2309">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5debd-2310">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2310">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5debd-2311">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-2311">Batch AI</span></span>

* <span data-ttu-id="5debd-2312">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="5debd-2312">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5debd-2313">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5debd-2313">Cognitive Services</span></span>

* <span data-ttu-id="5debd-2314">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="5debd-2314">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-2315">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-2315">Consumption</span></span>

* <span data-ttu-id="5debd-2316">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="5debd-2316">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2317">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2317">Container</span></span>

* <span data-ttu-id="5debd-2318">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2318">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5debd-2319">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-2319">Cosmos DB</span></span>

* <span data-ttu-id="5debd-2320">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-2320">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5debd-2321">DMS</span><span class="sxs-lookup"><span data-stu-id="5debd-2321">DMS</span></span>

* <span data-ttu-id="5debd-2322">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-2322">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2323">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2323">Extension</span></span>

* <span data-ttu-id="5debd-2324">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="5debd-2324">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2325">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2325">Interactive</span></span>

* <span data-ttu-id="5debd-2326">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="5debd-2326">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5debd-2327">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="5debd-2327">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5debd-2328">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2328">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5debd-2329">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2329">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5debd-2330">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5debd-2330">Lab</span></span>

* <span data-ttu-id="5debd-2331">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="5debd-2331">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2332">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2332">Network</span></span>

* <span data-ttu-id="5debd-2333">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="5debd-2333">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5debd-2334">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2334">Profile</span></span>

* <span data-ttu-id="5debd-2335">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2335">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5debd-2336">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="5debd-2336">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5debd-2337">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2337">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5debd-2338">Redis</span><span class="sxs-lookup"><span data-stu-id="5debd-2338">Redis</span></span>

* <span data-ttu-id="5debd-2339">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2339">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5debd-2340">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="5debd-2340">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5debd-2341">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2341">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5debd-2342">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2342">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5debd-2343">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2343">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2344">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2344">Role</span></span>

* <span data-ttu-id="5debd-2345">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="5debd-2345">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2346">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2346">Storage</span></span>

* <span data-ttu-id="5debd-2347">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="5debd-2347">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5debd-2348">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5debd-2348">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5debd-2349">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="5debd-2349">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5debd-2350">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="5debd-2350">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5debd-2351">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="5debd-2351">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2352">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2352">VM</span></span>

* <span data-ttu-id="5debd-2353">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="5debd-2353">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5debd-2354">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="5debd-2354">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5debd-2355">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2355">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5debd-2356">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2356">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5debd-2357">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="5debd-2357">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5debd-2358">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="5debd-2358">Added write accelerator support</span></span>
* <span data-ttu-id="5debd-2359">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2359">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5debd-2360">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5debd-2360">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5debd-2361">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="5debd-2361">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5debd-2362">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2362">April 10, 2018</span></span>

<span data-ttu-id="5debd-2363">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5debd-2363">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2364">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2364">ACR</span></span>

* <span data-ttu-id="5debd-2365">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="5debd-2365">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2366">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2366">ACS</span></span>

* <span data-ttu-id="5debd-2367">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="5debd-2367">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2368">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2368">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5debd-2370">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2370">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-2371">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5debd-2371">BatchAI</span></span>

* <span data-ttu-id="5debd-2372">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-2372">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="5debd-2373">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="5debd-2373">Job level mounting</span></span>
  - <span data-ttu-id="5debd-2374">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2374">Environment variables with secret values</span></span>
  - <span data-ttu-id="5debd-2375">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="5debd-2375">Performance counters settings</span></span>
  - <span data-ttu-id="5debd-2376">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="5debd-2376">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="5debd-2377">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2377">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="5debd-2378">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="5debd-2378">Usage and limits reporting</span></span>
  - <span data-ttu-id="5debd-2379">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2379">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="5debd-2380">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2380">Support for custom images</span></span>
  - <span data-ttu-id="5debd-2381">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="5debd-2381">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5debd-2382">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="5debd-2382">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5debd-2383">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2383">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5debd-2384">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="5debd-2384">National clouds are supported</span></span>
* <span data-ttu-id="5debd-2385">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2385">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5debd-2386">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2386">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5debd-2387">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2387">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5debd-2388">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2388">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5debd-2389">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="5debd-2389">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5debd-2390">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="5debd-2390">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5debd-2391">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2391">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5debd-2392">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="5debd-2392">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5debd-2393">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="5debd-2393">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5debd-2394">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2394">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5debd-2395">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="5debd-2395">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5debd-2396">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2396">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5debd-2397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2397">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5debd-2398">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="5debd-2398">Billing</span></span>

* <span data-ttu-id="5debd-2399">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2399">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-2400">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-2400">Consumption</span></span>

* <span data-ttu-id="5debd-2401">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2401">Added `marketplace` commands</span></span>
* <span data-ttu-id="5debd-2402">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2402">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5debd-2403">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2403">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5debd-2404">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2404">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5debd-2405">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2405">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5debd-2406">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2406">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2407">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2407">Container</span></span>

* <span data-ttu-id="5debd-2408">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2408">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5debd-2409">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="5debd-2409">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2410">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2410">Extension</span></span>

* <span data-ttu-id="5debd-2411">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2411">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2412">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2412">Interactive</span></span>

* <span data-ttu-id="5debd-2413">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="5debd-2413">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5debd-2414">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2414">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5debd-2415">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2415">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2416">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2416">Network</span></span>

* <span data-ttu-id="5debd-2417">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2417">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5debd-2418">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2418">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="5debd-2419">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="5debd-2419">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="5debd-2420">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2420">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="5debd-2421">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2421">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5debd-2422">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2422">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5debd-2423">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2423">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5debd-2424">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="5debd-2424">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-2425">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2425">Profile</span></span>

* <span data-ttu-id="5debd-2426">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2426">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5debd-2427">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2427">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-2428">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-2428">RDBMS</span></span>

* <span data-ttu-id="5debd-2429">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2429">Added `georestore` command</span></span>
* <span data-ttu-id="5debd-2430">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-2430">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2431">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2431">Resource</span></span>

* <span data-ttu-id="5debd-2432">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2432">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5debd-2433">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2433">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2434">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2434">SQL</span></span>

* <span data-ttu-id="5debd-2435">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2435">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2436">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2436">Storage</span></span>

* <span data-ttu-id="5debd-2437">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="5debd-2437">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2438">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2438">VM</span></span>

* <span data-ttu-id="5debd-2439">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="5debd-2439">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5debd-2440">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2440">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="5debd-2442">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2442">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5debd-2443">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-2443">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="5debd-2444">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="5debd-2444">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="5debd-2445">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="5debd-2445">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5debd-2446">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2446">March 27, 2018</span></span>

<span data-ttu-id="5debd-2447">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5debd-2447">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2448">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2448">Core</span></span>

* <span data-ttu-id="5debd-2449">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5debd-2449">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2450">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2450">ACS</span></span>

* <span data-ttu-id="5debd-2451">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5debd-2451">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2452">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2452">Appservice</span></span>

* <span data-ttu-id="5debd-2453">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2453">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5debd-2454">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2454">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-2455">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2455">Backup</span></span>

* <span data-ttu-id="5debd-2456">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2456">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5debd-2457">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="5debd-2457">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5debd-2458">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5debd-2458">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5debd-2459">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2459">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2460">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2460">Container</span></span>

* <span data-ttu-id="5debd-2461">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2461">Added `container exec` command.</span></span> <span data-ttu-id="5debd-2462">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2462">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5debd-2463">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2463">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2464">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2464">Extension</span></span>

* <span data-ttu-id="5debd-2465">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2465">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5debd-2466">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2466">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5debd-2467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2467">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2468">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2468">Interactive</span></span>

* <span data-ttu-id="5debd-2469">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2469">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5debd-2470">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2470">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5debd-2471">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2471">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5debd-2472">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2472">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5debd-2473">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5debd-2473">Lab</span></span>

* <span data-ttu-id="5debd-2474">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2474">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2475">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2475">Monitor</span></span>

* <span data-ttu-id="5debd-2476">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="5debd-2476">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5debd-2477">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2477">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5debd-2478">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="5debd-2478">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2479">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2479">Network</span></span>

* <span data-ttu-id="5debd-2480">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2480">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-2481">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2481">Profile</span></span>

* <span data-ttu-id="5debd-2482">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2482">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-2483">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-2483">RDBMS</span></span>

* <span data-ttu-id="5debd-2484">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="5debd-2484">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2485">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2485">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5debd-2487">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2487">Role</span></span>

* <span data-ttu-id="5debd-2488">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2488">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5debd-2489">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="5debd-2489">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5debd-2490">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="5debd-2490">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5debd-2491">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2491">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5debd-2492">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2492">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2493">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2493">Storage</span></span>

* <span data-ttu-id="5debd-2494">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5debd-2494">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5debd-2495">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5debd-2495">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2496">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2496">VM</span></span>

* <span data-ttu-id="5debd-2497">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2497">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5debd-2498">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2498">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5debd-2499">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="5debd-2499">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5debd-2500">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="5debd-2500">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5debd-2501">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2501">March 13, 2018</span></span>

<span data-ttu-id="5debd-2502">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5debd-2502">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2503">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2503">ACR</span></span>

* <span data-ttu-id="5debd-2504">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2504">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5debd-2505">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-2505">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5debd-2506">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-2506">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2507">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2507">ACS</span></span>

* <span data-ttu-id="5debd-2508">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="5debd-2508">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5debd-2509">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2509">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5debd-2510">Помощник</span><span class="sxs-lookup"><span data-stu-id="5debd-2510">Advisor</span></span>

* <span data-ttu-id="5debd-2511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2511">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5debd-2512">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2512">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5debd-2513">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2513">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="5debd-2514">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2514">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5debd-2515">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2515">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2516">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2516">Appservice</span></span>

* <span data-ttu-id="5debd-2517">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5debd-2517">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5debd-2518">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2518">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5debd-2519">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5debd-2519">Eventhubs</span></span>

* <span data-ttu-id="5debd-2520">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-2520">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2521">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2521">Extension</span></span>

* <span data-ttu-id="5debd-2522">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="5debd-2522">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2523">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2523">Interactive</span></span>

* <span data-ttu-id="5debd-2524">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="5debd-2524">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5debd-2525">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="5debd-2525">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5debd-2526">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="5debd-2526">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5debd-2527">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2527">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2528">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2528">Monitor</span></span>

* <span data-ttu-id="5debd-2529">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-2529">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5debd-2530">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2530">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5debd-2531">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2531">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5debd-2532">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2532">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2533">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2533">Network</span></span>

* <span data-ttu-id="5debd-2534">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2534">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5debd-2535">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5debd-2535">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5debd-2536">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2536">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5debd-2537">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2537">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-2538">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2538">Profile</span></span>

* <span data-ttu-id="5debd-2539">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="5debd-2539">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5debd-2540">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2540">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-2541">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-2541">RDBMS</span></span>

* <span data-ttu-id="5debd-2542">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-2542">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5debd-2543">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5debd-2543">Service Bus</span></span>

* <span data-ttu-id="5debd-2544">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-2544">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2545">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2545">Storage</span></span>

* <span data-ttu-id="5debd-2546">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="5debd-2546">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5debd-2547">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2547">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2548">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2548">VM</span></span>

* <span data-ttu-id="5debd-2549">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="5debd-2549">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5debd-2550">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5debd-2550">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5debd-2551">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2551">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5debd-2552">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="5debd-2552">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5debd-2553">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="5debd-2553">February 27, 2018</span></span>

<span data-ttu-id="5debd-2554">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5debd-2554">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2555">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2555">Core</span></span>

* <span data-ttu-id="5debd-2556">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="5debd-2556">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5debd-2557">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="5debd-2557">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5debd-2558">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2558">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2559">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2559">ACS</span></span>

* <span data-ttu-id="5debd-2560">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2560">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5debd-2561">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2561">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5debd-2562">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2562">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5debd-2563">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2563">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2564">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2564">Appservice</span></span>

* <span data-ttu-id="5debd-2565">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5debd-2565">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5debd-2566">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="5debd-2566">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5debd-2567">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5debd-2567">Cognitive Services</span></span>

* <span data-ttu-id="5debd-2568">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5debd-2568">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-2569">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-2569">Consumption</span></span>

* <span data-ttu-id="5debd-2570">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="5debd-2570">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5debd-2571">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="5debd-2571">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2572">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2572">Container</span></span>

* <span data-ttu-id="5debd-2573">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2573">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2574">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2574">Network</span></span>

* <span data-ttu-id="5debd-2575">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2575">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2576">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2576">Resource</span></span>

* <span data-ttu-id="5debd-2577">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="5debd-2577">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2578">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2578">Role</span></span>

* <span data-ttu-id="5debd-2579">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2579">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2580">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2580">SQL</span></span>

* <span data-ttu-id="5debd-2581">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2581">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2582">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2582">Storage</span></span>

* <span data-ttu-id="5debd-2583">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2583">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2584">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2584">VM</span></span>

* <span data-ttu-id="5debd-2585">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2585">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5debd-2586">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2586">February 13, 2018</span></span>

<span data-ttu-id="5debd-2587">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5debd-2587">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2588">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2588">Core</span></span>

* <span data-ttu-id="5debd-2589">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="5debd-2589">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2590">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2590">ACS</span></span>

* <span data-ttu-id="5debd-2591">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="5debd-2591">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5debd-2592">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2592">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5debd-2593">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-2593">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5debd-2594">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2594">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5debd-2595">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="5debd-2595">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5debd-2596">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2596">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5debd-2597">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-2597">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5debd-2598">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2598">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2599">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2599">Appservice</span></span>

* <span data-ttu-id="5debd-2600">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2600">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5debd-2601">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2601">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-2602">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-2602">CDN</span></span>

* <span data-ttu-id="5debd-2603">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2603">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2604">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2604">Container</span></span>

* <span data-ttu-id="5debd-2605">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="5debd-2605">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5debd-2606">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2606">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-2607">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-2607">CosmosDB</span></span>

* <span data-ttu-id="5debd-2608">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2608">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2609">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2609">Extension</span></span>

* <span data-ttu-id="5debd-2610">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2610">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5debd-2611">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2611">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5debd-2612">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5debd-2612">Feedback</span></span>

* <span data-ttu-id="5debd-2613">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2613">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2614">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2614">Interactive</span></span>

* <span data-ttu-id="5debd-2615">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5debd-2615">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5debd-2616">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2616">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-2617">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-2617">IoT</span></span>

* <span data-ttu-id="5debd-2618">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5debd-2618">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5debd-2619">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5debd-2619">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5debd-2620">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2620">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5debd-2621">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2621">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2622">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2622">Monitor</span></span>

* <span data-ttu-id="5debd-2623">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2623">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2624">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2624">Network</span></span>

* <span data-ttu-id="5debd-2625">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5debd-2625">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5debd-2626">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2626">Profile</span></span>

* <span data-ttu-id="5debd-2627">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5debd-2627">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2628">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2628">Resource</span></span>

* <span data-ttu-id="5debd-2629">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2629">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2630">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2630">Role</span></span>

* <span data-ttu-id="5debd-2631">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="5debd-2631">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2632">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2632">SQL</span></span>

* <span data-ttu-id="5debd-2633">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2633">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5debd-2634">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2634">Added `sql db rename`</span></span>
* <span data-ttu-id="5debd-2635">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-2635">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2636">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2636">Storage</span></span>

* <span data-ttu-id="5debd-2637">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="5debd-2637">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2638">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2638">VM</span></span>

* <span data-ttu-id="5debd-2639">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="5debd-2639">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5debd-2640">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2640">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5debd-2641">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="5debd-2641">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5debd-2642">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2642">January 31, 2018</span></span>

<span data-ttu-id="5debd-2643">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5debd-2643">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2644">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2644">Core</span></span>

* <span data-ttu-id="5debd-2645">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="5debd-2645">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5debd-2646">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-2646">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5debd-2647">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="5debd-2647">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5debd-2648">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="5debd-2648">Use `--verbose` to see</span></span>
* <span data-ttu-id="5debd-2649">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2649">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2650">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2650">ACS</span></span>

* <span data-ttu-id="5debd-2651">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2651">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5debd-2652">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2652">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2653">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2653">Appservice</span></span>

* <span data-ttu-id="5debd-2654">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2654">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5debd-2655">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="5debd-2655">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-2656">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-2656">CDN</span></span>

* <span data-ttu-id="5debd-2657">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2657">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-2658">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-2658">CosmosDB</span></span>

* <span data-ttu-id="5debd-2659">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2659">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2660">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2660">Interactive</span></span>

* <span data-ttu-id="5debd-2661">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="5debd-2661">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2662">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2662">Network</span></span>

* <span data-ttu-id="5debd-2663">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2663">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5debd-2664">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2664">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5debd-2665">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2665">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5debd-2666">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2666">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5debd-2667">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2667">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5debd-2668">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="5debd-2668">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5debd-2669">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="5debd-2669">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5debd-2670">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="5debd-2670">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5debd-2671">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2671">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="5debd-2672">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2672">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-2673">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2673">Profile</span></span>

* <span data-ttu-id="5debd-2674">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="5debd-2674">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2675">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2675">Resource</span></span>

* <span data-ttu-id="5debd-2676">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="5debd-2676">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2677">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2677">Storage</span></span>

* <span data-ttu-id="5debd-2678">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="5debd-2678">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5debd-2679">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="5debd-2679">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5debd-2680">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2680">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="5debd-2681">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2681">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5debd-2682">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="5debd-2682">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2683">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2683">VM</span></span>

* <span data-ttu-id="5debd-2684">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="5debd-2684">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5debd-2685">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2685">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5debd-2686">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2686">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5debd-2687">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2687">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5debd-2688">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2688">January 17, 2018</span></span>

<span data-ttu-id="5debd-2689">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5debd-2689">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2690">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2690">ACR</span></span>

* <span data-ttu-id="5debd-2691">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-2691">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5debd-2692">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="5debd-2692">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2693">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2693">ACS</span></span>

* <span data-ttu-id="5debd-2694">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2694">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5debd-2695">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2695">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2696">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2696">Appservice</span></span>

* <span data-ttu-id="5debd-2697">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="5debd-2697">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5debd-2698">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2698">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5debd-2699">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2699">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-2700">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2700">Backup</span></span>

* <span data-ttu-id="5debd-2701">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5debd-2701">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5debd-2702">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5debd-2702">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5debd-2703">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="5debd-2703">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5debd-2704">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="5debd-2704">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5debd-2705">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="5debd-2705">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2706">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2706">Batch</span></span>

* <span data-ttu-id="5debd-2707">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2707">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5debd-2708">Cloud</span><span class="sxs-lookup"><span data-stu-id="5debd-2708">Cloud</span></span>

* <span data-ttu-id="5debd-2709">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2709">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-2710">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-2710">Consumption</span></span>

* <span data-ttu-id="5debd-2711">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2711">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5debd-2712">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2712">Event Grid</span></span>

* <span data-ttu-id="5debd-2713">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2713">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5debd-2714">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2714">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5debd-2715">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2715">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5debd-2716">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2716">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5debd-2717">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2717">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5debd-2718">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2718">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5debd-2719">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2719">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5debd-2720">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2720">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-2721">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-2721">Interactive</span></span>

* <span data-ttu-id="5debd-2722">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="5debd-2722">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5debd-2723">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="5debd-2723">Fixed errors on startup</span></span>
* <span data-ttu-id="5debd-2724">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5debd-2724">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-2725">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-2725">IoT</span></span>

* <span data-ttu-id="5debd-2726">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="5debd-2726">Added support for device provisioning service</span></span>
* <span data-ttu-id="5debd-2727">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="5debd-2727">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5debd-2728">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5debd-2728">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2729">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2729">Monitor</span></span>

* <span data-ttu-id="5debd-2730">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2730">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5debd-2731">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2731">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5debd-2732">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="5debd-2732">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2733">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2733">Network</span></span>

* <span data-ttu-id="5debd-2734">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="5debd-2734">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5debd-2735">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="5debd-2735">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-2736">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-2736">Profile</span></span>

* <span data-ttu-id="5debd-2737">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2737">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2738">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2738">Role</span></span>

* <span data-ttu-id="5debd-2739">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2739">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5debd-2740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-2740">Service Fabric</span></span>

* <span data-ttu-id="5debd-2741">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5debd-2741">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5debd-2742">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-2742">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2743">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2743">VM</span></span>

* <span data-ttu-id="5debd-2744">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2744">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5debd-2745">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="5debd-2745">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5debd-2746">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2746">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5debd-2747">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="5debd-2747">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5debd-2748">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="5debd-2748">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5debd-2749">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2749">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5debd-2750">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2750">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5debd-2751">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2751">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5debd-2752">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2752">December 19, 2017</span></span>

<span data-ttu-id="5debd-2753">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5debd-2753">Version 2.0.23</span></span>

* <span data-ttu-id="5debd-2754">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2754">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2755">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2755">Container</span></span>

* <span data-ttu-id="5debd-2756">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2756">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2757">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2757">Network</span></span>

* <span data-ttu-id="5debd-2758">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2758">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5debd-2759">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2759">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2760">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2760">Storage</span></span>

* <span data-ttu-id="5debd-2761">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="5debd-2761">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2762">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2762">VM</span></span>

* <span data-ttu-id="5debd-2763">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="5debd-2763">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5debd-2764">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2764">December 5, 2017</span></span>

<span data-ttu-id="5debd-2765">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5debd-2765">Version 2.0.22</span></span>

* <span data-ttu-id="5debd-2766">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2766">Removed `az component` commands.</span></span> <span data-ttu-id="5debd-2767">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2767">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2768">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2768">Core</span></span>
* <span data-ttu-id="5debd-2769">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="5debd-2769">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5debd-2770">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2770">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2771">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2771">ACS</span></span>

* <span data-ttu-id="5debd-2772">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2772">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5debd-2773">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2773">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5debd-2774">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="5debd-2774">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5debd-2775">Помощник</span><span class="sxs-lookup"><span data-stu-id="5debd-2775">Advisor</span></span>

* <span data-ttu-id="5debd-2776">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-2776">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2777">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2777">Appservice</span></span>

* <span data-ttu-id="5debd-2778">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2778">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5debd-2779">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2779">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5debd-2780">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2780">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5debd-2781">Потребление</span><span class="sxs-lookup"><span data-stu-id="5debd-2781">Consumption</span></span>

* <span data-ttu-id="5debd-2782">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="5debd-2782">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2783">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2783">Container</span></span>

* <span data-ttu-id="5debd-2784">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2784">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2785">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2785">Monitor</span></span>

* <span data-ttu-id="5debd-2786">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="5debd-2786">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2787">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2787">Resource</span></span>

* <span data-ttu-id="5debd-2788">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="5debd-2788">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5debd-2789">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-2789">Role</span></span>

* <span data-ttu-id="5debd-2790">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2790">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5debd-2791">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="5debd-2791">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5debd-2792">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2792">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2793">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2793">SQL</span></span>

* <span data-ttu-id="5debd-2794">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2794">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5debd-2795">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2795">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2796">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2796">VM</span></span>

* <span data-ttu-id="5debd-2797">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2797">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5debd-2798">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2798">November 14, 2017</span></span>

<span data-ttu-id="5debd-2799">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5debd-2799">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2800">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2800">ACR</span></span>

* <span data-ttu-id="5debd-2801">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="5debd-2801">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5debd-2802">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2802">ACS</span></span>

* <span data-ttu-id="5debd-2803">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="5debd-2803">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5debd-2804">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="5debd-2804">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5debd-2805">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2805">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5debd-2806">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-2806">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5debd-2807">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-2807">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2808">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2808">Appservice</span></span>

* <span data-ttu-id="5debd-2809">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2809">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5debd-2810">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2810">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5debd-2811">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2811">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5debd-2812">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2812">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5debd-2813">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="5debd-2813">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5debd-2814">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="5debd-2814">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2815">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2815">Batch</span></span>

* <span data-ttu-id="5debd-2816">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2816">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-2817">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5debd-2817">Batchai</span></span>

* <span data-ttu-id="5debd-2818">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2818">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5debd-2819">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2819">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5debd-2820">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2820">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5debd-2821">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2821">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5debd-2822">Cloud</span><span class="sxs-lookup"><span data-stu-id="5debd-2822">Cloud</span></span>

* <span data-ttu-id="5debd-2823">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2823">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5debd-2824">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-2824">Container</span></span>

* <span data-ttu-id="5debd-2825">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2825">Added support to open multiple ports</span></span>
* <span data-ttu-id="5debd-2826">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2826">Added container group restart policy</span></span>
* <span data-ttu-id="5debd-2827">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="5debd-2827">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5debd-2828">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="5debd-2828">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5debd-2829">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5debd-2829">Data Lake Analytics</span></span>

* <span data-ttu-id="5debd-2830">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2830">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5debd-2831">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5debd-2831">Data Lake Store</span></span>

* <span data-ttu-id="5debd-2832">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5debd-2832">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2833">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2833">Extension</span></span>

* <span data-ttu-id="5debd-2834">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5debd-2834">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5debd-2835">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="5debd-2835">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-2836">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-2836">IoT</span></span>

* <span data-ttu-id="5debd-2837">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2837">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2838">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2838">Monitor</span></span>

* <span data-ttu-id="5debd-2839">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2839">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2840">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2840">Network</span></span>

* <span data-ttu-id="5debd-2841">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="5debd-2841">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5debd-2842">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2842">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5debd-2843">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5debd-2843">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5debd-2844">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2844">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5debd-2845">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2845">Reservations</span></span>

* <span data-ttu-id="5debd-2846">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="5debd-2846">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2847">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2847">Resource</span></span>

* <span data-ttu-id="5debd-2848">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2848">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2849">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2849">SQL</span></span>

* <span data-ttu-id="5debd-2850">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2850">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2851">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2851">Storage</span></span>

* <span data-ttu-id="5debd-2852">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2852">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5debd-2853">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="5debd-2853">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5debd-2854">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2854">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5debd-2855">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2855">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5debd-2856">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2856">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5debd-2857">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2857">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5debd-2858">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2858">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2859">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2859">VM</span></span>

* <span data-ttu-id="5debd-2860">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2860">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5debd-2861">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2861">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5debd-2862">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2862">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5debd-2863">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="5debd-2863">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5debd-2864">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5debd-2864">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5debd-2865">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2865">October 24, 2017</span></span>

<span data-ttu-id="5debd-2866">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5debd-2866">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2867">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2867">Core</span></span>

* <span data-ttu-id="5debd-2868">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="5debd-2868">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-2869">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-2869">ACR</span></span>

* <span data-ttu-id="5debd-2870">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="5debd-2870">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5debd-2871">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="5debd-2871">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5debd-2872">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="5debd-2872">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2873">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2873">ACS</span></span>

* <span data-ttu-id="5debd-2874">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="5debd-2874">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5debd-2875">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="5debd-2875">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2876">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2876">Appservice</span></span>

* <span data-ttu-id="5debd-2877">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="5debd-2877">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5debd-2878">Компонент</span><span class="sxs-lookup"><span data-stu-id="5debd-2878">Component</span></span>

* <span data-ttu-id="5debd-2879">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="5debd-2879">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-2880">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-2880">Monitor</span></span>

* <span data-ttu-id="5debd-2881">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2881">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2882">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2882">Resource</span></span>

* <span data-ttu-id="5debd-2883">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="5debd-2883">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5debd-2884">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="5debd-2884">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2885">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2885">VM</span></span>

* <span data-ttu-id="5debd-2886">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2886">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5debd-2887">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2887">October 9, 2017</span></span>

<span data-ttu-id="5debd-2888">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5debd-2888">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2889">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2889">Core</span></span>

* <span data-ttu-id="5debd-2890">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="5debd-2890">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2891">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2891">Appservice</span></span>

* <span data-ttu-id="5debd-2892">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2892">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-2893">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-2893">Batch</span></span>

* <span data-ttu-id="5debd-2894">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5debd-2894">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5debd-2895">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="5debd-2895">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5debd-2896">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2896">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5debd-2897">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2897">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5debd-2898">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5debd-2898">Batchai</span></span>

* <span data-ttu-id="5debd-2899">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5debd-2899">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-2900">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-2900">Keyvault</span></span>

* <span data-ttu-id="5debd-2901">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5debd-2901">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5debd-2902">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5debd-2902">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5debd-2903">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2903">Network</span></span>

* <span data-ttu-id="5debd-2904">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="5debd-2904">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5debd-2905">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="5debd-2905">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2906">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2906">Resource</span></span>

* <span data-ttu-id="5debd-2907">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2907">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5debd-2908">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5debd-2908">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5debd-2909">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="5debd-2909">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5debd-2910">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="5debd-2910">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2911">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2911">Sql</span></span>

* <span data-ttu-id="5debd-2912">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="5debd-2912">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5debd-2913">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-2913">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5debd-2914">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-2914">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2915">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2915">Storage</span></span>

* <span data-ttu-id="5debd-2916">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2916">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2917">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="5debd-2917">Vm</span></span>

* <span data-ttu-id="5debd-2918">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5debd-2918">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5debd-2919">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2919">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5debd-2920">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2920">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5debd-2921">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2921">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5debd-2922">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="5debd-2922">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5debd-2923">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2923">September 22, 2017</span></span>

<span data-ttu-id="5debd-2924">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5debd-2924">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2925">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2925">Resource</span></span>

* <span data-ttu-id="5debd-2926">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="5debd-2926">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5debd-2927">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="5debd-2927">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5debd-2928">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2928">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5debd-2929">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2929">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2930">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2930">Network</span></span>

* <span data-ttu-id="5debd-2931">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5debd-2931">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5debd-2932">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="5debd-2932">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5debd-2933">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="5debd-2933">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5debd-2934">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2934">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5debd-2935">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2935">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5debd-2936">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2936">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5debd-2937">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2937">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-2938">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-2938">Storage</span></span>

* <span data-ttu-id="5debd-2939">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="5debd-2939">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5debd-2940">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5debd-2940">Eventgrid</span></span>

* <span data-ttu-id="5debd-2941">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="5debd-2941">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2942">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2942">SQL</span></span>

* <span data-ttu-id="5debd-2943">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="5debd-2943">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5debd-2944">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="5debd-2944">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5debd-2945">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2945">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-2946">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-2946">Keyvault</span></span>

* <span data-ttu-id="5debd-2947">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="5debd-2947">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2948">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2948">VM</span></span>

* <span data-ttu-id="5debd-2949">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2949">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5debd-2950">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="5debd-2950">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5debd-2951">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="5debd-2951">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5debd-2952">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5debd-2952">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5debd-2953">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5debd-2953">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5debd-2954">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5debd-2954">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2955">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2955">ACS</span></span>

* <span data-ttu-id="5debd-2956">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5debd-2956">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2957">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2957">Appservice</span></span>

* <span data-ttu-id="5debd-2958">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5debd-2958">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5debd-2959">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5debd-2959">Backup</span></span>

* <span data-ttu-id="5debd-2960">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5debd-2960">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5debd-2961">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2961">September 11, 2017</span></span>

<span data-ttu-id="5debd-2962">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5debd-2962">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5debd-2963">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-2963">Core</span></span>

* <span data-ttu-id="5debd-2964">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5debd-2964">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5debd-2965">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="5debd-2965">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-2966">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-2966">Acs</span></span>

* <span data-ttu-id="5debd-2967">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2967">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5debd-2968">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-2968">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-2969">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-2969">Appservice</span></span>

* <span data-ttu-id="5debd-2970">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="5debd-2970">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-2971">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-2971">CDN</span></span>

* <span data-ttu-id="5debd-2972">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2972">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5debd-2973">Расширение</span><span class="sxs-lookup"><span data-stu-id="5debd-2973">Extension</span></span>

* <span data-ttu-id="5debd-2974">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-2974">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-2975">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-2975">Keyvault</span></span>

* <span data-ttu-id="5debd-2976">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2976">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-2977">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-2977">Network</span></span>

* <span data-ttu-id="5debd-2978">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5debd-2978">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5debd-2979">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2979">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5debd-2980">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2980">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5debd-2981">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2981">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5debd-2982">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2982">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-2983">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-2983">Resource</span></span>

* <span data-ttu-id="5debd-2984">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2984">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5debd-2985">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2985">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5debd-2986">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="5debd-2986">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5debd-2987">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="5debd-2987">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-2988">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-2988">SQL</span></span>

* <span data-ttu-id="5debd-2989">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2989">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-2990">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-2990">VM</span></span>

* <span data-ttu-id="5debd-2991">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5debd-2991">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5debd-2992">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="5debd-2992">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5debd-2993">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2993">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5debd-2994">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="5debd-2994">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5debd-2995">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="5debd-2995">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5debd-2996">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-2996">August 31, 2017</span></span>

<span data-ttu-id="5debd-2997">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5debd-2997">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-2998">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-2998">Keyvault</span></span>

* <span data-ttu-id="5debd-2999">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="5debd-2999">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5debd-3000">Sf</span><span class="sxs-lookup"><span data-stu-id="5debd-3000">Sf</span></span>

* <span data-ttu-id="5debd-3001">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="5debd-3001">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-3002">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3002">Storage</span></span>

* <span data-ttu-id="5debd-3003">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="5debd-3003">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5debd-3004">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="5debd-3004">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5debd-3005">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3005">August 28, 2017</span></span>

<span data-ttu-id="5debd-3006">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5debd-3006">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5debd-3007">CLI</span><span class="sxs-lookup"><span data-stu-id="5debd-3007">CLI</span></span>

* <span data-ttu-id="5debd-3008">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="5debd-3008">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3009">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3009">ACS</span></span>

* <span data-ttu-id="5debd-3010">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5debd-3010">Corrected preview regions</span></span>
* <span data-ttu-id="5debd-3011">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3011">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5debd-3012">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="5debd-3012">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-3013">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-3013">Appservice</span></span>

* <span data-ttu-id="5debd-3014">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3014">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5debd-3015">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3015">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5debd-3016">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3016">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5debd-3017">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="5debd-3017">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5debd-3018">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="5debd-3018">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-3019">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-3019">IoT</span></span>

* <span data-ttu-id="5debd-3020">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="5debd-3020">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5debd-3021">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-3021">Network</span></span>

* <span data-ttu-id="5debd-3022">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3022">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5debd-3023">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3023">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5debd-3024">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3024">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5debd-3025">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3025">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5debd-3026">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3026">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-3027">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-3027">Profile</span></span>

* <span data-ttu-id="5debd-3028">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5debd-3028">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5debd-3029">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-3029">Service Fabric</span></span>

* <span data-ttu-id="5debd-3030">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5debd-3030">Preview release</span></span>
* <span data-ttu-id="5debd-3031">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-3031">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5debd-3032">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="5debd-3032">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5debd-3033">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3033">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-3034">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3034">Storage</span></span>

* <span data-ttu-id="5debd-3035">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5debd-3035">Enabled setting blob tier</span></span>
* <span data-ttu-id="5debd-3036">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-3036">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5debd-3037">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3037">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5debd-3038">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="5debd-3038">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5debd-3039">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3039">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5debd-3040">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3040">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-3041">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-3041">VM</span></span>

* <span data-ttu-id="5debd-3042">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3042">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5debd-3043">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3043">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5debd-3044">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="5debd-3044">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5debd-3045">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="5debd-3045">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5debd-3046">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5debd-3046">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5debd-3047">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3047">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5debd-3048">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3048">August 15, 2017</span></span>

<span data-ttu-id="5debd-3049">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5debd-3049">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3050">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3050">ACS</span></span>

* <span data-ttu-id="5debd-3051">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5debd-3051">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-3052">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-3052">Appservice</span></span>

* <span data-ttu-id="5debd-3053">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="5debd-3053">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5debd-3054">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-3054">Event Grid</span></span>

* <span data-ttu-id="5debd-3055">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5debd-3055">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5debd-3056">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3056">August 11, 2017</span></span>

<span data-ttu-id="5debd-3057">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5debd-3057">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3058">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3058">ACS</span></span>

* <span data-ttu-id="5debd-3059">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5debd-3059">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-3060">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-3060">Batch</span></span>

* <span data-ttu-id="5debd-3061">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="5debd-3061">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5debd-3062">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="5debd-3062">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5debd-3063">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-3063">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5debd-3064">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="5debd-3064">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5debd-3065">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="5debd-3065">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5debd-3066">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3066">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5debd-3067">Компонент</span><span class="sxs-lookup"><span data-stu-id="5debd-3067">Component</span></span>

* <span data-ttu-id="5debd-3068">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="5debd-3068">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5debd-3069">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5debd-3069">Container</span></span>

* <span data-ttu-id="5debd-3070">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="5debd-3070">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5debd-3071">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5debd-3071">Data Lake Store</span></span>

* <span data-ttu-id="5debd-3072">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="5debd-3072">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5debd-3073">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-3073">Event Grid</span></span>

* <span data-ttu-id="5debd-3074">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5debd-3074">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5debd-3075">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-3075">Network</span></span>

* <span data-ttu-id="5debd-3076">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="5debd-3076">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5debd-3077">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3077">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5debd-3078">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3078">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5debd-3079">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3079">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-3080">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-3080">Profile</span></span>

* <span data-ttu-id="5debd-3081">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="5debd-3081">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-3082">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3082">Storage</span></span>

* <span data-ttu-id="5debd-3083">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5debd-3083">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-3084">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-3084">VM</span></span>

* <span data-ttu-id="5debd-3085">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="5debd-3085">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5debd-3086">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3086">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5debd-3087">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="5debd-3087">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5debd-3088">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="5debd-3088">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5debd-3089">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5debd-3089">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5debd-3090">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3090">July 28, 2017</span></span>

<span data-ttu-id="5debd-3091">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5debd-3091">Version 2.0.12</span></span>

* <span data-ttu-id="5debd-3092">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5debd-3092">Added container commands</span></span>
* <span data-ttu-id="5debd-3093">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5debd-3093">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5debd-3094">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-3094">Core</span></span>

* <span data-ttu-id="5debd-3095">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5debd-3095">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5debd-3096">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="5debd-3096">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5debd-3097">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5debd-3097">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5debd-3098">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="5debd-3098">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5debd-3099">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="5debd-3099">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5debd-3100">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="5debd-3100">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5debd-3101">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5debd-3101">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5debd-3102">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="5debd-3102">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5debd-3103">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="5debd-3103">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5debd-3104">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="5debd-3104">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5debd-3105">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="5debd-3105">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5debd-3106">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="5debd-3106">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5debd-3107">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-3107">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5debd-3108">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5debd-3108">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5debd-3109">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5debd-3109">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5debd-3110">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="5debd-3110">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5debd-3111">ACR</span><span class="sxs-lookup"><span data-stu-id="5debd-3111">ACR</span></span>

* <span data-ttu-id="5debd-3112">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5debd-3112">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5debd-3113">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5debd-3113">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5debd-3114">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="5debd-3114">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5debd-3115">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="5debd-3115">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5debd-3116">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="5debd-3116">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5debd-3117">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="5debd-3117">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3118">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3118">ACS</span></span>

* <span data-ttu-id="5debd-3119">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="5debd-3119">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-3120">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5debd-3120">Appservice</span></span>

* <span data-ttu-id="5debd-3121">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="5debd-3121">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5debd-3122">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="5debd-3122">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5debd-3123">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3123">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5debd-3124">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="5debd-3124">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5debd-3125">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="5debd-3125">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5debd-3126">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="5debd-3126">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5debd-3127">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="5debd-3127">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5debd-3128">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="5debd-3128">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5debd-3129">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="5debd-3129">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5debd-3130">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3130">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5debd-3131">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5debd-3131">Batch</span></span>

* <span data-ttu-id="5debd-3132">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="5debd-3132">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5debd-3133">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3133">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5debd-3134">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3134">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5debd-3135">CDN</span><span class="sxs-lookup"><span data-stu-id="5debd-3135">CDN</span></span>

* <span data-ttu-id="5debd-3136">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-3136">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5debd-3137">Cloud</span><span class="sxs-lookup"><span data-stu-id="5debd-3137">Cloud</span></span>

* <span data-ttu-id="5debd-3138">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5debd-3138">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5debd-3139">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="5debd-3139">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5debd-3140">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="5debd-3140">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5debd-3141">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5debd-3141">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5debd-3142">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3142">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-3143">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-3143">CosmosDB</span></span>

* <span data-ttu-id="5debd-3144">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="5debd-3144">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5debd-3145">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="5debd-3145">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5debd-3146">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5debd-3146">Data Lake Analytics</span></span>

* <span data-ttu-id="5debd-3147">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3147">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5debd-3148">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3148">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5debd-3149">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3149">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5debd-3150">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5debd-3150">Data Lake Store</span></span>

* <span data-ttu-id="5debd-3151">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3151">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5debd-3152">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="5debd-3152">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5debd-3153">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3153">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5debd-3154">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5debd-3154">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5debd-3155">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5debd-3155">Interactive</span></span>

* <span data-ttu-id="5debd-3156">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="5debd-3156">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5debd-3157">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="5debd-3157">Increased test coverage</span></span>
* <span data-ttu-id="5debd-3158">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="5debd-3158">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5debd-3159">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="5debd-3159">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5debd-3160">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="5debd-3160">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5debd-3161">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="5debd-3161">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5debd-3162">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5debd-3162">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5debd-3163">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3163">Added `--progress` flag</span></span>
* <span data-ttu-id="5debd-3164">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3164">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5debd-3165">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="5debd-3165">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5debd-3166">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5debd-3166">IoT</span></span>

* <span data-ttu-id="5debd-3167">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="5debd-3167">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5debd-3168">(3934).</span><span class="sxs-lookup"><span data-stu-id="5debd-3168">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5debd-3169">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-3169">Key vault</span></span>

* <span data-ttu-id="5debd-3170">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="5debd-3170">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5debd-3171">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3171">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5debd-3172">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="5debd-3172">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5debd-3173">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3173">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5debd-3174">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3174">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5debd-3175">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="5debd-3175">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5debd-3176">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="5debd-3176">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5debd-3177">(3307).</span><span class="sxs-lookup"><span data-stu-id="5debd-3177">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5debd-3178">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5debd-3178">Lab</span></span>

* <span data-ttu-id="5debd-3179">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3179">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5debd-3180">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3180">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-3181">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-3181">Monitor</span></span>

* <span data-ttu-id="5debd-3182">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="5debd-3182">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5debd-3183">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="5debd-3183">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5debd-3184">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="5debd-3184">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5debd-3185">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="5debd-3185">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5debd-3186">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="5debd-3186">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5debd-3187">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="5debd-3187">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5debd-3188">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="5debd-3188">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5debd-3189">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="5debd-3189">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5debd-3190">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5debd-3190">`location` no longer required</span></span>
  * <span data-ttu-id="5debd-3191">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="5debd-3191">Add name and ID support for target</span></span>
  * <span data-ttu-id="5debd-3192">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="5debd-3192">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5debd-3193">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5debd-3193">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5debd-3194">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="5debd-3194">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5debd-3195">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="5debd-3195">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5debd-3196">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3196">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5debd-3197">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3197">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5debd-3198">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-3198">Network</span></span>

* <span data-ttu-id="5debd-3199">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3199">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5debd-3200">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3200">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5debd-3201">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5debd-3201">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5debd-3202">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3202">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5debd-3203">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3203">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5debd-3204">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3204">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5debd-3205">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3205">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5debd-3206">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3206">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5debd-3207">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3207">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5debd-3208">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3208">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5debd-3209">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3209">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5debd-3210">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3210">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5debd-3211">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3211">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5debd-3212">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3212">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5debd-3213">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3213">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5debd-3214">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3214">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5debd-3215">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="5debd-3215">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5debd-3216">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3216">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5debd-3217">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3217">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5debd-3218">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3218">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5debd-3219">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3219">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5debd-3220">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3220">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5debd-3221">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3221">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5debd-3222">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-3222">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5debd-3223">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-3223">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5debd-3224">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5debd-3224">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5debd-3225">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-3225">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-3226">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-3226">Profile</span></span>

* <span data-ttu-id="5debd-3227">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5debd-3227">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5debd-3228">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5debd-3228">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5debd-3229">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5debd-3229">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5debd-3230">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="5debd-3230">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5debd-3231">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="5debd-3231">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5debd-3232">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5debd-3232">RDBMS</span></span>

* <span data-ttu-id="5debd-3233">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="5debd-3233">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5debd-3234">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="5debd-3234">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5debd-3235">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="5debd-3235">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5debd-3236">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="5debd-3236">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-3237">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-3237">Resource</span></span>

* <span data-ttu-id="5debd-3238">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3238">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5debd-3239">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3239">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5debd-3240">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3240">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5debd-3241">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3241">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5debd-3242">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="5debd-3242">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5debd-3243">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3243">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5debd-3244">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="5debd-3244">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5debd-3245">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3245">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5debd-3246">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-3246">Role</span></span>

* <span data-ttu-id="5debd-3247">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5debd-3247">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5debd-3248">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="5debd-3248">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5debd-3249">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="5debd-3249">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5debd-3250">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5debd-3250">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5debd-3251">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3251">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5debd-3252">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5debd-3252">Service Fabric</span></span>
* <span data-ttu-id="5debd-3253">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="5debd-3253">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5debd-3254">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="5debd-3254">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5debd-3255">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="5debd-3255">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-3256">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-3256">SQL</span></span>

* <span data-ttu-id="5debd-3257">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3257">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5debd-3258">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3258">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5debd-3259">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3259">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-3260">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3260">Storage</span></span>

* <span data-ttu-id="5debd-3261">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="5debd-3261">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5debd-3262">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5debd-3262">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5debd-3263">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="5debd-3263">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5debd-3264">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="5debd-3264">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5debd-3265">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="5debd-3265">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5debd-3266">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="5debd-3266">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-3267">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-3267">VM</span></span>

* <span data-ttu-id="5debd-3268">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="5debd-3268">Support configuring nsg</span></span>
* <span data-ttu-id="5debd-3269">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="5debd-3269">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5debd-3270">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5debd-3270">Support managed service identities</span></span>
* <span data-ttu-id="5debd-3271">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3271">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5debd-3272">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="5debd-3272">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5debd-3273">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3273">May 10, 2017</span></span>

<span data-ttu-id="5debd-3274">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5debd-3274">Version 2.0.6</span></span>

* <span data-ttu-id="5debd-3275">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5debd-3275">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5debd-3276">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="5debd-3276">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5debd-3277">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-3277">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5debd-3278">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5debd-3278">Include Cognitive Services module</span></span>
* <span data-ttu-id="5debd-3279">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="5debd-3279">Include Service Fabric module</span></span>
* <span data-ttu-id="5debd-3280">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="5debd-3280">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5debd-3281">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="5debd-3281">Add support for CDN commands</span></span>
* <span data-ttu-id="5debd-3282">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="5debd-3282">Remove Container module</span></span>
* <span data-ttu-id="5debd-3283">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3283">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5debd-3284">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3284">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5debd-3285">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-3285">Core</span></span>

* <span data-ttu-id="5debd-3286">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="5debd-3286">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5debd-3287">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3287">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5debd-3288">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3288">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5debd-3289">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3289">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5debd-3290">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3290">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5debd-3291">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3291">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5debd-3292">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3292">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5debd-3293">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3293">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5debd-3294">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3294">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5debd-3295">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="5debd-3295">core: Improved performance</span></span>
* <span data-ttu-id="5debd-3296">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="5debd-3296">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5debd-3297">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="5debd-3297">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3298">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3298">ACS</span></span>

* <span data-ttu-id="5debd-3299">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="5debd-3299">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5debd-3300">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="5debd-3300">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5debd-3301">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="5debd-3301">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5debd-3302">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3302">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-3303">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-3303">AppService</span></span>

* <span data-ttu-id="5debd-3304">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="5debd-3304">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5debd-3305">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3305">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5debd-3306">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="5debd-3306">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5debd-3307">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5debd-3307">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5debd-3308">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="5debd-3308">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5debd-3309">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3309">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5debd-3310">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="5debd-3310">support slot swap with preview</span></span>
* <span data-ttu-id="5debd-3311">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3311">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5debd-3312">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3312">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5debd-3313">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5debd-3313">CosmosDB</span></span>

* <span data-ttu-id="5debd-3314">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5debd-3314">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5debd-3315">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="5debd-3315">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5debd-3316">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="5debd-3316">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5debd-3317">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="5debd-3317">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5debd-3318">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5debd-3318">Data Lake Analytics</span></span>

* <span data-ttu-id="5debd-3319">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="5debd-3319">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5debd-3320">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="5debd-3320">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5debd-3321">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3321">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5debd-3322">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="5debd-3322">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5debd-3323">Таблица</span><span class="sxs-lookup"><span data-stu-id="5debd-3323">Table</span></span>
  * <span data-ttu-id="5debd-3324">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="5debd-3324">Table valued function</span></span>
  * <span data-ttu-id="5debd-3325">Представление</span><span class="sxs-lookup"><span data-stu-id="5debd-3325">View</span></span>
  * <span data-ttu-id="5debd-3326">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="5debd-3326">Table Statistics.</span></span> <span data-ttu-id="5debd-3327">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="5debd-3327">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5debd-3328">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5debd-3328">Data Lake Store</span></span>

* <span data-ttu-id="5debd-3329">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="5debd-3329">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5debd-3330">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3330">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5debd-3331">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="5debd-3331">missed help for access show.</span></span> <span data-ttu-id="5debd-3332">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="5debd-3332">adding it.</span></span> <span data-ttu-id="5debd-3333">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5debd-3333">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5debd-3334">Поиск</span><span class="sxs-lookup"><span data-stu-id="5debd-3334">Find</span></span>

* <span data-ttu-id="5debd-3335">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="5debd-3335">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5debd-3336">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5debd-3336">KeyVault</span></span>

* <span data-ttu-id="5debd-3337">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="5debd-3337">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5debd-3338">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="5debd-3338">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5debd-3339">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="5debd-3339">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5debd-3340">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="5debd-3340">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5debd-3341">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3341">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5debd-3342">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5debd-3342">Lab</span></span>

* <span data-ttu-id="5debd-3343">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5debd-3343">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5debd-3344">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5debd-3344">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5debd-3345">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5debd-3345">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5debd-3346">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5debd-3346">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5debd-3347">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5debd-3347">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5debd-3348">Монитор</span><span class="sxs-lookup"><span data-stu-id="5debd-3348">Monitor</span></span>

* <span data-ttu-id="5debd-3349">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3349">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5debd-3350">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3350">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5debd-3351">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-3351">Network</span></span>

* <span data-ttu-id="5debd-3352">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3352">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5debd-3353">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3353">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5debd-3354">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3354">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5debd-3355">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3355">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5debd-3356">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5debd-3356">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5debd-3357">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="5debd-3357">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5debd-3358">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3358">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5debd-3359">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5debd-3359">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5debd-3360">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3360">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5debd-3361">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="5debd-3361">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5debd-3362">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3362">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5debd-3363">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3363">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5debd-3364">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="5debd-3364">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5debd-3365">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="5debd-3365">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5debd-3366">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="5debd-3366">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5debd-3367">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="5debd-3367">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5debd-3368">Профиль</span><span class="sxs-lookup"><span data-stu-id="5debd-3368">Profile</span></span>

* <span data-ttu-id="5debd-3369">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3369">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5debd-3370">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3370">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5debd-3371">Redis</span><span class="sxs-lookup"><span data-stu-id="5debd-3371">Redis</span></span>

* <span data-ttu-id="5debd-3372">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="5debd-3372">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5debd-3373">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="5debd-3373">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5debd-3374">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5debd-3374">Resource</span></span>

* <span data-ttu-id="5debd-3375">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3375">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5debd-3376">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3376">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5debd-3377">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3377">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5debd-3378">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="5debd-3378">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5debd-3379">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5debd-3379">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5debd-3380">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="5debd-3380">Add docs for az lock update.</span></span> <span data-ttu-id="5debd-3381">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5debd-3381">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5debd-3382">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="5debd-3382">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5debd-3383">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5debd-3383">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5debd-3384">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5debd-3384">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5debd-3385">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5debd-3385">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5debd-3386">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3386">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5debd-3387">Роль</span><span class="sxs-lookup"><span data-stu-id="5debd-3387">Role</span></span>

* <span data-ttu-id="5debd-3388">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3388">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5debd-3389">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3389">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5debd-3390">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3390">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5debd-3391">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="5debd-3391">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5debd-3392">SQL</span><span class="sxs-lookup"><span data-stu-id="5debd-3392">SQL</span></span>

* <span data-ttu-id="5debd-3393">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="5debd-3393">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5debd-3394">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3394">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5debd-3395">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3395">Storage</span></span>

* <span data-ttu-id="5debd-3396">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3396">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5debd-3397">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-3397">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5debd-3398">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5debd-3398">Add support for large block blob upload</span></span>
* <span data-ttu-id="5debd-3399">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5debd-3399">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-3400">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-3400">VM</span></span>

* <span data-ttu-id="5debd-3401">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="5debd-3401">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5debd-3402">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="5debd-3402">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5debd-3403">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5debd-3403">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5debd-3404">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5debd-3404">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5debd-3405">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="5debd-3405">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5debd-3406">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="5debd-3406">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5debd-3407">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3407">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5debd-3408">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3408">April 3, 2017</span></span>

<span data-ttu-id="5debd-3409">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5debd-3409">Version 2.0.2</span></span>

<span data-ttu-id="5debd-3410">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="5debd-3410">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5debd-3411">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5debd-3411">Core</span></span>

* <span data-ttu-id="5debd-3412">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-3412">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5debd-3413">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3413">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5debd-3414">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3414">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5debd-3415">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3415">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5debd-3416">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3416">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5debd-3417">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="5debd-3417">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5debd-3418">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3418">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5debd-3419">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5debd-3419">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5debd-3420">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="5debd-3420">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5debd-3421">ACS</span><span class="sxs-lookup"><span data-stu-id="5debd-3421">ACS</span></span>

* <span data-ttu-id="5debd-3422">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3422">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5debd-3423">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="5debd-3423">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5debd-3424">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3424">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5debd-3425">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="5debd-3425">Add support for windows clusters.</span></span> <span data-ttu-id="5debd-3426">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3426">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5debd-3427">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="5debd-3427">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5debd-3428">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3428">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5debd-3429">AppService</span><span class="sxs-lookup"><span data-stu-id="5debd-3429">AppService</span></span>

* <span data-ttu-id="5debd-3430">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3430">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5debd-3431">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3431">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5debd-3432">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3432">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5debd-3433">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3433">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5debd-3434">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5debd-3434">DataLake</span></span>

* <span data-ttu-id="5debd-3435">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5debd-3435">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5debd-3436">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5debd-3436">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5debd-3437">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="5debd-3437">DocuemntDB</span></span>

* <span data-ttu-id="5debd-3438">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3438">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5debd-3439">ВМ</span><span class="sxs-lookup"><span data-stu-id="5debd-3439">VM</span></span>

* <span data-ttu-id="5debd-3440">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3440">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5debd-3441">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3441">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5debd-3442">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3442">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5debd-3443">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3443">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5debd-3444">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3444">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5debd-3445">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3445">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="5debd-3446">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="5debd-3446">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5debd-3447">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5debd-3447">February 27, 2017</span></span>

<span data-ttu-id="5debd-3448">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5debd-3448">Version 2.0.0</span></span>

<span data-ttu-id="5debd-3449">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="5debd-3449">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5debd-3450">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="5debd-3450">Container Service (acs)</span></span>
- <span data-ttu-id="5debd-3451">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="5debd-3451">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5debd-3452">Сеть</span><span class="sxs-lookup"><span data-stu-id="5debd-3452">Networking</span></span>
- <span data-ttu-id="5debd-3453">Память</span><span class="sxs-lookup"><span data-stu-id="5debd-3453">Storage</span></span>

<span data-ttu-id="5debd-3454">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3454">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5debd-3455">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="5debd-3455">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5debd-3456">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="5debd-3456">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5debd-3457">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="5debd-3457">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5debd-3458">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5debd-3458">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5debd-3459">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="5debd-3459">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5debd-3460">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="5debd-3460">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5debd-3461">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="5debd-3461">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5debd-3462">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5debd-3462">Provide feedback from the command line with the `az feedback` command</span></span>
