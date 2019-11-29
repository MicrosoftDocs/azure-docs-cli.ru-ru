---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 75a3a3ee800edc20bd1c8ed7ab1ff542f5935c6c
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543465"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="4ee15-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4ee15-103">Azure CLI release notes</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="4ee15-104">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-104">November 26, 2019</span></span>

<span data-ttu-id="4ee15-105">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="4ee15-105">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-106">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-106">ACR</span></span>

* <span data-ttu-id="4ee15-107">Устарел флаг `--branch` параметра, используемый при обновлении или создании задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-107">Deprecated paramater `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="4ee15-108">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="4ee15-108">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="4ee15-109">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-109">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="4ee15-110">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-110">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-111">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-111">AKS</span></span>

* <span data-ttu-id="4ee15-112">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="4ee15-112">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="4ee15-113">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4ee15-113">AppConfig</span></span>

* <span data-ttu-id="4ee15-114">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-114">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="4ee15-115">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-115">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="4ee15-116">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-116">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="4ee15-117">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-117">AppService</span></span>

* <span data-ttu-id="4ee15-118">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-118">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="4ee15-119">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="4ee15-119">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="4ee15-120">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="4ee15-120">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-121">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-121">Backup</span></span>

* <span data-ttu-id="4ee15-122">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="4ee15-122">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="4ee15-123">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="4ee15-123">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-124">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-124">Compute</span></span>

* <span data-ttu-id="4ee15-125">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-125">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="4ee15-126">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="4ee15-126">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="4ee15-127">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="4ee15-127">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="4ee15-128">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="4ee15-128">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="4ee15-129">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="4ee15-129">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="4ee15-130">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-130">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="4ee15-131">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-131">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="4ee15-132">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="4ee15-132">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="4ee15-133">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-133">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="4ee15-134">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-134">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-135">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-135">IOT</span></span>

* <span data-ttu-id="4ee15-136">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="4ee15-136">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="4ee15-137">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-137">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="4ee15-138">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-138">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-139">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-139">Key Vault</span></span>

* <span data-ttu-id="4ee15-140">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-140">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4ee15-141">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4ee15-141">NetAppFiles</span></span>

* <span data-ttu-id="4ee15-142">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-142">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-143">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-143">Network</span></span>

* <span data-ttu-id="4ee15-144">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="4ee15-144">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="4ee15-145">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-145">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="4ee15-146">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="4ee15-146">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="4ee15-147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="4ee15-147">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="4ee15-148">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-148">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="4ee15-149">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-149">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="4ee15-150">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4ee15-150">Packaging</span></span>

* <span data-ttu-id="4ee15-151">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="4ee15-151">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="4ee15-152">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="4ee15-152">Added support for Python 3.8</span></span>
* <span data-ttu-id="4ee15-153">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="4ee15-153">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-154">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-154">Profile</span></span>

* <span data-ttu-id="4ee15-155">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4ee15-155">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="4ee15-156">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-156">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="4ee15-157">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-157">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="4ee15-158">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-158">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="4ee15-159">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-159">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-160">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-160">RBAC</span></span>

* <span data-ttu-id="4ee15-161">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-161">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="4ee15-162">Redis</span><span class="sxs-lookup"><span data-stu-id="4ee15-162">Redis</span></span>

* <span data-ttu-id="4ee15-163">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="4ee15-163">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="4ee15-164">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4ee15-164">Reservations</span></span>

* <span data-ttu-id="4ee15-165">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="4ee15-165">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="4ee15-166">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="4ee15-166">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="4ee15-167">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-167">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="4ee15-168">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-168">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="4ee15-169">Rest</span><span class="sxs-lookup"><span data-stu-id="4ee15-169">Rest</span></span>
* <span data-ttu-id="4ee15-170">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="4ee15-170">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-171">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-171">SQL</span></span>

* <span data-ttu-id="4ee15-172">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-172">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-173">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-173">Storage</span></span>

* <span data-ttu-id="4ee15-174">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-174">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="4ee15-175">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ee15-175">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="4ee15-176">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="4ee15-176">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="4ee15-177">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="4ee15-177">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="4ee15-178">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-178">November 4, 2019</span></span>

<span data-ttu-id="4ee15-179">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="4ee15-179">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-180">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-180">ACR</span></span>

* <span data-ttu-id="4ee15-181">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-181">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="4ee15-182">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-182">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="4ee15-183">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-183">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-184">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-184">AKS</span></span>

* <span data-ttu-id="4ee15-185">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-185">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="4ee15-186">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-186">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="4ee15-187">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4ee15-187">AppConfig</span></span>

* <span data-ttu-id="4ee15-188">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-188">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="4ee15-189">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="4ee15-189">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="4ee15-190">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-190">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-191">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-191">AppService</span></span>

* <span data-ttu-id="4ee15-192">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="4ee15-192">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="4ee15-193">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-193">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="4ee15-194">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="4ee15-194">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="4ee15-195">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="4ee15-195">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="4ee15-196">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-196">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="4ee15-197">ARM</span><span class="sxs-lookup"><span data-stu-id="4ee15-197">ARM</span></span>

* <span data-ttu-id="4ee15-198">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-198">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="4ee15-199">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-199">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-200">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-200">Backup</span></span>

* <span data-ttu-id="4ee15-201">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="4ee15-201">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-202">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-202">Compute</span></span>

* <span data-ttu-id="4ee15-203">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="4ee15-203">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="4ee15-204">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="4ee15-204">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="4ee15-205">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="4ee15-205">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="4ee15-206">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="4ee15-206">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="4ee15-207">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="4ee15-207">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="4ee15-208">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set` Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-208">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="4ee15-209">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4ee15-209">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="4ee15-210">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="4ee15-210">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-211">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-211">CosmosDB</span></span>

* <span data-ttu-id="4ee15-212">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create` `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-212">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="4ee15-213">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create` `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-213">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="4ee15-214">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-214">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="4ee15-215">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-215">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="4ee15-216">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-216">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="4ee15-217">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-217">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="4ee15-218">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="4ee15-218">Fixed typo in help message</span></span>
* <span data-ttu-id="4ee15-219">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-219">database: Added deprecation infomation</span></span>
* <span data-ttu-id="4ee15-220">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-220">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-221">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-221">IoT</span></span>

* <span data-ttu-id="4ee15-222">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="4ee15-222">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="4ee15-223">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-223">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-224">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-224">Key Vault</span></span>

* <span data-ttu-id="4ee15-225">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="4ee15-225">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="4ee15-226">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-226">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4ee15-227">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4ee15-227">NetAppFiles</span></span>

* <span data-ttu-id="4ee15-228">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-228">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="4ee15-229">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="4ee15-229">This new API version includes:</span></span>

    - <span data-ttu-id="4ee15-230">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="4ee15-230">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="4ee15-231">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="4ee15-231">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="4ee15-232">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-232">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="4ee15-233">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="4ee15-233">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-234">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-234">Network</span></span>

* <span data-ttu-id="4ee15-235">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-235">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="4ee15-236">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="4ee15-236">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="4ee15-237">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-237">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="4ee15-238">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-238">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="4ee15-239">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-239">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="4ee15-240">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-240">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-241">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-241">Profile</span></span>

* <span data-ttu-id="4ee15-242">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-242">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="4ee15-243">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-243">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-244">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-244">RBAC</span></span>

* <span data-ttu-id="4ee15-245">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="4ee15-245">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4ee15-246">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-246">ServiceFabric</span></span>

* <span data-ttu-id="4ee15-247">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-247">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-248">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-248">SQL</span></span>

* <span data-ttu-id="4ee15-249">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-249">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-250">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-250">Storage</span></span>

* <span data-ttu-id="4ee15-251">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-251">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="4ee15-252">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-252">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="4ee15-253">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-253">October 15, 2019</span></span>

<span data-ttu-id="4ee15-254">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="4ee15-254">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-255">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-255">AKS</span></span>

* <span data-ttu-id="4ee15-256">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-256">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="4ee15-257">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-257">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-258">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-258">AMS</span></span>

* <span data-ttu-id="4ee15-259">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-259">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="4ee15-260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-260">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-261">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-261">AppService</span></span>

* <span data-ttu-id="4ee15-262">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-262">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="4ee15-263">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-263">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="4ee15-264">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-264">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="4ee15-265">ARM</span><span class="sxs-lookup"><span data-stu-id="4ee15-265">ARM</span></span>

* <span data-ttu-id="4ee15-266">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-266">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-267">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-267">Compute</span></span>

* <span data-ttu-id="4ee15-268">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-268">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="4ee15-269">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="4ee15-269">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="4ee15-270">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="4ee15-270">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="4ee15-271">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-271">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="4ee15-272">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-272">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="4ee15-273">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-273">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-274">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-274">Core</span></span>

* <span data-ttu-id="4ee15-275">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-275">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-276">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-276">IoT</span></span>

* <span data-ttu-id="4ee15-277">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="4ee15-277">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-278">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-278">Monitor</span></span>

* <span data-ttu-id="4ee15-279">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="4ee15-279">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-280">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-280">Network</span></span>

* <span data-ttu-id="4ee15-281">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-281">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="4ee15-282">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-282">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-283">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-283">SQL</span></span>

* <span data-ttu-id="4ee15-284">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-284">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-285">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-285">Storage</span></span>

* <span data-ttu-id="4ee15-286">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-286">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="4ee15-287">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-287">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="4ee15-288">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-288">September 24, 2019</span></span>

<span data-ttu-id="4ee15-289">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="4ee15-289">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-290">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-290">ACR</span></span>

* <span data-ttu-id="4ee15-291">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-291">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="4ee15-292">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-292">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-293">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-293">AKS</span></span>

* <span data-ttu-id="4ee15-294">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-294">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="4ee15-295">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-295">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="4ee15-296">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-296">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="4ee15-297">ARM</span><span class="sxs-lookup"><span data-stu-id="4ee15-297">ARM</span></span>

* <span data-ttu-id="4ee15-298">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-298">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-299">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-299">Compute</span></span>

* <span data-ttu-id="4ee15-300">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-300">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="4ee15-301">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-301">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="4ee15-302">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-302">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="4ee15-303">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="4ee15-303">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="4ee15-304">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4ee15-304">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4ee15-305">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-305">Cosmos DB</span></span>

* <span data-ttu-id="4ee15-306">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-306">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="4ee15-307">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-307">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="4ee15-308">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4ee15-308">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4ee15-309">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-309">EventGrid</span></span>

* <span data-ttu-id="4ee15-310">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-310">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-311">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-311">Key Vault</span></span>

* <span data-ttu-id="4ee15-312">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-312">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-313">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-313">Monitor</span></span>

* <span data-ttu-id="4ee15-314">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-314">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="4ee15-315">Политика</span><span class="sxs-lookup"><span data-stu-id="4ee15-315">Policy</span></span>

* <span data-ttu-id="4ee15-316">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-316">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="4ee15-317">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-317">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-318">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-318">Storage</span></span>

* <span data-ttu-id="4ee15-319">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-319">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="4ee15-320">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-320">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-321">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-321">ACR</span></span>

* <span data-ttu-id="4ee15-322">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-322">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-323">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-323">AKS</span></span>

* <span data-ttu-id="4ee15-324">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4ee15-324">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="4ee15-325">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-325">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="4ee15-326">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-326">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="4ee15-327">ARM</span><span class="sxs-lookup"><span data-stu-id="4ee15-327">ARM</span></span>

* <span data-ttu-id="4ee15-328">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="4ee15-328">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-329">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-329">Batch</span></span>

* <span data-ttu-id="4ee15-330">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-330">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="4ee15-331">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="4ee15-331">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="4ee15-332">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="4ee15-332">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="4ee15-333">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-333">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="4ee15-334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-334">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="4ee15-335">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="4ee15-335">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="4ee15-336">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-336">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-337">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-337">HDInsight</span></span>

* <span data-ttu-id="4ee15-338">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="4ee15-338">GA release</span></span>
* <span data-ttu-id="4ee15-339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4ee15-339">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-340">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-340">Key Vault</span></span>

* <span data-ttu-id="4ee15-341">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="4ee15-341">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="4ee15-342">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="4ee15-342">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-343">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-343">Network</span></span>

* <span data-ttu-id="4ee15-344">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="4ee15-344">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="4ee15-345">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="4ee15-345">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="4ee15-346">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-346">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="4ee15-347">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-347">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="4ee15-348">Политика</span><span class="sxs-lookup"><span data-stu-id="4ee15-348">Policy</span></span>

* <span data-ttu-id="4ee15-349">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-349">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="4ee15-350">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-350">August 27, 2019</span></span>

<span data-ttu-id="4ee15-351">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="4ee15-351">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-352">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-352">ACR</span></span>

* <span data-ttu-id="4ee15-353">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-353">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="4ee15-354">Управление API</span><span class="sxs-lookup"><span data-stu-id="4ee15-354">API Management</span></span>

* <span data-ttu-id="4ee15-355">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-355">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-356">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-356">AppService</span></span>

* <span data-ttu-id="4ee15-357">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="4ee15-357">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="4ee15-358">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-358">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-359">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-359">Keyvault</span></span>

* <span data-ttu-id="4ee15-360">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-360">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-361">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-361">Network</span></span>

* <span data-ttu-id="4ee15-362">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-362">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="4ee15-363">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="4ee15-363">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="4ee15-364">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-364">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="4ee15-365">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="4ee15-365">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-366">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-366">RBAC</span></span>

* <span data-ttu-id="4ee15-367">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="4ee15-367">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4ee15-368">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-368">ServiceFabric</span></span>

* <span data-ttu-id="4ee15-369">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="4ee15-369">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="4ee15-370">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="4ee15-370">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="4ee15-371">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="4ee15-371">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="4ee15-372">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="4ee15-372">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="4ee15-373">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-373">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="4ee15-374">SignalR</span><span class="sxs-lookup"><span data-stu-id="4ee15-374">SignalR</span></span>

* <span data-ttu-id="4ee15-375">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="4ee15-375">Added new commands:</span></span>
  * <span data-ttu-id="4ee15-376">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="4ee15-376">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="4ee15-377">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="4ee15-377">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="4ee15-378">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="4ee15-378">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="4ee15-379">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-379">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-380">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-380">Storage</span></span>

* <span data-ttu-id="4ee15-381">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-381">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="4ee15-382">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-382">August 13, 2019</span></span>

<span data-ttu-id="4ee15-383">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="4ee15-383">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-384">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-384">AppService</span></span>

* <span data-ttu-id="4ee15-385">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="4ee15-385">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-386">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-386">BotService</span></span>

* <span data-ttu-id="4ee15-387">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="4ee15-387">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="4ee15-388">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="4ee15-388">CognitiveServices</span></span>

* <span data-ttu-id="4ee15-389">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-389">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4ee15-390">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-390">Cosmos DB</span></span>

* <span data-ttu-id="4ee15-391">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-391">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="4ee15-392">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-392">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-393">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-393">HDInsight</span></span>

<span data-ttu-id="4ee15-394">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-394">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="4ee15-395">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-395">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="4ee15-396">Команда `--storage-default-container` переименована в `--storage-container`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-396">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="4ee15-397">Команда `--storage-default-filesystem` переименована в `--storage-filesystem`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-397">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="4ee15-398">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-398">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="4ee15-399">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-399">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="4ee15-400">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-400">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="4ee15-401">Команда `--application-type` переименована в `--type`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-401">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="4ee15-402">Команда `--marketplace-identifier` переименована в `--marketplace-id`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-402">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="4ee15-403">Команда `--https-endpoint-access-mode` переименована в `--access-mode`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-403">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="4ee15-404">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-404">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="4ee15-405">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-405">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="4ee15-406">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-406">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="4ee15-407">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-407">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="4ee15-408">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-408">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="4ee15-409">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-409">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="4ee15-410">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-410">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="4ee15-411">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="4ee15-411">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="4ee15-412">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-412">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="4ee15-413">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-413">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="4ee15-414">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-414">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="4ee15-415">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-415">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="4ee15-416">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="4ee15-416">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="4ee15-417">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-417">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-418">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-418">Interactive</span></span>

* <span data-ttu-id="4ee15-419">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-419">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="4ee15-420">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4ee15-420">Kubernetes</span></span>

* <span data-ttu-id="4ee15-421">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-421">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-422">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-422">Network</span></span>

* <span data-ttu-id="4ee15-423">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-423">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-424">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-424">Profile</span></span>

* <span data-ttu-id="4ee15-425">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4ee15-425">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4ee15-426">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-426">ServiceFabric</span></span>

* <span data-ttu-id="4ee15-427">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="4ee15-427">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="4ee15-428">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="4ee15-428">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-429">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-429">Storage</span></span>

* <span data-ttu-id="4ee15-430">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-430">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="4ee15-431">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-431">July 30, 2019</span></span>

<span data-ttu-id="4ee15-432">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="4ee15-432">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-433">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-433">ACR</span></span>

* <span data-ttu-id="4ee15-434">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="4ee15-434">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="4ee15-435">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-435">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-436">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-436">Appservice</span></span>

* <span data-ttu-id="4ee15-437">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="4ee15-437">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="4ee15-438">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-438">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="4ee15-439">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="4ee15-439">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-440">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-440">Network</span></span>

* <span data-ttu-id="4ee15-441">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="4ee15-441">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="4ee15-442">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="4ee15-442">Fixes #9604.</span></span> <span data-ttu-id="4ee15-443">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-443">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="4ee15-444">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="4ee15-444">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-445">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-445">RBAC</span></span>

* <span data-ttu-id="4ee15-446">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-446">Added `user update` command</span></span>
* <span data-ttu-id="4ee15-447">[УСТАРЕЛО] `--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-447">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="4ee15-448">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-448">Use replacement argument `--id`</span></span>
* <span data-ttu-id="4ee15-449">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-449">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-450">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-450">SQL</span></span>

* <span data-ttu-id="4ee15-451">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-451">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-452">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-452">Storage</span></span>

* <span data-ttu-id="4ee15-453">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-453">Added `storage remove` command</span></span>
* <span data-ttu-id="4ee15-454">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-454">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-455">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-455">VM</span></span>

* <span data-ttu-id="4ee15-456">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-456">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="4ee15-457">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-457">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="4ee15-458">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-458">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="4ee15-459">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-459">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="4ee15-460">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4ee15-460">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="4ee15-461">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-461">July 16, 2019</span></span>

<span data-ttu-id="4ee15-462">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="4ee15-462">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-463">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-463">Appservice</span></span>

* <span data-ttu-id="4ee15-464">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-464">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="4ee15-465">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="4ee15-465">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="4ee15-466">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-466">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-467">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-467">Core</span></span>

* <span data-ttu-id="4ee15-468">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="4ee15-468">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-469">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-469">Batch</span></span>

* <span data-ttu-id="4ee15-470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-470">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="4ee15-471">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-471">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="4ee15-472">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-472">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="4ee15-473">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-473">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4ee15-474">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-474">Eventhubs</span></span>

* <span data-ttu-id="4ee15-475">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-475">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-476">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-476">RDBMS</span></span>

* <span data-ttu-id="4ee15-477">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="4ee15-477">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="4ee15-478">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-478">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="4ee15-479">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="4ee15-479">Relay</span></span>

* <span data-ttu-id="4ee15-480">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-480">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="4ee15-481">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-481">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="4ee15-482">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-482">Servicebus</span></span>

* <span data-ttu-id="4ee15-483">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-483">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-484">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-484">Storage</span></span>

* <span data-ttu-id="4ee15-485">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="4ee15-485">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="4ee15-486">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-486">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="4ee15-487">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-487">July 2, 2019</span></span>

<span data-ttu-id="4ee15-488">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="4ee15-488">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-489">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-489">Core</span></span>

* <span data-ttu-id="4ee15-490">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="4ee15-490">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="4ee15-491">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-491">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="4ee15-492">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-492">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-493">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-493">ACR</span></span>

* <span data-ttu-id="4ee15-494">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-494">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-495">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-495">Appservice</span></span>

* <span data-ttu-id="4ee15-496">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-496">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="4ee15-497">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-497">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="4ee15-498">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-498">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="4ee15-499">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-499">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4ee15-500">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-500">Cosmos DB</span></span>

* <span data-ttu-id="4ee15-501">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-501">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="4ee15-502">DLS</span><span class="sxs-lookup"><span data-stu-id="4ee15-502">DLS</span></span>

* <span data-ttu-id="4ee15-503">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="4ee15-503">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="4ee15-504">Отзыв</span><span class="sxs-lookup"><span data-stu-id="4ee15-504">Feedback</span></span>

* <span data-ttu-id="4ee15-505">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-505">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-506">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-506">HDInsight</span></span>

* <span data-ttu-id="4ee15-507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-507">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="4ee15-508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="4ee15-508">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="4ee15-509">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-509">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="4ee15-510">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-510">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="4ee15-511">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-511">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="4ee15-512">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-512">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="4ee15-513">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-513">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="4ee15-514">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-514">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="4ee15-515">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-515">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="4ee15-516">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="4ee15-516">Managed Services</span></span>

* <span data-ttu-id="4ee15-517">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-517">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-518">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-518">Profile</span></span>
* <span data-ttu-id="4ee15-519">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="4ee15-519">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-520">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-520">RBAC</span></span>

* <span data-ttu-id="4ee15-521">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-521">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="4ee15-522">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="4ee15-522">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="4ee15-523">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-523">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="4ee15-524">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-524">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-525">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-525">RDBMS</span></span>

* <span data-ttu-id="4ee15-526">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-526">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-527">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-527">SQL</span></span>

* <span data-ttu-id="4ee15-528">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-528">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-529">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-529">Storage</span></span>

* <span data-ttu-id="4ee15-530">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-530">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="4ee15-531">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-531">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="4ee15-532">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-532">VM</span></span>

* <span data-ttu-id="4ee15-533">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-533">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="4ee15-534">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee15-534">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="4ee15-535">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-535">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="4ee15-536">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-536">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="4ee15-537">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-537">June 18, 2019</span></span>

<span data-ttu-id="4ee15-538">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="4ee15-538">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-539">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-539">Core</span></span>

<span data-ttu-id="4ee15-540">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-540">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="4ee15-541">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="4ee15-541">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="4ee15-542">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="4ee15-542">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="4ee15-543">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-543">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="4ee15-544">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-544">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="4ee15-545">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="4ee15-545">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="4ee15-546">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="4ee15-546">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-547">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-547">ACR</span></span>
* <span data-ttu-id="4ee15-548">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="4ee15-548">Added 'acr check-health' command</span></span>
* <span data-ttu-id="4ee15-549">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-549">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-550">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-550">ACS</span></span>
* <span data-ttu-id="4ee15-551">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-551">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-552">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-552">AMS</span></span>
* <span data-ttu-id="4ee15-553">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="4ee15-553">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-554">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-554">AppService</span></span>
* <span data-ttu-id="4ee15-555">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-555">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="4ee15-556">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-556">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="4ee15-557">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="4ee15-557">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="4ee15-558">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-558">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="4ee15-559">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="4ee15-559">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="4ee15-560">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-560">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-561">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-561">Batch</span></span>
* <span data-ttu-id="4ee15-562">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-562">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-563">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-563">BatchAI</span></span>
* <span data-ttu-id="4ee15-564">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="4ee15-564">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-565">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-565">BotService</span></span>
* <span data-ttu-id="4ee15-566">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="4ee15-566">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-567">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-567">CosmosDB</span></span>
* <span data-ttu-id="4ee15-568">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-568">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="4ee15-569">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-569">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="4ee15-570">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="4ee15-570">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="4ee15-571">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="4ee15-571">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4ee15-572">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-572">EventGrid</span></span>
* <span data-ttu-id="4ee15-573">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="4ee15-573">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="4ee15-574">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="4ee15-574">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="4ee15-575">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="4ee15-575">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="4ee15-576">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-576">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="4ee15-577">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-577">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-578">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-578">HDInsight</span></span>
* <span data-ttu-id="4ee15-579">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-579">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-580">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-580">IoT</span></span>
* <span data-ttu-id="4ee15-581">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-581">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="4ee15-582">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="4ee15-582">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-583">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-583">Network</span></span>
* <span data-ttu-id="4ee15-584">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="4ee15-584">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="4ee15-585">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-585">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="4ee15-586">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="4ee15-586">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="4ee15-587">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-587">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-588">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-588">Resource</span></span>
* <span data-ttu-id="4ee15-589">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="4ee15-589">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="4ee15-590">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-590">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="4ee15-591">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-591">ServiceBus</span></span>
* <span data-ttu-id="4ee15-592">Исправлена ошибка [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-592">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-593">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-593">SQL</span></span>
* <span data-ttu-id="4ee15-594">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-594">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="4ee15-595">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-595">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="4ee15-596">SQLVm</span><span class="sxs-lookup"><span data-stu-id="4ee15-596">SQLVm</span></span>
* <span data-ttu-id="4ee15-597">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-597">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="4ee15-598">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-598">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-599">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-599">Storage</span></span>
* <span data-ttu-id="4ee15-600">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-600">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="4ee15-601">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-601">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-602">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-602">VM</span></span>
* <span data-ttu-id="4ee15-603">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4ee15-603">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="4ee15-604">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-604">June 4, 2019</span></span>

<span data-ttu-id="4ee15-605">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="4ee15-605">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-606">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-606">Core</span></span>
* <span data-ttu-id="4ee15-607">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="4ee15-607">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-608">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-608">ACR</span></span>
* <span data-ttu-id="4ee15-609">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-609">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-610">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-610">ACS</span></span>
* <span data-ttu-id="4ee15-611">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-611">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="4ee15-612">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="4ee15-612">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-613">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-613">Batch</span></span>
* <span data-ttu-id="4ee15-614">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="4ee15-614">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-615">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-615">IoT</span></span>
* <span data-ttu-id="4ee15-616">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="4ee15-616">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-617">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-617">Network</span></span>
* <span data-ttu-id="4ee15-618">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="4ee15-618">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="4ee15-619">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-619">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="4ee15-620">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-620">Resource</span></span>
* <span data-ttu-id="4ee15-621">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="4ee15-621">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-622">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-622">Role</span></span>
* <span data-ttu-id="4ee15-623">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-623">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-624">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-624">Compute</span></span>
* <span data-ttu-id="4ee15-625">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-625">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="4ee15-626">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-626">May 21, 2019</span></span>

<span data-ttu-id="4ee15-627">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="4ee15-627">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-628">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-628">Core</span></span>
* <span data-ttu-id="4ee15-629">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-629">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="4ee15-630">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="4ee15-630">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="4ee15-631">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-631">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-632">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-632">ACR</span></span>
* <span data-ttu-id="4ee15-633">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-633">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-634">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-634">ACS</span></span>
* <span data-ttu-id="4ee15-635">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="4ee15-635">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-636">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-636">AppService</span></span>
* <span data-ttu-id="4ee15-637">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="4ee15-637">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="4ee15-638">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-638">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="4ee15-639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-639">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="4ee15-640">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="4ee15-640">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="4ee15-641">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-641">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="4ee15-642">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-642">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="4ee15-643">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="4ee15-643">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-644">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-644">BotService</span></span>
* <span data-ttu-id="4ee15-645">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-645">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="4ee15-646">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-646">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-647">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-647">Consumption</span></span>
* <span data-ttu-id="4ee15-648">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-648">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-649">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-649">IoT</span></span>
* <span data-ttu-id="4ee15-650">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-650">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-651">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-651">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="4ee15-653">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="4ee15-653">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="4ee15-654">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-654">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-655">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-655">RDBMS</span></span>
* <span data-ttu-id="4ee15-656">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-656">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-657">RBAC</span><span class="sxs-lookup"><span data-stu-id="4ee15-657">RBAC</span></span>
* <span data-ttu-id="4ee15-658">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-658">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-659">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-659">Storage</span></span>
* <span data-ttu-id="4ee15-660">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-660">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="4ee15-661">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4ee15-661">Compute</span></span>
* <span data-ttu-id="4ee15-662">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4ee15-662">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="4ee15-663">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="4ee15-663">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="4ee15-664">__Примечание__. Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-664">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="4ee15-665">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="4ee15-665">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="4ee15-666">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-666">May 6, 2019</span></span>

<span data-ttu-id="4ee15-667">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="4ee15-667">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-668">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-668">ACS</span></span>
* <span data-ttu-id="4ee15-669">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-669">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="4ee15-670">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="4ee15-670">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="4ee15-671">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-671">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="4ee15-672">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-672">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-673">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-673">Appservice</span></span>
* <span data-ttu-id="4ee15-674">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4ee15-674">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="4ee15-675">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-675">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="4ee15-676">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-676">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="4ee15-677">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-677">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="4ee15-678">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-678">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="4ee15-679">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-679">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="4ee15-680">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-680">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="4ee15-681">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="4ee15-681">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="4ee15-682">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-682">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="4ee15-683">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-683">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-684">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-684">Batch</span></span>
* <span data-ttu-id="4ee15-685">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-685">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-686">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-686">Botservice</span></span>
* <span data-ttu-id="4ee15-687">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="4ee15-687">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="4ee15-688">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-688">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="4ee15-689">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-689">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="4ee15-690">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-690">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="4ee15-691">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-691">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="4ee15-692">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-692">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="4ee15-693">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-693">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="4ee15-694">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-694">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="4ee15-695">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4ee15-695">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="4ee15-696">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4ee15-696">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="4ee15-697">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="4ee15-697">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="4ee15-698">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-698">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="4ee15-699">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-699">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="4ee15-700">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="4ee15-700">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="4ee15-701">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-701">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="4ee15-702">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="4ee15-702">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="4ee15-703">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-703">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="4ee15-704">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-704">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="4ee15-705">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="4ee15-705">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="4ee15-706">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-706">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="4ee15-707">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-707">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="4ee15-708">Настройка</span><span class="sxs-lookup"><span data-stu-id="4ee15-708">Configure</span></span>
* <span data-ttu-id="4ee15-709">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-709">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4ee15-710">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-710">Eventhubs</span></span>
* <span data-ttu-id="4ee15-711">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-711">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="4ee15-712">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-712">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-713">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-713">Network</span></span>
* <span data-ttu-id="4ee15-714">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-714">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="4ee15-715">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-715">Policy Insights</span></span>
* <span data-ttu-id="4ee15-716">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-716">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-717">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-717">Role</span></span>
* <span data-ttu-id="4ee15-718">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="4ee15-718">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="4ee15-719">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-719">Service Bus</span></span>
* <span data-ttu-id="4ee15-720">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-720">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="4ee15-721">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-721">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="4ee15-722">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4ee15-722">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-723">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-723">SQL</span></span>
* <span data-ttu-id="4ee15-724">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-724">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-725">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-725">VM</span></span>
* <span data-ttu-id="4ee15-726">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4ee15-726">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="4ee15-727">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4ee15-727">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="4ee15-728">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-728">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="4ee15-729">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="4ee15-729">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="4ee15-730">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="4ee15-730">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="4ee15-731">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-731">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="4ee15-732">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-732">April 23, 2019</span></span>

<span data-ttu-id="4ee15-733">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="4ee15-733">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-734">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-734">ACS</span></span>
* <span data-ttu-id="4ee15-735">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-735">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="4ee15-736">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="4ee15-736">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-737">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-737">AMS</span></span>
* <span data-ttu-id="4ee15-738">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-738">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-739">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-739">AppService</span></span>
* <span data-ttu-id="4ee15-740">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-740">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="4ee15-741">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-741">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="4ee15-742">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="4ee15-742">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="4ee15-743">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="4ee15-743">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="4ee15-744">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-744">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="4ee15-745">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-745">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="4ee15-746">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="4ee15-746">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="4ee15-747">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="4ee15-747">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="4ee15-748">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-748">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="4ee15-749">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="4ee15-749">Deployment Manager</span></span>
* <span data-ttu-id="4ee15-750">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="4ee15-750">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="4ee15-751">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4ee15-751">Lab</span></span>
* <span data-ttu-id="4ee15-752">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-752">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-753">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-753">Network</span></span>
* <span data-ttu-id="4ee15-754">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="4ee15-754">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-755">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-755">Resource</span></span>
* <span data-ttu-id="4ee15-756">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-756">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="4ee15-757">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-757">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="4ee15-758">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="4ee15-758">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="4ee15-759">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ee15-759">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-760">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-760">SQL</span></span>
* <span data-ttu-id="4ee15-761">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-761">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="4ee15-762">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-762">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="4ee15-763">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-763">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="4ee15-764">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-764">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-765">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-765">Storage</span></span>
* <span data-ttu-id="4ee15-766">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-766">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-767">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-767">VM</span></span>
* <span data-ttu-id="4ee15-768">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-768">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="4ee15-769">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-769">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="4ee15-770">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-770">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="4ee15-771">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-771">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-772">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-772">Core</span></span>
* <span data-ttu-id="4ee15-773">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="4ee15-773">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-774">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-774">ACR</span></span>
* <span data-ttu-id="4ee15-775">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="4ee15-775">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-776">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-776">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="4ee15-779">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-779">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="4ee15-780">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-780">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-781">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-781">AppService</span></span>
* <span data-ttu-id="4ee15-782">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-782">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="4ee15-783">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-783">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="4ee15-784">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-784">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="4ee15-785">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-785">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="4ee15-786">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-786">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="4ee15-787">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-787">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="4ee15-788">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-788">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-789">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-789">CDN</span></span>
* <span data-ttu-id="4ee15-790">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-790">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="4ee15-791">Отзыв</span><span class="sxs-lookup"><span data-stu-id="4ee15-791">Feedback</span></span>
* <span data-ttu-id="4ee15-792">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-792">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="4ee15-793">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-793">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="4ee15-794">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="4ee15-794">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-795">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-795">Monitor</span></span>
* <span data-ttu-id="4ee15-796">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-796">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="4ee15-797">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-797">Network</span></span>
* <span data-ttu-id="4ee15-798">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-798">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="4ee15-799">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-799">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="4ee15-800">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-800">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="4ee15-801">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-801">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="4ee15-802">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="4ee15-802">PrivateDNS</span></span>
* <span data-ttu-id="4ee15-803">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-803">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-804">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-804">Resource</span></span>
* <span data-ttu-id="4ee15-805">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="4ee15-805">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-806">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-806">Role</span></span>
* <span data-ttu-id="4ee15-807">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="4ee15-807">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="4ee15-808">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-808">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-809">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-809">SQL</span></span>
* <span data-ttu-id="4ee15-810">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="4ee15-810">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-811">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-811">Storage</span></span>
* <span data-ttu-id="4ee15-812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-812">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="4ee15-813">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-813">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="4ee15-814">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="4ee15-814">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="4ee15-815">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ee15-815">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="4ee15-816">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-816">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="4ee15-817">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-817">Core</span></span>
* <span data-ttu-id="4ee15-818">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-818">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="4ee15-819">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="4ee15-819">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="4ee15-820">Облако</span><span class="sxs-lookup"><span data-stu-id="4ee15-820">Cloud</span></span>
* <span data-ttu-id="4ee15-821">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-821">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-822">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-822">ACR</span></span>
* <span data-ttu-id="4ee15-823">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-823">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="4ee15-824">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-824">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="4ee15-825">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-825">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="4ee15-826">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-826">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-827">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-827">AppService</span></span>
* <span data-ttu-id="4ee15-828">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="4ee15-828">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="4ee15-829">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-829">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="4ee15-830">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-830">BOT Service</span></span>
* <span data-ttu-id="4ee15-831">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-831">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="4ee15-832">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="4ee15-832">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="4ee15-833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-833">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="4ee15-834">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4ee15-834">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-835">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-835">CDN</span></span>
* <span data-ttu-id="4ee15-836">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-836">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="4ee15-837">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-837">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="4ee15-838">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-838">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="4ee15-839">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="4ee15-839">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-840">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-840">Cosmosdb</span></span>
* <span data-ttu-id="4ee15-841">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-841">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="4ee15-842">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-842">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-843">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-843">Interactive</span></span>
* <span data-ttu-id="4ee15-844">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="4ee15-844">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-845">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-845">Monitor</span></span>
* <span data-ttu-id="4ee15-846">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-846">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-847">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-847">Network</span></span>
* <span data-ttu-id="4ee15-848">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-848">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-849">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-849">Profile</span></span>
* <span data-ttu-id="4ee15-850">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-850">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="4ee15-851">Postgres</span><span class="sxs-lookup"><span data-stu-id="4ee15-851">Postgres</span></span> 
* <span data-ttu-id="4ee15-852">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-852">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="4ee15-853">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-853">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-854">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-854">Resource</span></span>
* <span data-ttu-id="4ee15-855">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-855">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="4ee15-856">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="4ee15-856">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="4ee15-857">График</span><span class="sxs-lookup"><span data-stu-id="4ee15-857">Graph</span></span>
* <span data-ttu-id="4ee15-858">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-858">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="4ee15-859">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-859">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="4ee15-860">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-860">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="4ee15-861">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-861">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="4ee15-862">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="4ee15-862">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-863">storage</span><span class="sxs-lookup"><span data-stu-id="4ee15-863">storage</span></span>
* <span data-ttu-id="4ee15-864">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-864">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="4ee15-865">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="4ee15-865">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="4ee15-866">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-866">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="4ee15-867">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="4ee15-867">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-868">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-868">VM</span></span>
* <span data-ttu-id="4ee15-869">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-869">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="4ee15-870">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-870">March 12, 2019</span></span>

<span data-ttu-id="4ee15-871">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="4ee15-871">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-872">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-872">Core</span></span>

* <span data-ttu-id="4ee15-873">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="4ee15-873">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-874">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-874">ACR</span></span>

* <span data-ttu-id="4ee15-875">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-875">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-876">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-876">ACS</span></span>

* <span data-ttu-id="4ee15-877">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="4ee15-877">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="4ee15-878">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-878">AppService</span></span>

* <span data-ttu-id="4ee15-879">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-879">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="4ee15-880">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-880">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="4ee15-881">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-881">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="4ee15-882">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="4ee15-882">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-883">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-883">Botservice</span></span>

* <span data-ttu-id="4ee15-884">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4ee15-884">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="4ee15-885">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4ee15-885">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="4ee15-886">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-886">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="4ee15-887">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-887">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-888">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-888">Container</span></span>

* <span data-ttu-id="4ee15-889">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-889">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="4ee15-890">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-890">EventHub</span></span>

* <span data-ttu-id="4ee15-891">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-891">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="4ee15-892">Поиск</span><span class="sxs-lookup"><span data-stu-id="4ee15-892">Find</span></span>

* <span data-ttu-id="4ee15-893">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="4ee15-893">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-894">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-894">HDInsight</span></span>

* <span data-ttu-id="4ee15-895">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-895">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-896">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-896">Network</span></span>

* <span data-ttu-id="4ee15-897">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-897">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4ee15-898">Rdbms</span></span>

* <span data-ttu-id="4ee15-899">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-899">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-900">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-900">Role</span></span>

* <span data-ttu-id="4ee15-901">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-901">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="4ee15-902">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-902">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4ee15-903">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-903">Service Fabric</span></span>

* <span data-ttu-id="4ee15-904">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-904">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="4ee15-905">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-905">February 26, 2019</span></span>

<span data-ttu-id="4ee15-906">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="4ee15-906">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-907">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-907">Core</span></span>

* <span data-ttu-id="4ee15-908">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="4ee15-908">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-909">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-909">ACR</span></span>

* <span data-ttu-id="4ee15-910">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-910">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="4ee15-911">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-911">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-912">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-912">ACS</span></span>

* <span data-ttu-id="4ee15-913">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-913">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-914">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-914">AppService</span></span>

* <span data-ttu-id="4ee15-915">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-915">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-916">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-916">Batch</span></span>
* <span data-ttu-id="4ee15-917">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-917">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="4ee15-918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-918">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="4ee15-919">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-919">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="4ee15-920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-920">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="4ee15-921">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="4ee15-921">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="4ee15-922">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ee15-922">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-923">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-923">CosmosDB</span></span>

* <span data-ttu-id="4ee15-924">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-924">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="4ee15-925">Kusto</span><span class="sxs-lookup"><span data-stu-id="4ee15-925">Kusto</span></span>

* <span data-ttu-id="4ee15-926">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="4ee15-926">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-927">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-927">Network</span></span>

* <span data-ttu-id="4ee15-928">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-928">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="4ee15-929">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-929">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="4ee15-930">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-930">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="4ee15-931">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-931">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="4ee15-932">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-932">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="4ee15-933">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-933">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="4ee15-934">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-934">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-935">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-935">Resource</span></span>

* <span data-ttu-id="4ee15-936">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-936">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="4ee15-937">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-937">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="4ee15-938">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-938">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="4ee15-939">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-939">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="4ee15-940">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-940">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-941">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-941">Role</span></span>

* <span data-ttu-id="4ee15-942">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-942">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-943">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-943">VM</span></span>

* <span data-ttu-id="4ee15-944">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-944">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="4ee15-945">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-945">February 12, 2019</span></span>

<span data-ttu-id="4ee15-946">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="4ee15-946">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-947">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-947">Core</span></span>

* <span data-ttu-id="4ee15-948">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="4ee15-948">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="4ee15-949">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-949">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-950">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-950">ACR</span></span>
* <span data-ttu-id="4ee15-951">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-951">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="4ee15-952">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-952">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-953">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-953">ACS</span></span>
* <span data-ttu-id="4ee15-954">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-954">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="4ee15-955">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-955">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="4ee15-956">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="4ee15-956">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-957">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-957">AMS</span></span>
* <span data-ttu-id="4ee15-958">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-958">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="4ee15-959">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-959">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-960">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-960">Appservice</span></span>
* <span data-ttu-id="4ee15-961">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-961">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="4ee15-962">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-962">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="4ee15-963">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-963">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="4ee15-964">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-964">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="4ee15-965">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-965">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-966">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-966">Botservice</span></span>
* <span data-ttu-id="4ee15-967">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-967">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="4ee15-968">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-968">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="4ee15-969">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-969">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="4ee15-970">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4ee15-970">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="4ee15-971">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-971">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="4ee15-972">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="4ee15-972">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="4ee15-973">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-973">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="4ee15-974">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-974">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="4ee15-975">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="4ee15-975">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="4ee15-976">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="4ee15-976">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-977">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-977">Key Vault</span></span>
* <span data-ttu-id="4ee15-978">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-978">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-979">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-979">Monitor</span></span>
* <span data-ttu-id="4ee15-980">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-980">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-981">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-981">Network</span></span>
* <span data-ttu-id="4ee15-982">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="4ee15-982">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="4ee15-983">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-983">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="4ee15-984">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-984">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="4ee15-985">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-985">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4ee15-986">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-986">Policy Insights</span></span>
* <span data-ttu-id="4ee15-987">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-987">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-988">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-988">RDBMS</span></span>
* <span data-ttu-id="4ee15-989">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-989">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="4ee15-990">Redis</span><span class="sxs-lookup"><span data-stu-id="4ee15-990">Redis</span></span>
* <span data-ttu-id="4ee15-991">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="4ee15-991">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="4ee15-992">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="4ee15-992">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="4ee15-993">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="4ee15-993">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="4ee15-994">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="4ee15-994">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="4ee15-995">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-995">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="4ee15-996">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="4ee15-996">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="4ee15-997">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-997">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-998">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-998">Role</span></span>
* <span data-ttu-id="4ee15-999">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-999">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="4ee15-1000">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1000">SQL VM</span></span>
* <span data-ttu-id="4ee15-1001">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1001">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1002">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1002">VM</span></span>
* <span data-ttu-id="4ee15-1003">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1003">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="4ee15-1004">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1004">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="4ee15-1005">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1005">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="4ee15-1006">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1006">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="4ee15-1007">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1007">January 31, 2019</span></span>

<span data-ttu-id="4ee15-1008">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="4ee15-1008">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1009">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1009">Core</span></span>

* <span data-ttu-id="4ee15-1010">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1010">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="4ee15-1011">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1011">January 28, 2019</span></span>

<span data-ttu-id="4ee15-1012">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="4ee15-1012">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1013">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1013">ACR</span></span>
* <span data-ttu-id="4ee15-1014">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1014">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1015">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1015">ACS</span></span>
* <span data-ttu-id="4ee15-1016">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1016">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4ee15-1017">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1017">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="4ee15-1018">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1018">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-1019">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1019">AMS</span></span>
* <span data-ttu-id="4ee15-1020">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1020">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="4ee15-1021">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1021">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1022">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1022">Appservice</span></span>
* <span data-ttu-id="4ee15-1023">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1023">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="4ee15-1024">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1024">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="4ee15-1025">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1025">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1026">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1026">Container</span></span>
* <span data-ttu-id="4ee15-1027">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1027">Added `container start` command</span></span>
* <span data-ttu-id="4ee15-1028">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1028">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4ee15-1029">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-1029">EventGrid</span></span>
* <span data-ttu-id="4ee15-1030">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1030">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="4ee15-1031">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1031">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="4ee15-1032">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1032">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="4ee15-1033">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1033">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="4ee15-1034">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1034">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-1035">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-1035">HDInsight</span></span>
* <span data-ttu-id="4ee15-1036">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1036">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="4ee15-1037">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1037">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="4ee15-1038">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1038">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="4ee15-1039">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1039">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="4ee15-1040">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1040">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="4ee15-1041">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1041">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-1042">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1042">IoT</span></span>
* <span data-ttu-id="4ee15-1043">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1043">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="4ee15-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="4ee15-1044">Kusto</span></span>
* <span data-ttu-id="4ee15-1045">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1045">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-1046">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-1046">Monitor</span></span>
* <span data-ttu-id="4ee15-1047">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1047">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-1048">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1048">Profile</span></span>
* <span data-ttu-id="4ee15-1049">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1049">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1050">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1050">Network</span></span>
* <span data-ttu-id="4ee15-1051">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1051">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="4ee15-1052">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1052">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1053">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1053">Resource</span></span>
* <span data-ttu-id="4ee15-1054">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1054">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="4ee15-1055">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1055">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="4ee15-1056">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1056">SQL Virtual Machine</span></span>
* <span data-ttu-id="4ee15-1057">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1057">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1058">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1058">Storage</span></span>
* <span data-ttu-id="4ee15-1059">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1059">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="4ee15-1060">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1060">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1061">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1061">VM</span></span>
* <span data-ttu-id="4ee15-1062">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1062">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="4ee15-1063">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1063">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="4ee15-1064">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1064">January 15, 2019</span></span>

<span data-ttu-id="4ee15-1065">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="4ee15-1065">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1066">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1066">ACR</span></span>
* <span data-ttu-id="4ee15-1067">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1067">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="4ee15-1068">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1068">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="4ee15-1069">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1069">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="4ee15-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1070">ACS</span></span>
* <span data-ttu-id="4ee15-1071">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1071">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1072">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1072">Appservice</span></span>
* <span data-ttu-id="4ee15-1073">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1073">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="4ee15-1074">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1074">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="4ee15-1075">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1075">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="4ee15-1076">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1076">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-1077">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-1077">Botservice</span></span>
* <span data-ttu-id="4ee15-1078">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1078">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="4ee15-1079">Настройка</span><span class="sxs-lookup"><span data-stu-id="4ee15-1079">Configure</span></span>
* <span data-ttu-id="4ee15-1080">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1080">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-1081">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-1081">CosmosDB</span></span>
* <span data-ttu-id="4ee15-1082">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1082">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-1083">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-1083">HDInsight</span></span>
* <span data-ttu-id="4ee15-1084">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1084">Added commands for managing applications</span></span>
* <span data-ttu-id="4ee15-1085">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1085">Added commands for managing script actions</span></span>
* <span data-ttu-id="4ee15-1086">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1086">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="4ee15-1087">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1087">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="4ee15-1088">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1088">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1089">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1089">Network</span></span>
* <span data-ttu-id="4ee15-1090">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-1090">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="4ee15-1091">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1091">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="4ee15-1092">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-1092">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="4ee15-1093">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1093">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1094">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1094">Role</span></span>
* <span data-ttu-id="4ee15-1095">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1095">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="4ee15-1096">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1096">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="4ee15-1097">Безопасность</span><span class="sxs-lookup"><span data-stu-id="4ee15-1097">Security</span></span>
* <span data-ttu-id="4ee15-1098">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1098">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1099">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1099">Storage</span></span>
* <span data-ttu-id="4ee15-1100">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1100">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="4ee15-1101">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1101">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="4ee15-1102">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1102">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="4ee15-1103">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1103">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="4ee15-1104">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1104">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1105">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1105">VM</span></span>
* <span data-ttu-id="4ee15-1106">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1106">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="4ee15-1107">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1107">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4ee15-1108">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1108">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="4ee15-1109">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1109">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="4ee15-1110">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1110">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="4ee15-1111">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1111">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="4ee15-1112">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1112">December 20, 2018</span></span>

<span data-ttu-id="4ee15-1113">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="4ee15-1113">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="4ee15-1114">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1114">Appservice</span></span>
* <span data-ttu-id="4ee15-1115">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1115">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="4ee15-1116">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1116">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="4ee15-1117">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1117">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4ee15-1118">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4ee15-1118">IoTCentral</span></span>
* <span data-ttu-id="4ee15-1119">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1119">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1120">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1120">Role</span></span>
* <span data-ttu-id="4ee15-1121">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1121">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1122">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1122">SQL</span></span>
* <span data-ttu-id="4ee15-1123">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1123">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1124">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1124">VM</span></span>
* <span data-ttu-id="4ee15-1125">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1125">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="4ee15-1126">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1126">December 18, 2018</span></span>

<span data-ttu-id="4ee15-1127">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="4ee15-1127">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="4ee15-1128">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1128">ACR</span></span>
* <span data-ttu-id="4ee15-1129">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1129">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="4ee15-1130">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1130">Condensed the table layout for task list</span></span>
* <span data-ttu-id="4ee15-1131">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1131">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1132">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1132">ACS</span></span>
* <span data-ttu-id="4ee15-1133">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1133">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4ee15-1134">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1134">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="4ee15-1135">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1135">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="4ee15-1136">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1136">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="4ee15-1137">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1137">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="4ee15-1138">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1138">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1139">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1139">Appservice</span></span>
* <span data-ttu-id="4ee15-1140">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1140">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="4ee15-1141">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-1141">Botservice</span></span>
* <span data-ttu-id="4ee15-1142">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1142">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="4ee15-1143">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1143">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="4ee15-1144">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1144">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="4ee15-1145">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1145">Reduced Kudu network calls</span></span>
* <span data-ttu-id="4ee15-1146">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1146">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-1147">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-1147">Consumption</span></span>
* <span data-ttu-id="4ee15-1148">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1148">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-1149">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-1149">CosmosDB</span></span>
* <span data-ttu-id="4ee15-1150">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1150">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="4ee15-1151">Maps</span><span class="sxs-lookup"><span data-stu-id="4ee15-1151">Maps</span></span>
* <span data-ttu-id="4ee15-1152">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1152">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1153">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1153">Network</span></span>
* <span data-ttu-id="4ee15-1154">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1154">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="4ee15-1155">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1155">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1156">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1156">Resource</span></span>
* <span data-ttu-id="4ee15-1157">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1157">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="4ee15-1158">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1158">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1159">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1159">Storage</span></span>
*  <span data-ttu-id="4ee15-1160">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1160">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1161">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1161">VM</span></span>
* <span data-ttu-id="4ee15-1162">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1162">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="4ee15-1163">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1163">December 4, 2018</span></span>

<span data-ttu-id="4ee15-1164">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="4ee15-1164">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="4ee15-1165">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1165">Core</span></span>
* <span data-ttu-id="4ee15-1166">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1166">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="4ee15-1167">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1167">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1168">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1168">Appservice</span></span>
* <span data-ttu-id="4ee15-1169">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1169">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="4ee15-1170">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1170">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1171">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1171">Network</span></span>
* <span data-ttu-id="4ee15-1172">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1172">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1173">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1173">Role</span></span>
* <span data-ttu-id="4ee15-1174">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1174">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="4ee15-1175">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1175">VM</span></span>
* <span data-ttu-id="4ee15-1176">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1176">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="4ee15-1177">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1177">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="4ee15-1178">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1178">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="4ee15-1179">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1179">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="4ee15-1180">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1180">November 20, 2018</span></span>

<span data-ttu-id="4ee15-1181">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="4ee15-1181">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="4ee15-1182">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1182">Core</span></span>
* <span data-ttu-id="4ee15-1183">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1183">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1184">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1184">ACR</span></span>
* <span data-ttu-id="4ee15-1185">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1185">Added context token to task step</span></span>
* <span data-ttu-id="4ee15-1186">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1186">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="4ee15-1187">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1187">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1188">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1188">Appservice</span></span>
* <span data-ttu-id="4ee15-1189">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1189">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="4ee15-1190">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1190">Updated the default `node_version`.</span></span> <span data-ttu-id="4ee15-1191">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1191">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="4ee15-1192">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1192">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="4ee15-1193">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1193">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4ee15-1194">IotCentral</span><span class="sxs-lookup"><span data-stu-id="4ee15-1194">IotCentral</span></span>
* <span data-ttu-id="4ee15-1195">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1195">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-1196">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1196">KeyVault</span></span>
* <span data-ttu-id="4ee15-1197">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1197">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1198">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1198">Network</span></span>
* <span data-ttu-id="4ee15-1199">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1199">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="4ee15-1200">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1200">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="4ee15-1201">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1201">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="4ee15-1202">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1202">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-1203">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4ee15-1203">Rdbms</span></span>
* <span data-ttu-id="4ee15-1204">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1204">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="4ee15-1205">RBAC:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1205">Rbac</span></span>
* <span data-ttu-id="4ee15-1206">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1206">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="4ee15-1207">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1207">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="4ee15-1208">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1208">Storage</span></span>
* <span data-ttu-id="4ee15-1209">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1209">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="4ee15-1210">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1210">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="4ee15-1211">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1211">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="4ee15-1212">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1212">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1213">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1213">VM</span></span>
* <span data-ttu-id="4ee15-1214">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1214">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="4ee15-1215">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1215">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="4ee15-1216">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1216">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="4ee15-1217">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1217">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="4ee15-1218">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1218">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="4ee15-1219">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1219">Added `snapshot wait` command</span></span>
* <span data-ttu-id="4ee15-1220">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1220">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="4ee15-1221">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1221">November 6, 2018</span></span>

<span data-ttu-id="4ee15-1222">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="4ee15-1222">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1223">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1223">Core</span></span>
* <span data-ttu-id="4ee15-1224">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1224">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1225">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1225">ACR</span></span>
* <span data-ttu-id="4ee15-1226">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1226">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="4ee15-1227">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1227">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1228">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1228">ACS</span></span>
* <span data-ttu-id="4ee15-1229">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1229">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="4ee15-1230">Помощник</span><span class="sxs-lookup"><span data-stu-id="4ee15-1230">Advisor</span></span>
* <span data-ttu-id="4ee15-1231">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="4ee15-1231">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-1232">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1232">AMS</span></span>
* <span data-ttu-id="4ee15-1233">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1233">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="4ee15-1234">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1234">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="4ee15-1235">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1235">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="4ee15-1236">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1236">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="4ee15-1237">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1237">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="4ee15-1238">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1238">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="4ee15-1239">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1239">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="4ee15-1240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1240">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="4ee15-1241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1241">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="4ee15-1242">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1242">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="4ee15-1243">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1243">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="4ee15-1244">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1244">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="4ee15-1245">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1245">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="4ee15-1246">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1246">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="4ee15-1247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1247">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="4ee15-1248">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1248">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="4ee15-1249">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1249">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1250">AppService</span></span>
* <span data-ttu-id="4ee15-1251">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1251">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="4ee15-1252">Настройка</span><span class="sxs-lookup"><span data-stu-id="4ee15-1252">Configure</span></span>
* <span data-ttu-id="4ee15-1253">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1253">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1254">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1254">Container</span></span>
* <span data-ttu-id="4ee15-1255">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1255">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="4ee15-1256">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1256">EventHub</span></span>
* <span data-ttu-id="4ee15-1257">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1257">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1258">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1258">Interactive</span></span>
* <span data-ttu-id="4ee15-1259">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1259">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-1260">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-1260">Monitor</span></span>
* <span data-ttu-id="4ee15-1261">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1261">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1262">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1262">Network</span></span>
* <span data-ttu-id="4ee15-1263">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1263">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="4ee15-1264">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1264">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="4ee15-1265">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1265">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="4ee15-1266">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1266">Profile</span></span>
* <span data-ttu-id="4ee15-1267">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1267">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-1268">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-1268">RDBMS</span></span>
* <span data-ttu-id="4ee15-1269">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1269">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1270">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1270">Resource</span></span>
* <span data-ttu-id="4ee15-1271">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1271">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1272">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1272">Role</span></span>
* <span data-ttu-id="4ee15-1273">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1273">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="4ee15-1274">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1274">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="4ee15-1275">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1275">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1276">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1276">Storage</span></span>
* <span data-ttu-id="4ee15-1277">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1277">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1278">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1278">VM</span></span>
* <span data-ttu-id="4ee15-1279">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1279">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="4ee15-1280">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1280">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="4ee15-1281">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1281">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="4ee15-1282">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1282">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="4ee15-1283">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1283">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="4ee15-1284">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1284">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="4ee15-1285">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1285">October 23, 2018</span></span>

<span data-ttu-id="4ee15-1286">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="4ee15-1286">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1287">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1287">Core</span></span>
* <span data-ttu-id="4ee15-1288">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1288">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="4ee15-1289">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1289">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1290">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1290">ACR</span></span>
* <span data-ttu-id="4ee15-1291">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1291">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-1292">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-1292">CDN</span></span>
* <span data-ttu-id="4ee15-1293">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1293">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="4ee15-1294">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1294">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1295">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1295">Container</span></span>
* <span data-ttu-id="4ee15-1296">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1296">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="4ee15-1297">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1297">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="4ee15-1298">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1298">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="4ee15-1299">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1299">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="4ee15-1300">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1300">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="4ee15-1301">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1301">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="4ee15-1302">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1302">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-1303">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-1303">CosmosDB</span></span>
* <span data-ttu-id="4ee15-1304">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1304">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1305">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1305">Interactive</span></span>
* <span data-ttu-id="4ee15-1306">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1306">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="4ee15-1307">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4ee15-1307">IoT Central</span></span>
* <span data-ttu-id="4ee15-1308">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1308">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="4ee15-1309">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1309">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-1310">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-1310">Monitor</span></span>
* <span data-ttu-id="4ee15-1311">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1311">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="4ee15-1312">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1312">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="4ee15-1313">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1313">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4ee15-1314">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1314">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="4ee15-1315">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1315">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="4ee15-1316">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1316">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="4ee15-1317">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1317">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="4ee15-1318">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1318">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4ee15-1319">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1319">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="4ee15-1320">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1320">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1321">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1321">Network</span></span>
* <span data-ttu-id="4ee15-1322">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1322">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="4ee15-1323">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1323">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="4ee15-1324">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-1324">ServiceBus</span></span>
* <span data-ttu-id="4ee15-1325">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1325">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1326">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1326">SQL</span></span>
* <span data-ttu-id="4ee15-1327">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1327">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1328">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1328">Storage</span></span>
* <span data-ttu-id="4ee15-1329">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1329">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="4ee15-1330">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1330">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1331">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1331">VM</span></span>
* <span data-ttu-id="4ee15-1332">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1332">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="4ee15-1333">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1333">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="4ee15-1334">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1334">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="4ee15-1335">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1335">October 16, 2018</span></span>

<span data-ttu-id="4ee15-1336">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="4ee15-1336">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1337">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1337">VM</span></span>
* <span data-ttu-id="4ee15-1338">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1338">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="4ee15-1339">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1339">October 9, 2018</span></span>

<span data-ttu-id="4ee15-1340">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="4ee15-1340">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1341">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1341">Core</span></span>
* <span data-ttu-id="4ee15-1342">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1342">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1343">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1343">ACR</span></span>
* <span data-ttu-id="4ee15-1344">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1344">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1345">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1345">ACS</span></span>
* <span data-ttu-id="4ee15-1346">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1346">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="4ee15-1347">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1347">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="4ee15-1348">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1348">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="4ee15-1349">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1349">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1350">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1350">Container</span></span>
* <span data-ttu-id="4ee15-1351">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1351">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="4ee15-1352">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1352">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="4ee15-1353">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-1353">Event Hub</span></span>
* <span data-ttu-id="4ee15-1354">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1354">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="4ee15-1355">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1355">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="4ee15-1356">расширения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1356">Extensions</span></span>
* <span data-ttu-id="4ee15-1357">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1357">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4ee15-1358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4ee15-1358">HDInsight</span></span>
* <span data-ttu-id="4ee15-1359">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1359">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-1360">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1360">IoT</span></span>
* <span data-ttu-id="4ee15-1361">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1361">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-1362">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1362">KeyVault</span></span>
* <span data-ttu-id="4ee15-1363">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1363">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1364">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1364">Network</span></span>
* <span data-ttu-id="4ee15-1365">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1365">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="4ee15-1366">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1366">See #6052</span></span>
* <span data-ttu-id="4ee15-1367">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1367">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="4ee15-1368">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1368">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="4ee15-1369">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1369">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="4ee15-1370">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1370">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="4ee15-1371">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1371">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="4ee15-1372">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1372">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1373">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1373">Role</span></span>
* <span data-ttu-id="4ee15-1374">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1374">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="4ee15-1375">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1375">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="4ee15-1376">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1376">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="4ee15-1377">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1377">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="4ee15-1378">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-1378">Service Bus</span></span>
* <span data-ttu-id="4ee15-1379">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1379">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1380">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1380">VM</span></span>
* <span data-ttu-id="4ee15-1381">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1381">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="4ee15-1382">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1382">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="4ee15-1383">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1383">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="4ee15-1384">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1384">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="4ee15-1385">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1385">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="4ee15-1386">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1386">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="4ee15-1387">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1387">September 21, 2018</span></span>

<span data-ttu-id="4ee15-1388">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="4ee15-1388">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1389">ACR</span></span>
* <span data-ttu-id="4ee15-1390">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1390">Added ACR Task commands</span></span>
* <span data-ttu-id="4ee15-1391">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1391">Added quick run command</span></span>
* <span data-ttu-id="4ee15-1392">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1392">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="4ee15-1393">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1393">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="4ee15-1394">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1394">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="4ee15-1395">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1395">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1396">ACS</span></span>
* <span data-ttu-id="4ee15-1397">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1397">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="4ee15-1398">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1398">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1399">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1399">AppService</span></span>

* <span data-ttu-id="4ee15-1400">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1400">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="4ee15-1401">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1401">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="4ee15-1402">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1402">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="4ee15-1403">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1403">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-1404">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-1404">Batch</span></span>
* <span data-ttu-id="4ee15-1405">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1405">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="4ee15-1406">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1406">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="4ee15-1407">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1407">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="4ee15-1408">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1408">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4ee15-1409">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1409">Batch AI</span></span> 
* <span data-ttu-id="4ee15-1410">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1410">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4ee15-1411">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4ee15-1411">Cognitive Services</span></span>
* <span data-ttu-id="4ee15-1412">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1412">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="4ee15-1413">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1413">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="4ee15-1414">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1414">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="4ee15-1415">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1415">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="4ee15-1416">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1416">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="4ee15-1417">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1417">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1418">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1418">Container</span></span>
* <span data-ttu-id="4ee15-1419">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1419">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="4ee15-1420">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1420">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="4ee15-1421">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1421">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="4ee15-1422">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1422">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="4ee15-1423">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4ee15-1423">Datalake</span></span>
* <span data-ttu-id="4ee15-1424">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1424">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="4ee15-1425">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="4ee15-1425">Interactive Shell</span></span>
* <span data-ttu-id="4ee15-1426">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1426">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="4ee15-1427">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1427">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-1428">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1428">IoT</span></span>
* <span data-ttu-id="4ee15-1429">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1429">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-1430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4ee15-1430">Key Vault</span></span>
* <span data-ttu-id="4ee15-1431">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1431">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1432">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1432">Network</span></span>
* <span data-ttu-id="4ee15-1433">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1433">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="4ee15-1434">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1434">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="4ee15-1435">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="4ee15-1435">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="4ee15-1436">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1436">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="4ee15-1437">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1437">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="4ee15-1438">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1438">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="4ee15-1439">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1439">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="4ee15-1440">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1440">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="4ee15-1441">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1441">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="4ee15-1442">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1442">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="4ee15-1443">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1443">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="4ee15-1444">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1444">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="4ee15-1445">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1445">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="4ee15-1446">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1446">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="4ee15-1447">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1447">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="4ee15-1448">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1448">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="4ee15-1449">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1449">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="4ee15-1450">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1450">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-1451">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-1451">RDBMS</span></span>
* <span data-ttu-id="4ee15-1452">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1452">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="4ee15-1453">резервирование.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1453">Reservation</span></span>
* <span data-ttu-id="4ee15-1454">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1454">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="4ee15-1455">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1455">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="4ee15-1456">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="4ee15-1456">Manage App</span></span>
* <span data-ttu-id="4ee15-1457">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1457">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="4ee15-1458">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1458">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1459">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1459">Role</span></span>
* <span data-ttu-id="4ee15-1460">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1460">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="4ee15-1461">SignalR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1461">SignalR</span></span>
* <span data-ttu-id="4ee15-1462">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1462">First release</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1463">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1463">Storage</span></span>
* <span data-ttu-id="4ee15-1464">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1464">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="4ee15-1465">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1465">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1466">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1466">VM</span></span>
* <span data-ttu-id="4ee15-1467">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1467">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="4ee15-1468">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1468">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="4ee15-1469">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1469">August 28, 2018</span></span>

<span data-ttu-id="4ee15-1470">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="4ee15-1470">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1471">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1471">Core</span></span>

* <span data-ttu-id="4ee15-1472">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1472">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="4ee15-1473">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1473">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1474">ACR</span></span>

* <span data-ttu-id="4ee15-1475">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1475">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="4ee15-1476">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1476">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1477">ACS</span></span>

* <span data-ttu-id="4ee15-1478">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1478">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="4ee15-1479">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1479">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1480">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1480">AppService</span></span>

* <span data-ttu-id="4ee15-1481">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1481">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="4ee15-1482">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1482">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="4ee15-1483">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1483">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-1484">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-1484">Backup</span></span>

* <span data-ttu-id="4ee15-1485">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1485">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="4ee15-1486">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-1486">Bot Service</span></span>

* <span data-ttu-id="4ee15-1487">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="4ee15-1487">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4ee15-1488">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4ee15-1488">Cognitive Services</span></span>

* <span data-ttu-id="4ee15-1489">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1489">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-1490">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1490">IoT</span></span>

* <span data-ttu-id="4ee15-1491">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1491">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-1492">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-1492">Monitor</span></span>

* <span data-ttu-id="4ee15-1493">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1493">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="4ee15-1494">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1494">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1495">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1495">Network</span></span>

* <span data-ttu-id="4ee15-1496">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1496">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1497">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1497">Resource</span></span>

* <span data-ttu-id="4ee15-1498">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1498">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1499">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1499">Storage</span></span>

* <span data-ttu-id="4ee15-1500">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1500">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1501">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1501">VM</span></span>

* <span data-ttu-id="4ee15-1502">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1502">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="4ee15-1503">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1503">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="4ee15-1504">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1504">Auguest 14, 2018</span></span>

<span data-ttu-id="4ee15-1505">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="4ee15-1505">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1506">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1506">Core</span></span>

* <span data-ttu-id="4ee15-1507">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1507">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="4ee15-1508">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1508">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="4ee15-1509">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="4ee15-1509">Telemetry</span></span>

* <span data-ttu-id="4ee15-1510">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1510">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1511">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1511">ACR</span></span>

* <span data-ttu-id="4ee15-1512">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1512">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="4ee15-1513">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1513">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1514">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1514">ACS</span></span>

* <span data-ttu-id="4ee15-1515">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1515">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="4ee15-1516">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1516">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="4ee15-1517">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1517">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="4ee15-1518">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1518">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="4ee15-1519">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1519">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="4ee15-1520">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1520">AppService</span></span>

* <span data-ttu-id="4ee15-1521">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1521">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="4ee15-1522">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1522">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-1523">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1523">BatchAI</span></span>

* <span data-ttu-id="4ee15-1524">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1524">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="4ee15-1525">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1525">Container</span></span>

* <span data-ttu-id="4ee15-1526">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1526">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="4ee15-1527">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1527">IoT</span></span>

* <span data-ttu-id="4ee15-1528">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1528">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="4ee15-1529">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1529">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="4ee15-1530">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4ee15-1530">Iot Central</span></span>

* <span data-ttu-id="4ee15-1531">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="4ee15-1531">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-1532">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1532">KeyVault</span></span>


* <span data-ttu-id="4ee15-1533">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1533">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="4ee15-1534">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1534">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="4ee15-1535">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1535">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="4ee15-1536">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1536">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="4ee15-1537">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1537">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="4ee15-1538">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="4ee15-1538">Relay</span></span>

* <span data-ttu-id="4ee15-1539">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1539">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1540">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1540">Sql</span></span>

* <span data-ttu-id="4ee15-1541">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1541">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1542">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1542">Storage</span></span>

* <span data-ttu-id="4ee15-1543">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1543">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="4ee15-1544">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1544">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="4ee15-1545">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1545">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="4ee15-1546">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1546">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="4ee15-1547">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1547">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1548">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1548">VM</span></span>

* <span data-ttu-id="4ee15-1549">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1549">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="4ee15-1550">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1550">July 31, 2018</span></span>

<span data-ttu-id="4ee15-1551">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="4ee15-1551">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1552">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1552">ACR</span></span>

* <span data-ttu-id="4ee15-1553">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1553">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="4ee15-1554">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1554">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1555">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1555">ACS</span></span>

* <span data-ttu-id="4ee15-1556">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1556">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-1557">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-1557">Batch</span></span>

* <span data-ttu-id="4ee15-1558">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1558">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1559">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1559">Container</span></span>

* <span data-ttu-id="4ee15-1560">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1560">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1561">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1561">Network</span></span>

* <span data-ttu-id="4ee15-1562">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1562">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="4ee15-1563">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1563">Resource</span></span>

* <span data-ttu-id="4ee15-1564">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1564">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="4ee15-1565">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1565">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1566">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1566">Role</span></span>

* <span data-ttu-id="4ee15-1567">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1567">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="4ee15-1568">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1568">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="4ee15-1569">Поиск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1569">Search</span></span>

* <span data-ttu-id="4ee15-1570">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1570">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="4ee15-1571">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-1571">Service Bus</span></span>

* <span data-ttu-id="4ee15-1572">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1572">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="4ee15-1573">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1573">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="4ee15-1574">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="4ee15-1574">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="4ee15-1575">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1575">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1576">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1576">Storage</span></span>

* <span data-ttu-id="4ee15-1577">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1577">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="4ee15-1578">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1578">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1579">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1579">VM</span></span>

* <span data-ttu-id="4ee15-1580">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1580">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="4ee15-1581">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1581">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="4ee15-1582">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1582">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="4ee15-1583">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1583">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="4ee15-1584">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1584">July 18, 2018</span></span>

<span data-ttu-id="4ee15-1585">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="4ee15-1585">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1586">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1586">Core</span></span>

* <span data-ttu-id="4ee15-1587">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1587">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="4ee15-1588">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1588">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="4ee15-1589">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1589">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1590">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1590">ACR</span></span>

* <span data-ttu-id="4ee15-1591">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1591">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="4ee15-1592">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1592">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="4ee15-1593">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1593">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="4ee15-1594">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1594">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1595">ACS</span></span>

* <span data-ttu-id="4ee15-1596">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1596">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1597">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1597">AppService</span></span>

* <span data-ttu-id="4ee15-1598">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1598">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-1599">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-1599">Batch</span></span>

* <span data-ttu-id="4ee15-1600">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1600">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="4ee15-1601">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1601">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4ee15-1602">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1602">Batch AI</span></span>

* <span data-ttu-id="4ee15-1603">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1603">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1604">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1604">Container</span></span>

* <span data-ttu-id="4ee15-1605">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1605">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="4ee15-1606">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1606">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1607">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1607">Network</span></span>

* <span data-ttu-id="4ee15-1608">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1608">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="4ee15-1609">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1609">Added `network nic wait`</span></span>
* <span data-ttu-id="4ee15-1610">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1610">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="4ee15-1611">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1611">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="4ee15-1612">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1612">Resource</span></span>

* <span data-ttu-id="4ee15-1613">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1613">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="4ee15-1614">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1614">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="4ee15-1615">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1615">Added `deployment wait` command</span></span>
* <span data-ttu-id="4ee15-1616">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1616">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1617">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1617">SQL</span></span>

* <span data-ttu-id="4ee15-1618">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1618">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="4ee15-1619">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1619">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="4ee15-1620">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1620">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1621">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1621">Storage</span></span>

* <span data-ttu-id="4ee15-1622">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1622">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1623">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1623">VM</span></span>

* <span data-ttu-id="4ee15-1624">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1624">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="4ee15-1625">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1625">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="4ee15-1626">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1626">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4ee15-1627">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1627">July 3, 2018</span></span>

<span data-ttu-id="4ee15-1628">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="4ee15-1628">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-1629">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1629">AKS</span></span>

* <span data-ttu-id="4ee15-1630">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1630">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4ee15-1631">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1631">July 3, 2018</span></span>

<span data-ttu-id="4ee15-1632">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="4ee15-1632">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1633">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1633">Core</span></span>

* <span data-ttu-id="4ee15-1634">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1634">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1635">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1635">ACR</span></span>

* <span data-ttu-id="4ee15-1636">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1636">Added polling build status</span></span>
* <span data-ttu-id="4ee15-1637">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1637">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="4ee15-1638">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1638">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1639">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1639">ACS</span></span>

* <span data-ttu-id="4ee15-1640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1640">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="4ee15-1641">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1641">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="4ee15-1642">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1642">Updated options for `aks browse` command.</span></span> <span data-ttu-id="4ee15-1643">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1643">Added `--listen-port` support</span></span>
* <span data-ttu-id="4ee15-1644">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1644">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="4ee15-1645">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1645">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="4ee15-1646">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1646">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1647">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1647">AppService</span></span>

* <span data-ttu-id="4ee15-1648">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1648">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="4ee15-1649">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1649">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-1650">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-1650">Backup</span></span>

* <span data-ttu-id="4ee15-1651">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1651">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-1652">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1652">BatchAI</span></span>

* <span data-ttu-id="4ee15-1653">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1653">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="4ee15-1654">Облако</span><span class="sxs-lookup"><span data-stu-id="4ee15-1654">Cloud</span></span>

* <span data-ttu-id="4ee15-1655">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1655">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1656">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1656">Container</span></span>

* <span data-ttu-id="4ee15-1657">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1657">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="4ee15-1658">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1658">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="4ee15-1659">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1659">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-1660">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1660">Extension</span></span>

* <span data-ttu-id="4ee15-1661">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1661">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1662">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1662">Network</span></span>

* <span data-ttu-id="4ee15-1663">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1663">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-1664">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4ee15-1664">Rdbms</span></span>

* <span data-ttu-id="4ee15-1665">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1665">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1666">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1666">Resource</span></span>

* <span data-ttu-id="4ee15-1667">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1667">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1668">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1668">VM</span></span>

* <span data-ttu-id="4ee15-1669">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1669">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="4ee15-1670">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1670">June 25, 2018</span></span>

<span data-ttu-id="4ee15-1671">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="4ee15-1671">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="4ee15-1672">CLI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1672">CLI</span></span>

* <span data-ttu-id="4ee15-1673">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1673">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="4ee15-1674">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1674">June 19, 2018</span></span>

<span data-ttu-id="4ee15-1675">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="4ee15-1675">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1676">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1676">Core</span></span>

* <span data-ttu-id="4ee15-1677">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1677">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1678">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1678">ACR</span></span>

* <span data-ttu-id="4ee15-1679">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1679">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="4ee15-1680">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1680">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1681">ACS</span></span>

* <span data-ttu-id="4ee15-1682">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1682">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="4ee15-1683">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1683">Added `--update` support</span></span>
* <span data-ttu-id="4ee15-1684">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1684">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="4ee15-1685">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1685">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="4ee15-1686">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1686">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="4ee15-1687">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1687">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="4ee15-1688">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1688">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="4ee15-1689">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1689">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1690">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1690">AppService</span></span>

* <span data-ttu-id="4ee15-1691">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1691">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="4ee15-1692">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1692">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-1693">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-1693">Batch</span></span>

* <span data-ttu-id="4ee15-1694">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1694">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4ee15-1695">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1695">Batch AI</span></span>

* <span data-ttu-id="4ee15-1696">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1696">Added support for workspaces.</span></span> <span data-ttu-id="4ee15-1697">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1697">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="4ee15-1698">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1698">Added support for experiments.</span></span> <span data-ttu-id="4ee15-1699">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1699">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="4ee15-1700">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1700">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="4ee15-1701">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1701">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="4ee15-1702">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1702">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="4ee15-1703">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1703">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="4ee15-1704">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1704">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="4ee15-1705">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1705">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="4ee15-1706">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1706">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="4ee15-1707">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1707">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="4ee15-1708">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1708">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="4ee15-1709">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1709">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="4ee15-1710">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1710">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="4ee15-1711">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1711">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="4ee15-1712">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1712">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="4ee15-1713">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1713">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="4ee15-1714">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="4ee15-1714">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="4ee15-1715">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="4ee15-1715">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4ee15-1716">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="4ee15-1716">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4ee15-1717">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="4ee15-1717">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="4ee15-1718">Maps</span><span class="sxs-lookup"><span data-stu-id="4ee15-1718">Maps</span></span>

* <span data-ttu-id="4ee15-1719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1719">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1720">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1720">Network</span></span>

* <span data-ttu-id="4ee15-1721">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1721">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="4ee15-1722">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1722">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="4ee15-1723">#6502</span><span class="sxs-lookup"><span data-stu-id="4ee15-1723">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="4ee15-1724">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4ee15-1724">Reservations</span></span>

* <span data-ttu-id="4ee15-1725">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1725">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="4ee15-1726">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1726">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="4ee15-1727">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1727">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="4ee15-1728">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1728">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="4ee15-1729">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1729">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="4ee15-1730">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1730">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1731">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1731">Role</span></span>

* <span data-ttu-id="4ee15-1732">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1732">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1733">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1733">SQL</span></span>

* <span data-ttu-id="4ee15-1734">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1734">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1735">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1735">Storage</span></span>

* <span data-ttu-id="4ee15-1736">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1736">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1737">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1737">VM</span></span>

* <span data-ttu-id="4ee15-1738">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1738">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="4ee15-1739">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1739">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="4ee15-1740">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1740">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4ee15-1741">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1741">June 13, 2018</span></span>

<span data-ttu-id="4ee15-1742">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="4ee15-1742">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1743">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1743">Core</span></span>

* <span data-ttu-id="4ee15-1744">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1744">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4ee15-1745">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1745">June 13, 2018</span></span>

<span data-ttu-id="4ee15-1746">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4ee15-1746">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-1747">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1747">AKS</span></span>

* <span data-ttu-id="4ee15-1748">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1748">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4ee15-1749">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1749">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="4ee15-1750">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-1750">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4ee15-1751">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-1751">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4ee15-1752">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1752">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1753">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1753">AppService</span></span>

* <span data-ttu-id="4ee15-1754">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1754">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4ee15-1755">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1755">June 5, 2018</span></span>

<span data-ttu-id="4ee15-1756">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4ee15-1756">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1757">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1757">Interactive</span></span>

* <span data-ttu-id="4ee15-1758">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1758">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4ee15-1759">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1759">June 5, 2018</span></span>

<span data-ttu-id="4ee15-1760">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4ee15-1760">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1761">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1761">Core</span></span>

* <span data-ttu-id="4ee15-1762">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1762">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4ee15-1763">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1763">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1764">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1764">ACR</span></span>

* <span data-ttu-id="4ee15-1765">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1765">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4ee15-1766">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1766">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4ee15-1767">AKS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1767">AKS</span></span>

* <span data-ttu-id="4ee15-1768">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1768">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-1769">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-1769">Batch</span></span>

* <span data-ttu-id="4ee15-1770">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4ee15-1770">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-1771">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1771">IOT</span></span>

* <span data-ttu-id="4ee15-1772">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1772">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1773">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1773">Network</span></span>

* <span data-ttu-id="4ee15-1774">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1774">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4ee15-1775">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-1775">Policy Insights</span></span>

* <span data-ttu-id="4ee15-1776">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-1776">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4ee15-1777">ARM</span><span class="sxs-lookup"><span data-stu-id="4ee15-1777">ARM</span></span>

* <span data-ttu-id="4ee15-1778">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1778">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1779">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1779">SQL</span></span>

* <span data-ttu-id="4ee15-1780">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1780">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4ee15-1781">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1781">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4ee15-1782">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1782">Storage</span></span>

* <span data-ttu-id="4ee15-1783">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1783">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1784">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1784">VM</span></span>

* <span data-ttu-id="4ee15-1785">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1785">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4ee15-1786">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1786">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4ee15-1787">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1787">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4ee15-1788">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1788">May 22, 2018</span></span>

<span data-ttu-id="4ee15-1789">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4ee15-1789">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1790">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1790">Core</span></span>

* <span data-ttu-id="4ee15-1791">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1791">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1792">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1792">ACS</span></span>

* <span data-ttu-id="4ee15-1793">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1793">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4ee15-1794">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1794">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1795">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-1795">AppService</span></span>

* <span data-ttu-id="4ee15-1796">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1796">Improved generic update commands</span></span>
* <span data-ttu-id="4ee15-1797">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1797">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1798">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1798">Container</span></span>

* <span data-ttu-id="4ee15-1799">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1799">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4ee15-1800">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1800">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-1801">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1801">Extension</span></span>

* <span data-ttu-id="4ee15-1802">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1802">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1803">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1803">Interactive</span></span>

* <span data-ttu-id="4ee15-1804">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1804">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4ee15-1805">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1805">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-1806">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-1806">KeyVault</span></span>

* <span data-ttu-id="4ee15-1807">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1807">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1808">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1808">Network</span></span>

* <span data-ttu-id="4ee15-1809">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="4ee15-1809">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4ee15-1810">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="4ee15-1810">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1811">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1811">SQL</span></span>

* <span data-ttu-id="4ee15-1812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1812">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4ee15-1813">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1813">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4ee15-1814">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1814">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="4ee15-1815">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1815">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4ee15-1816">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1816">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4ee15-1817">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1817">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4ee15-1818">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1818">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4ee15-1819">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1819">`edition`.</span></span> <span data-ttu-id="4ee15-1820">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1820">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4ee15-1821">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1821">`elasticPoolName`.</span></span> <span data-ttu-id="4ee15-1822">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1822">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4ee15-1823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1823">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4ee15-1824">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1824">`edition`.</span></span> <span data-ttu-id="4ee15-1825">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1825">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4ee15-1826">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1826">`dtu`.</span></span> <span data-ttu-id="4ee15-1827">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1827">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4ee15-1828">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1828">`databaseDtuMin`.</span></span> <span data-ttu-id="4ee15-1829">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1829">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4ee15-1830">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1830">`databaseDtuMax`.</span></span> <span data-ttu-id="4ee15-1831">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1831">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4ee15-1832">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1832">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4ee15-1833">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1833">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1834">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1834">Storage</span></span>

* <span data-ttu-id="4ee15-1835">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1835">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4ee15-1836">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1836">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1837">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1837">VM</span></span>

* <span data-ttu-id="4ee15-1838">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1838">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4ee15-1839">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1839">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4ee15-1840">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1840">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4ee15-1841">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1841">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4ee15-1842">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1842">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4ee15-1843">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1843">May 7, 2018</span></span>

<span data-ttu-id="4ee15-1844">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4ee15-1844">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-1845">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-1845">Core</span></span>

* <span data-ttu-id="4ee15-1846">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1846">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4ee15-1847">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1847">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4ee15-1848">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1848">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4ee15-1849">#5591</span><span class="sxs-lookup"><span data-stu-id="4ee15-1849">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4ee15-1850">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1850">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4ee15-1851">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1851">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4ee15-1852">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1852">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4ee15-1853">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1853">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4ee15-1854">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1854">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1855">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1855">ACR</span></span>

* <span data-ttu-id="4ee15-1856">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1856">Added ACR Build commands</span></span>
* <span data-ttu-id="4ee15-1857">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1857">Improved resource not found error messages</span></span>
* <span data-ttu-id="4ee15-1858">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1858">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4ee15-1859">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1859">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4ee15-1860">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1860">Improved repository commands error messages</span></span>
* <span data-ttu-id="4ee15-1861">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1861">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1862">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1862">ACS</span></span>

* <span data-ttu-id="4ee15-1863">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1863">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4ee15-1864">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1864">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4ee15-1865">AMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1865">AMS</span></span>

* <span data-ttu-id="4ee15-1866">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1866">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1867">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1867">Appservice</span></span>

* <span data-ttu-id="4ee15-1868">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1868">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4ee15-1869">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1869">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4ee15-1870">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1870">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4ee15-1871">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1871">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4ee15-1872">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1872">Batch AI</span></span>

* <span data-ttu-id="4ee15-1873">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1873">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4ee15-1874">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4ee15-1874">Cognitive Services</span></span>

* <span data-ttu-id="4ee15-1875">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1875">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-1876">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-1876">Consumption</span></span>

* <span data-ttu-id="4ee15-1877">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1877">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1878">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1878">Container</span></span>

* <span data-ttu-id="4ee15-1879">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1879">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4ee15-1880">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-1880">Cosmos DB</span></span>

* <span data-ttu-id="4ee15-1881">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-1881">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4ee15-1882">DMS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1882">DMS</span></span>

* <span data-ttu-id="4ee15-1883">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1883">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-1884">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1884">Extension</span></span>

* <span data-ttu-id="4ee15-1885">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1885">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1886">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1886">Interactive</span></span>

* <span data-ttu-id="4ee15-1887">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1887">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4ee15-1888">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1888">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4ee15-1889">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1889">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4ee15-1890">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1890">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4ee15-1891">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4ee15-1891">Lab</span></span>

* <span data-ttu-id="4ee15-1892">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1892">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1893">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1893">Network</span></span>

* <span data-ttu-id="4ee15-1894">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1894">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4ee15-1895">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1895">Profile</span></span>

* <span data-ttu-id="4ee15-1896">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1896">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4ee15-1897">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1897">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4ee15-1898">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1898">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4ee15-1899">Redis</span><span class="sxs-lookup"><span data-stu-id="4ee15-1899">Redis</span></span>

* <span data-ttu-id="4ee15-1900">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1900">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4ee15-1901">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1901">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4ee15-1902">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1902">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4ee15-1903">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1903">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4ee15-1904">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1904">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-1905">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1905">Role</span></span>

* <span data-ttu-id="4ee15-1906">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1906">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1907">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1907">Storage</span></span>

* <span data-ttu-id="4ee15-1908">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1908">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4ee15-1909">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1909">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4ee15-1910">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1910">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4ee15-1911">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1911">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4ee15-1912">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="4ee15-1912">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1913">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1913">VM</span></span>

* <span data-ttu-id="4ee15-1914">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1914">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4ee15-1915">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1915">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4ee15-1916">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1916">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4ee15-1917">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1917">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4ee15-1918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="4ee15-1918">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4ee15-1919">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1919">Added write accelerator support</span></span>
* <span data-ttu-id="4ee15-1920">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1920">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4ee15-1921">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1921">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4ee15-1922">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1922">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4ee15-1923">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1923">April 10, 2018</span></span>

<span data-ttu-id="4ee15-1924">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4ee15-1924">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-1925">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-1925">ACR</span></span>

* <span data-ttu-id="4ee15-1926">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1926">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-1927">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-1927">ACS</span></span>

* <span data-ttu-id="4ee15-1928">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1928">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-1929">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-1929">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4ee15-1931">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1931">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-1932">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4ee15-1932">BatchAI</span></span>

* <span data-ttu-id="4ee15-1933">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1933">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="4ee15-1934">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1934">Job level mounting</span></span>
  - <span data-ttu-id="4ee15-1935">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1935">Environment variables with secret values</span></span>
  - <span data-ttu-id="4ee15-1936">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="4ee15-1936">Performance counters settings</span></span>
  - <span data-ttu-id="4ee15-1937">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1937">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="4ee15-1938">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1938">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="4ee15-1939">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1939">Usage and limits reporting</span></span>
  - <span data-ttu-id="4ee15-1940">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1940">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="4ee15-1941">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1941">Support for custom images</span></span>
  - <span data-ttu-id="4ee15-1942">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1942">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4ee15-1943">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1943">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4ee15-1944">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1944">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4ee15-1945">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1945">National clouds are supported</span></span>
* <span data-ttu-id="4ee15-1946">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1946">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4ee15-1947">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1947">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4ee15-1948">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1948">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4ee15-1949">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1949">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4ee15-1950">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1950">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4ee15-1951">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1951">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4ee15-1952">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1952">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4ee15-1953">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1953">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4ee15-1954">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1954">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4ee15-1955">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1955">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4ee15-1956">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1956">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4ee15-1957">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1957">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4ee15-1958">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1958">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4ee15-1959">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="4ee15-1959">Billing</span></span>

* <span data-ttu-id="4ee15-1960">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1960">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-1961">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-1961">Consumption</span></span>

* <span data-ttu-id="4ee15-1962">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1962">Added `marketplace` commands</span></span>
* <span data-ttu-id="4ee15-1963">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1963">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4ee15-1964">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1964">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4ee15-1965">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1965">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4ee15-1966">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1966">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4ee15-1967">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1967">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-1968">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1968">Container</span></span>

* <span data-ttu-id="4ee15-1969">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1969">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4ee15-1970">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1970">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-1971">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-1971">Extension</span></span>

* <span data-ttu-id="4ee15-1972">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1972">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-1973">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-1973">Interactive</span></span>

* <span data-ttu-id="4ee15-1974">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1974">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4ee15-1975">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1975">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4ee15-1976">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1976">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-1977">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-1977">Network</span></span>

* <span data-ttu-id="4ee15-1978">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1978">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4ee15-1979">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1979">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="4ee15-1980">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="4ee15-1980">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="4ee15-1981">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1981">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="4ee15-1982">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1982">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4ee15-1983">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1983">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4ee15-1984">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1984">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4ee15-1985">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1985">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-1986">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-1986">Profile</span></span>

* <span data-ttu-id="4ee15-1987">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1987">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4ee15-1988">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1988">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-1989">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-1989">RDBMS</span></span>

* <span data-ttu-id="4ee15-1990">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1990">Added `georestore` command</span></span>
* <span data-ttu-id="4ee15-1991">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1991">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-1992">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-1992">Resource</span></span>

* <span data-ttu-id="4ee15-1993">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1993">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4ee15-1994">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1994">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-1995">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-1995">SQL</span></span>

* <span data-ttu-id="4ee15-1996">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1996">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-1997">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-1997">Storage</span></span>

* <span data-ttu-id="4ee15-1998">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="4ee15-1998">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-1999">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-1999">VM</span></span>

* <span data-ttu-id="4ee15-2000">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2000">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4ee15-2001">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2001">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4ee15-2003">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2003">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4ee15-2004">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2004">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="4ee15-2005">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2005">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="4ee15-2006">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2006">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4ee15-2007">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2007">March 27, 2018</span></span>

<span data-ttu-id="4ee15-2008">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4ee15-2008">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2009">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2009">Core</span></span>

* <span data-ttu-id="4ee15-2010">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2010">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2011">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2011">ACS</span></span>

* <span data-ttu-id="4ee15-2012">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2012">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2013">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2013">Appservice</span></span>

* <span data-ttu-id="4ee15-2014">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2014">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4ee15-2015">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2015">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-2016">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-2016">Backup</span></span>

* <span data-ttu-id="4ee15-2017">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2017">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4ee15-2018">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2018">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4ee15-2019">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2019">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4ee15-2020">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2020">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2021">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2021">Container</span></span>

* <span data-ttu-id="4ee15-2022">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2022">Added `container exec` command.</span></span> <span data-ttu-id="4ee15-2023">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2023">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4ee15-2024">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2024">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-2025">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2025">Extension</span></span>

* <span data-ttu-id="4ee15-2026">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2026">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4ee15-2027">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2027">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4ee15-2028">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2028">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2029">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-2029">Interactive</span></span>

* <span data-ttu-id="4ee15-2030">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2030">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4ee15-2031">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2031">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4ee15-2032">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2032">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4ee15-2033">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2033">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4ee15-2034">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4ee15-2034">Lab</span></span>

* <span data-ttu-id="4ee15-2035">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2035">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2036">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2036">Monitor</span></span>

* <span data-ttu-id="4ee15-2037">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2037">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4ee15-2038">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2038">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4ee15-2039">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2039">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2040">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2040">Network</span></span>

* <span data-ttu-id="4ee15-2041">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2041">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2042">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2042">Profile</span></span>

* <span data-ttu-id="4ee15-2043">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2043">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-2044">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-2044">RDBMS</span></span>

* <span data-ttu-id="4ee15-2045">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2045">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2046">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2046">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4ee15-2048">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2048">Role</span></span>

* <span data-ttu-id="4ee15-2049">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2049">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4ee15-2050">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2050">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4ee15-2051">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2051">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4ee15-2052">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2052">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4ee15-2053">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2053">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2054">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2054">Storage</span></span>

* <span data-ttu-id="4ee15-2055">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2055">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4ee15-2056">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2056">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2057">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2057">VM</span></span>

* <span data-ttu-id="4ee15-2058">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2058">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4ee15-2059">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2059">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4ee15-2060">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2060">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4ee15-2061">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2061">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4ee15-2062">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2062">March 13, 2018</span></span>

<span data-ttu-id="4ee15-2063">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4ee15-2063">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-2064">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-2064">ACR</span></span>

* <span data-ttu-id="4ee15-2065">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2065">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4ee15-2066">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2066">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4ee15-2067">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2067">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2068">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2068">ACS</span></span>

* <span data-ttu-id="4ee15-2069">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2069">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4ee15-2070">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2070">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4ee15-2071">Помощник</span><span class="sxs-lookup"><span data-stu-id="4ee15-2071">Advisor</span></span>

* <span data-ttu-id="4ee15-2072">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2072">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4ee15-2073">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2073">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4ee15-2074">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2074">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="4ee15-2075">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2075">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4ee15-2076">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2076">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2077">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2077">Appservice</span></span>

* <span data-ttu-id="4ee15-2078">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2078">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4ee15-2079">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2079">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4ee15-2080">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-2080">Eventhubs</span></span>

* <span data-ttu-id="4ee15-2081">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2081">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-2082">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2082">Extension</span></span>

* <span data-ttu-id="4ee15-2083">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2083">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2084">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-2084">Interactive</span></span>

* <span data-ttu-id="4ee15-2085">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2085">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4ee15-2086">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2086">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4ee15-2087">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2087">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4ee15-2088">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2088">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2089">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2089">Monitor</span></span>

* <span data-ttu-id="4ee15-2090">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2090">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4ee15-2091">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2091">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4ee15-2092">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2092">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4ee15-2093">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2093">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2094">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2094">Network</span></span>

* <span data-ttu-id="4ee15-2095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2095">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4ee15-2096">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2096">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4ee15-2097">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2097">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4ee15-2098">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2098">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2099">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2099">Profile</span></span>

* <span data-ttu-id="4ee15-2100">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2100">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4ee15-2101">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2101">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-2102">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-2102">RDBMS</span></span>

* <span data-ttu-id="4ee15-2103">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2103">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4ee15-2104">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4ee15-2104">Service Bus</span></span>

* <span data-ttu-id="4ee15-2105">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2105">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2106">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2106">Storage</span></span>

* <span data-ttu-id="4ee15-2107">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2107">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4ee15-2108">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2108">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2109">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2109">VM</span></span>

* <span data-ttu-id="4ee15-2110">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2110">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4ee15-2111">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2111">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4ee15-2112">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2112">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4ee15-2113">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2113">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4ee15-2114">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="4ee15-2114">February 27, 2018</span></span>

<span data-ttu-id="4ee15-2115">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4ee15-2115">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2116">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2116">Core</span></span>

* <span data-ttu-id="4ee15-2117">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2117">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4ee15-2118">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2118">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4ee15-2119">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2119">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2120">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2120">ACS</span></span>

* <span data-ttu-id="4ee15-2121">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2121">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4ee15-2122">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2122">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4ee15-2123">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2123">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4ee15-2124">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2124">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2125">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2125">Appservice</span></span>

* <span data-ttu-id="4ee15-2126">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4ee15-2126">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4ee15-2127">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2127">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4ee15-2128">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4ee15-2128">Cognitive Services</span></span>

* <span data-ttu-id="4ee15-2129">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2129">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-2130">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-2130">Consumption</span></span>

* <span data-ttu-id="4ee15-2131">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2131">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4ee15-2132">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2132">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2133">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2133">Container</span></span>

* <span data-ttu-id="4ee15-2134">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2134">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2135">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2135">Network</span></span>

* <span data-ttu-id="4ee15-2136">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2136">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2137">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2137">Resource</span></span>

* <span data-ttu-id="4ee15-2138">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2138">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2139">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2139">Role</span></span>

* <span data-ttu-id="4ee15-2140">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2140">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2141">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2141">SQL</span></span>

* <span data-ttu-id="4ee15-2142">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2142">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2143">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2143">Storage</span></span>

* <span data-ttu-id="4ee15-2144">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2144">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2145">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2145">VM</span></span>

* <span data-ttu-id="4ee15-2146">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2146">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4ee15-2147">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2147">February 13, 2018</span></span>

<span data-ttu-id="4ee15-2148">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4ee15-2148">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2149">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2149">Core</span></span>

* <span data-ttu-id="4ee15-2150">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2150">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2151">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2151">ACS</span></span>

* <span data-ttu-id="4ee15-2152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2152">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4ee15-2153">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2153">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4ee15-2154">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2154">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4ee15-2155">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2155">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4ee15-2156">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2156">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4ee15-2157">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2157">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4ee15-2158">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2158">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4ee15-2159">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2159">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2160">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2160">Appservice</span></span>

* <span data-ttu-id="4ee15-2161">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2161">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4ee15-2162">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2162">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-2163">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-2163">CDN</span></span>

* <span data-ttu-id="4ee15-2164">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2164">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2165">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2165">Container</span></span>

* <span data-ttu-id="4ee15-2166">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2166">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4ee15-2167">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2167">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-2168">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-2168">CosmosDB</span></span>

* <span data-ttu-id="4ee15-2169">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2169">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-2170">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2170">Extension</span></span>

* <span data-ttu-id="4ee15-2171">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2171">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4ee15-2172">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2172">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4ee15-2173">Отзыв</span><span class="sxs-lookup"><span data-stu-id="4ee15-2173">Feedback</span></span>

* <span data-ttu-id="4ee15-2174">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2174">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2175">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-2175">Interactive</span></span>

* <span data-ttu-id="4ee15-2176">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2176">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4ee15-2177">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2177">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-2178">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2178">IoT</span></span>

* <span data-ttu-id="4ee15-2179">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="4ee15-2179">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4ee15-2180">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="4ee15-2180">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4ee15-2181">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2181">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4ee15-2182">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2182">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2183">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2183">Monitor</span></span>

* <span data-ttu-id="4ee15-2184">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2184">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2185">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2185">Network</span></span>

* <span data-ttu-id="4ee15-2186">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2186">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4ee15-2187">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2187">Profile</span></span>

* <span data-ttu-id="4ee15-2188">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2188">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2189">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2189">Resource</span></span>

* <span data-ttu-id="4ee15-2190">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2190">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2191">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2191">Role</span></span>

* <span data-ttu-id="4ee15-2192">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2192">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2193">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2193">SQL</span></span>

* <span data-ttu-id="4ee15-2194">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2194">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4ee15-2195">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2195">Added `sql db rename`</span></span>
* <span data-ttu-id="4ee15-2196">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2196">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2197">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2197">Storage</span></span>

* <span data-ttu-id="4ee15-2198">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2198">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2199">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2199">VM</span></span>

* <span data-ttu-id="4ee15-2200">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2200">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4ee15-2201">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2201">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4ee15-2202">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2202">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4ee15-2203">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2203">January 31, 2018</span></span>

<span data-ttu-id="4ee15-2204">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4ee15-2204">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2205">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2205">Core</span></span>

* <span data-ttu-id="4ee15-2206">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2206">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4ee15-2207">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2207">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4ee15-2208">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2208">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4ee15-2209">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2209">Use `--verbose` to see</span></span>
* <span data-ttu-id="4ee15-2210">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2210">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2211">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2211">ACS</span></span>

* <span data-ttu-id="4ee15-2212">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2212">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4ee15-2213">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2213">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2214">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2214">Appservice</span></span>

* <span data-ttu-id="4ee15-2215">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2215">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4ee15-2216">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2216">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-2217">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-2217">CDN</span></span>

* <span data-ttu-id="4ee15-2218">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2218">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-2219">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-2219">CosmosDB</span></span>

* <span data-ttu-id="4ee15-2220">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2220">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2221">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-2221">Interactive</span></span>

* <span data-ttu-id="4ee15-2222">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2222">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2223">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2223">Network</span></span>

* <span data-ttu-id="4ee15-2224">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2224">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4ee15-2225">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2225">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4ee15-2226">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2226">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4ee15-2227">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2227">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4ee15-2228">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2228">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4ee15-2229">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2229">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4ee15-2230">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2230">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4ee15-2231">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2231">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4ee15-2232">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2232">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="4ee15-2233">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2233">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2234">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2234">Profile</span></span>

* <span data-ttu-id="4ee15-2235">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2235">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2236">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2236">Resource</span></span>

* <span data-ttu-id="4ee15-2237">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2237">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2238">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2238">Storage</span></span>

* <span data-ttu-id="4ee15-2239">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2239">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4ee15-2240">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2240">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4ee15-2241">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2241">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="4ee15-2242">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2242">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4ee15-2243">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2243">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2244">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2244">VM</span></span>

* <span data-ttu-id="4ee15-2245">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2245">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4ee15-2246">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2246">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4ee15-2247">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2247">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4ee15-2248">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2248">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4ee15-2249">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2249">January 17, 2018</span></span>

<span data-ttu-id="4ee15-2250">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4ee15-2250">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-2251">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-2251">ACR</span></span>

* <span data-ttu-id="4ee15-2252">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2252">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4ee15-2253">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2253">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2254">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2254">ACS</span></span>

* <span data-ttu-id="4ee15-2255">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2255">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4ee15-2256">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2256">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2257">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2257">Appservice</span></span>

* <span data-ttu-id="4ee15-2258">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2258">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4ee15-2259">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2259">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4ee15-2260">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2260">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-2261">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-2261">Backup</span></span>

* <span data-ttu-id="4ee15-2262">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2262">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4ee15-2263">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2263">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4ee15-2264">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2264">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4ee15-2265">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2265">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4ee15-2266">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2266">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-2267">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2267">Batch</span></span>

* <span data-ttu-id="4ee15-2268">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2268">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4ee15-2269">Облако</span><span class="sxs-lookup"><span data-stu-id="4ee15-2269">Cloud</span></span>

* <span data-ttu-id="4ee15-2270">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2270">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-2271">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-2271">Consumption</span></span>

* <span data-ttu-id="4ee15-2272">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2272">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4ee15-2273">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2273">Event Grid</span></span>

* <span data-ttu-id="4ee15-2274">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2274">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4ee15-2275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2275">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4ee15-2276">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2276">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4ee15-2277">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2277">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4ee15-2278">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2278">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4ee15-2279">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2279">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4ee15-2280">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2280">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4ee15-2281">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2281">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2282">Interactive</span><span class="sxs-lookup"><span data-stu-id="4ee15-2282">Interactive</span></span>

* <span data-ttu-id="4ee15-2283">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2283">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4ee15-2284">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2284">Fixed errors on startup</span></span>
* <span data-ttu-id="4ee15-2285">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2285">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-2286">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2286">IoT</span></span>

* <span data-ttu-id="4ee15-2287">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2287">Added support for device provisioning service</span></span>
* <span data-ttu-id="4ee15-2288">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2288">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4ee15-2289">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2289">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2290">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2290">Monitor</span></span>

* <span data-ttu-id="4ee15-2291">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2291">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4ee15-2292">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2292">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4ee15-2293">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2293">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2294">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2294">Network</span></span>

* <span data-ttu-id="4ee15-2295">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2295">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4ee15-2296">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2296">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2297">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2297">Profile</span></span>

* <span data-ttu-id="4ee15-2298">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2298">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2299">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2299">Role</span></span>

* <span data-ttu-id="4ee15-2300">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2300">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4ee15-2301">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-2301">Service Fabric</span></span>

* <span data-ttu-id="4ee15-2302">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2302">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4ee15-2303">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2303">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2304">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2304">VM</span></span>

* <span data-ttu-id="4ee15-2305">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2305">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4ee15-2306">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="4ee15-2306">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4ee15-2307">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2307">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4ee15-2308">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2308">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4ee15-2309">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2309">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4ee15-2310">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2310">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4ee15-2311">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2311">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4ee15-2312">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2312">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4ee15-2313">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2313">December 19, 2017</span></span>

<span data-ttu-id="4ee15-2314">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4ee15-2314">Version 2.0.23</span></span>

* <span data-ttu-id="4ee15-2315">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2315">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2316">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2316">Container</span></span>

* <span data-ttu-id="4ee15-2317">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2317">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2318">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2318">Network</span></span>

* <span data-ttu-id="4ee15-2319">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2319">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4ee15-2320">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2320">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2321">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2321">Storage</span></span>

* <span data-ttu-id="4ee15-2322">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2322">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2323">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2323">VM</span></span>

* <span data-ttu-id="4ee15-2324">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2324">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4ee15-2325">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2325">December 5, 2017</span></span>

<span data-ttu-id="4ee15-2326">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4ee15-2326">Version 2.0.22</span></span>

* <span data-ttu-id="4ee15-2327">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2327">Removed `az component` commands.</span></span> <span data-ttu-id="4ee15-2328">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2328">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2329">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2329">Core</span></span>
* <span data-ttu-id="4ee15-2330">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2330">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4ee15-2331">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2331">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2332">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2332">ACS</span></span>

* <span data-ttu-id="4ee15-2333">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2333">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4ee15-2334">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2334">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4ee15-2335">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2335">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4ee15-2336">Помощник</span><span class="sxs-lookup"><span data-stu-id="4ee15-2336">Advisor</span></span>

* <span data-ttu-id="4ee15-2337">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2337">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2338">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2338">Appservice</span></span>

* <span data-ttu-id="4ee15-2339">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2339">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4ee15-2340">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2340">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4ee15-2341">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2341">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4ee15-2342">Потребление</span><span class="sxs-lookup"><span data-stu-id="4ee15-2342">Consumption</span></span>

* <span data-ttu-id="4ee15-2343">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2343">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2344">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2344">Container</span></span>

* <span data-ttu-id="4ee15-2345">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2345">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2346">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2346">Monitor</span></span>

* <span data-ttu-id="4ee15-2347">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2347">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2348">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2348">Resource</span></span>

* <span data-ttu-id="4ee15-2349">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2349">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2350">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2350">Role</span></span>

* <span data-ttu-id="4ee15-2351">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2351">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4ee15-2352">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2352">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4ee15-2353">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2353">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2354">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2354">SQL</span></span>

* <span data-ttu-id="4ee15-2355">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2355">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4ee15-2356">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2356">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2357">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2357">VM</span></span>

* <span data-ttu-id="4ee15-2358">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2358">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4ee15-2359">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2359">November 14, 2017</span></span>

<span data-ttu-id="4ee15-2360">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4ee15-2360">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-2361">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-2361">ACR</span></span>

* <span data-ttu-id="4ee15-2362">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2362">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4ee15-2363">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2363">ACS</span></span>

* <span data-ttu-id="4ee15-2364">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2364">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4ee15-2365">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2365">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4ee15-2366">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2366">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4ee15-2367">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2367">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4ee15-2368">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2368">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2369">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2369">Appservice</span></span>

* <span data-ttu-id="4ee15-2370">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2370">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4ee15-2371">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2371">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4ee15-2372">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2372">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4ee15-2373">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2373">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4ee15-2374">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="4ee15-2374">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4ee15-2375">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2375">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-2376">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2376">Batch</span></span>

* <span data-ttu-id="4ee15-2377">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2377">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-2378">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4ee15-2378">Batchai</span></span>

* <span data-ttu-id="4ee15-2379">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2379">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4ee15-2380">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2380">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4ee15-2381">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2381">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4ee15-2382">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2382">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4ee15-2383">Облако</span><span class="sxs-lookup"><span data-stu-id="4ee15-2383">Cloud</span></span>

* <span data-ttu-id="4ee15-2384">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2384">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2385">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2385">Container</span></span>

* <span data-ttu-id="4ee15-2386">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2386">Added support to open multiple ports</span></span>
* <span data-ttu-id="4ee15-2387">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2387">Added container group restart policy</span></span>
* <span data-ttu-id="4ee15-2388">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2388">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4ee15-2389">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2389">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4ee15-2390">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4ee15-2390">Data Lake Analytics</span></span>

* <span data-ttu-id="4ee15-2391">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2391">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4ee15-2392">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4ee15-2392">Data Lake Store</span></span>

* <span data-ttu-id="4ee15-2393">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2393">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-2394">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2394">Extension</span></span>

* <span data-ttu-id="4ee15-2395">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2395">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4ee15-2396">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2396">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-2397">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2397">IoT</span></span>

* <span data-ttu-id="4ee15-2398">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2398">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2399">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2399">Monitor</span></span>

* <span data-ttu-id="4ee15-2400">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2400">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2401">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2401">Network</span></span>

* <span data-ttu-id="4ee15-2402">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2402">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4ee15-2403">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2403">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4ee15-2404">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2404">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4ee15-2405">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2405">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4ee15-2406">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4ee15-2406">Reservations</span></span>

* <span data-ttu-id="4ee15-2407">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="4ee15-2407">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2408">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2408">Resource</span></span>

* <span data-ttu-id="4ee15-2409">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2409">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2410">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2410">SQL</span></span>

* <span data-ttu-id="4ee15-2411">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2411">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2412">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2412">Storage</span></span>

* <span data-ttu-id="4ee15-2413">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2413">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4ee15-2414">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2414">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4ee15-2415">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2415">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4ee15-2416">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2416">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4ee15-2417">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2417">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4ee15-2418">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2418">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4ee15-2419">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2419">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2420">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2420">VM</span></span>

* <span data-ttu-id="4ee15-2421">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2421">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4ee15-2422">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2422">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4ee15-2423">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2423">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4ee15-2424">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2424">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4ee15-2425">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2425">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4ee15-2426">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2426">October 24, 2017</span></span>

<span data-ttu-id="4ee15-2427">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4ee15-2427">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2428">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2428">Core</span></span>

* <span data-ttu-id="4ee15-2429">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2429">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-2430">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-2430">ACR</span></span>

* <span data-ttu-id="4ee15-2431">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2431">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4ee15-2432">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="4ee15-2432">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4ee15-2433">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="4ee15-2433">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2434">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2434">ACS</span></span>

* <span data-ttu-id="4ee15-2435">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2435">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4ee15-2436">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2436">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2437">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2437">Appservice</span></span>

* <span data-ttu-id="4ee15-2438">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2438">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4ee15-2439">Компонент</span><span class="sxs-lookup"><span data-stu-id="4ee15-2439">Component</span></span>

* <span data-ttu-id="4ee15-2440">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="4ee15-2440">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2441">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2441">Monitor</span></span>

* <span data-ttu-id="4ee15-2442">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2442">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2443">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2443">Resource</span></span>

* <span data-ttu-id="4ee15-2444">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2444">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4ee15-2445">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-2445">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2446">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2446">VM</span></span>

* <span data-ttu-id="4ee15-2447">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2447">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4ee15-2448">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2448">October 9, 2017</span></span>

<span data-ttu-id="4ee15-2449">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4ee15-2449">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2450">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2450">Core</span></span>

* <span data-ttu-id="4ee15-2451">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2451">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2452">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2452">Appservice</span></span>

* <span data-ttu-id="4ee15-2453">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2453">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-2454">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2454">Batch</span></span>

* <span data-ttu-id="4ee15-2455">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4ee15-2455">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4ee15-2456">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2456">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4ee15-2457">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2457">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4ee15-2458">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2458">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4ee15-2459">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4ee15-2459">Batchai</span></span>

* <span data-ttu-id="4ee15-2460">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4ee15-2460">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-2461">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2461">Keyvault</span></span>

* <span data-ttu-id="4ee15-2462">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2462">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4ee15-2463">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4ee15-2463">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4ee15-2464">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2464">Network</span></span>

* <span data-ttu-id="4ee15-2465">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2465">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4ee15-2466">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2466">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2467">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2467">Resource</span></span>

* <span data-ttu-id="4ee15-2468">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2468">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4ee15-2469">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2469">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4ee15-2470">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2470">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4ee15-2471">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2471">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2472">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2472">Sql</span></span>

* <span data-ttu-id="4ee15-2473">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2473">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4ee15-2474">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2474">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4ee15-2475">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2475">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2476">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2476">Storage</span></span>

* <span data-ttu-id="4ee15-2477">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2477">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2478">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="4ee15-2478">Vm</span></span>

* <span data-ttu-id="4ee15-2479">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2479">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4ee15-2480">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2480">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4ee15-2481">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2481">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4ee15-2482">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2482">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4ee15-2483">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2483">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4ee15-2484">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2484">September 22, 2017</span></span>

<span data-ttu-id="4ee15-2485">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4ee15-2485">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2486">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2486">Resource</span></span>

* <span data-ttu-id="4ee15-2487">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-2487">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4ee15-2488">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="4ee15-2488">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4ee15-2489">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2489">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4ee15-2490">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2490">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2491">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2491">Network</span></span>

* <span data-ttu-id="4ee15-2492">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2492">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4ee15-2493">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2493">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4ee15-2494">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2494">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4ee15-2495">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2495">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4ee15-2496">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2496">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4ee15-2497">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2497">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4ee15-2498">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2498">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2499">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2499">Storage</span></span>

* <span data-ttu-id="4ee15-2500">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="4ee15-2500">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4ee15-2501">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4ee15-2501">Eventgrid</span></span>

* <span data-ttu-id="4ee15-2502">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="4ee15-2502">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2503">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2503">SQL</span></span>

* <span data-ttu-id="4ee15-2504">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2504">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4ee15-2505">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="4ee15-2505">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4ee15-2506">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2506">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-2507">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2507">Keyvault</span></span>

* <span data-ttu-id="4ee15-2508">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="4ee15-2508">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2509">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2509">VM</span></span>

* <span data-ttu-id="4ee15-2510">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2510">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4ee15-2511">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="4ee15-2511">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4ee15-2512">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2512">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4ee15-2513">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2513">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4ee15-2514">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2514">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4ee15-2515">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2515">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2516">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2516">ACS</span></span>

* <span data-ttu-id="4ee15-2517">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4ee15-2517">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2518">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2518">Appservice</span></span>

* <span data-ttu-id="4ee15-2519">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4ee15-2519">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4ee15-2520">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="4ee15-2520">Backup</span></span>

* <span data-ttu-id="4ee15-2521">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2521">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4ee15-2522">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2522">September 11, 2017</span></span>

<span data-ttu-id="4ee15-2523">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4ee15-2523">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4ee15-2524">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2524">Core</span></span>

* <span data-ttu-id="4ee15-2525">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2525">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4ee15-2526">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2526">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2527">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2527">Acs</span></span>

* <span data-ttu-id="4ee15-2528">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2528">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4ee15-2529">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2529">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2530">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2530">Appservice</span></span>

* <span data-ttu-id="4ee15-2531">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2531">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-2532">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-2532">CDN</span></span>

* <span data-ttu-id="4ee15-2533">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2533">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4ee15-2534">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2534">Extension</span></span>

* <span data-ttu-id="4ee15-2535">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2535">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-2536">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2536">Keyvault</span></span>

* <span data-ttu-id="4ee15-2537">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2537">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2538">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2538">Network</span></span>

* <span data-ttu-id="4ee15-2539">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2539">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4ee15-2540">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2540">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4ee15-2541">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2541">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4ee15-2542">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2542">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4ee15-2543">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2543">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2544">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2544">Resource</span></span>

* <span data-ttu-id="4ee15-2545">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2545">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4ee15-2546">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2546">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4ee15-2547">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2547">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4ee15-2548">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2548">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2549">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2549">SQL</span></span>

* <span data-ttu-id="4ee15-2550">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2550">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2551">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2551">VM</span></span>

* <span data-ttu-id="4ee15-2552">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2552">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4ee15-2553">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2553">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4ee15-2554">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2554">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4ee15-2555">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2555">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4ee15-2556">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2556">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4ee15-2557">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2557">August 31, 2017</span></span>

<span data-ttu-id="4ee15-2558">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4ee15-2558">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-2559">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2559">Keyvault</span></span>

* <span data-ttu-id="4ee15-2560">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2560">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4ee15-2561">Sf</span><span class="sxs-lookup"><span data-stu-id="4ee15-2561">Sf</span></span>

* <span data-ttu-id="4ee15-2562">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2562">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2563">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2563">Storage</span></span>

* <span data-ttu-id="4ee15-2564">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2564">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4ee15-2565">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2565">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4ee15-2566">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2566">August 28, 2017</span></span>

<span data-ttu-id="4ee15-2567">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4ee15-2567">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4ee15-2568">CLI</span><span class="sxs-lookup"><span data-stu-id="4ee15-2568">CLI</span></span>

* <span data-ttu-id="4ee15-2569">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2569">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2570">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2570">ACS</span></span>

* <span data-ttu-id="4ee15-2571">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2571">Corrected preview regions</span></span>
* <span data-ttu-id="4ee15-2572">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2572">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4ee15-2573">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2573">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2574">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2574">Appservice</span></span>

* <span data-ttu-id="4ee15-2575">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2575">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4ee15-2576">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2576">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4ee15-2577">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2577">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4ee15-2578">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2578">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4ee15-2579">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2579">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-2580">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2580">IoT</span></span>

* <span data-ttu-id="4ee15-2581">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2581">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2582">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2582">Network</span></span>

* <span data-ttu-id="4ee15-2583">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2583">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4ee15-2584">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2584">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4ee15-2585">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2585">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4ee15-2586">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2586">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4ee15-2587">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2587">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2588">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2588">Profile</span></span>

* <span data-ttu-id="4ee15-2589">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2589">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4ee15-2590">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-2590">Service Fabric</span></span>

* <span data-ttu-id="4ee15-2591">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2591">Preview release</span></span>
* <span data-ttu-id="4ee15-2592">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2592">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4ee15-2593">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2593">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4ee15-2594">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2594">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2595">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2595">Storage</span></span>

* <span data-ttu-id="4ee15-2596">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2596">Enabled setting blob tier</span></span>
* <span data-ttu-id="4ee15-2597">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2597">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4ee15-2598">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2598">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4ee15-2599">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2599">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4ee15-2600">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2600">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4ee15-2601">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2601">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2602">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2602">VM</span></span>

* <span data-ttu-id="4ee15-2603">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2603">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4ee15-2604">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2604">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4ee15-2605">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2605">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4ee15-2606">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2606">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4ee15-2607">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2607">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4ee15-2608">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2608">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4ee15-2609">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2609">August 15, 2017</span></span>

<span data-ttu-id="4ee15-2610">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4ee15-2610">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2611">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2611">ACS</span></span>

* <span data-ttu-id="4ee15-2612">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2612">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2613">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2613">Appservice</span></span>

* <span data-ttu-id="4ee15-2614">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2614">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4ee15-2615">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2615">Event Grid</span></span>

* <span data-ttu-id="4ee15-2616">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2616">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4ee15-2617">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2617">August 11, 2017</span></span>

<span data-ttu-id="4ee15-2618">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4ee15-2618">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2619">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2619">ACS</span></span>

* <span data-ttu-id="4ee15-2620">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2620">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-2621">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2621">Batch</span></span>

* <span data-ttu-id="4ee15-2622">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2622">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4ee15-2623">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2623">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4ee15-2624">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2624">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4ee15-2625">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2625">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4ee15-2626">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2626">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4ee15-2627">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2627">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4ee15-2628">Компонент</span><span class="sxs-lookup"><span data-stu-id="4ee15-2628">Component</span></span>

* <span data-ttu-id="4ee15-2629">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2629">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4ee15-2630">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4ee15-2630">Container</span></span>

* <span data-ttu-id="4ee15-2631">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2631">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4ee15-2632">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4ee15-2632">Data Lake Store</span></span>

* <span data-ttu-id="4ee15-2633">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2633">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4ee15-2634">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2634">Event Grid</span></span>

* <span data-ttu-id="4ee15-2635">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2635">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2636">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2636">Network</span></span>

* <span data-ttu-id="4ee15-2637">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2637">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4ee15-2638">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2638">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4ee15-2639">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2639">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4ee15-2640">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2640">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2641">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2641">Profile</span></span>

* <span data-ttu-id="4ee15-2642">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2642">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2643">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2643">Storage</span></span>

* <span data-ttu-id="4ee15-2644">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2644">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2645">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2645">VM</span></span>

* <span data-ttu-id="4ee15-2646">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2646">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4ee15-2647">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2647">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4ee15-2648">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2648">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4ee15-2649">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2649">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4ee15-2650">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2650">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4ee15-2651">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2651">July 28, 2017</span></span>

<span data-ttu-id="4ee15-2652">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4ee15-2652">Version 2.0.12</span></span>

* <span data-ttu-id="4ee15-2653">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2653">Added container commands</span></span>
* <span data-ttu-id="4ee15-2654">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2654">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4ee15-2655">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2655">Core</span></span>

* <span data-ttu-id="4ee15-2656">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2656">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4ee15-2657">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2657">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4ee15-2658">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2658">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4ee15-2659">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2659">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4ee15-2660">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2660">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4ee15-2661">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2661">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4ee15-2662">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2662">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4ee15-2663">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2663">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4ee15-2664">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2664">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4ee15-2665">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2665">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4ee15-2666">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2666">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4ee15-2667">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2667">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4ee15-2668">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2668">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4ee15-2669">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2669">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4ee15-2670">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2670">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4ee15-2671">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2671">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4ee15-2672">ACR</span><span class="sxs-lookup"><span data-stu-id="4ee15-2672">ACR</span></span>

* <span data-ttu-id="4ee15-2673">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2673">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4ee15-2674">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2674">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4ee15-2675">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2675">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4ee15-2676">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2676">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4ee15-2677">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2677">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4ee15-2678">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2678">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2679">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2679">ACS</span></span>

* <span data-ttu-id="4ee15-2680">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2680">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2681">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4ee15-2681">Appservice</span></span>

* <span data-ttu-id="4ee15-2682">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2682">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4ee15-2683">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2683">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4ee15-2684">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2684">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4ee15-2685">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2685">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4ee15-2686">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2686">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4ee15-2687">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2687">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4ee15-2688">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2688">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4ee15-2689">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2689">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4ee15-2690">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2690">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4ee15-2691">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2691">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4ee15-2692">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4ee15-2692">Batch</span></span>

* <span data-ttu-id="4ee15-2693">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2693">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4ee15-2694">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2694">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4ee15-2695">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2695">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4ee15-2696">CDN</span><span class="sxs-lookup"><span data-stu-id="4ee15-2696">CDN</span></span>

* <span data-ttu-id="4ee15-2697">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2697">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4ee15-2698">Облако</span><span class="sxs-lookup"><span data-stu-id="4ee15-2698">Cloud</span></span>

* <span data-ttu-id="4ee15-2699">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2699">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4ee15-2700">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2700">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4ee15-2701">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2701">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4ee15-2702">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2702">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4ee15-2703">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2703">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-2704">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-2704">CosmosDB</span></span>

* <span data-ttu-id="4ee15-2705">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2705">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4ee15-2706">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2706">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4ee15-2707">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4ee15-2707">Data Lake Analytics</span></span>

* <span data-ttu-id="4ee15-2708">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2708">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4ee15-2709">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2709">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4ee15-2710">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2710">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4ee15-2711">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4ee15-2711">Data Lake Store</span></span>

* <span data-ttu-id="4ee15-2712">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2712">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4ee15-2713">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2713">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4ee15-2714">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2714">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4ee15-2715">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2715">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4ee15-2716">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="4ee15-2716">Interactive</span></span>

* <span data-ttu-id="4ee15-2717">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2717">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4ee15-2718">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2718">Increased test coverage</span></span>
* <span data-ttu-id="4ee15-2719">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2719">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4ee15-2720">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2720">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4ee15-2721">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2721">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4ee15-2722">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2722">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4ee15-2723">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2723">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4ee15-2724">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2724">Added `--progress` flag</span></span>
* <span data-ttu-id="4ee15-2725">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2725">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4ee15-2726">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2726">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4ee15-2727">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2727">IoT</span></span>

* <span data-ttu-id="4ee15-2728">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="4ee15-2728">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4ee15-2729">(3934).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2729">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4ee15-2730">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2730">Key vault</span></span>

* <span data-ttu-id="4ee15-2731">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2731">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4ee15-2732">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2732">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4ee15-2733">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2733">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4ee15-2734">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2734">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4ee15-2735">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2735">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4ee15-2736">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2736">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4ee15-2737">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="4ee15-2737">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4ee15-2738">(3307).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2738">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4ee15-2739">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4ee15-2739">Lab</span></span>

* <span data-ttu-id="4ee15-2740">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2740">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4ee15-2741">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2741">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2742">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2742">Monitor</span></span>

* <span data-ttu-id="4ee15-2743">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2743">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4ee15-2744">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2744">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4ee15-2745">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2745">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4ee15-2746">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2746">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4ee15-2747">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2747">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4ee15-2748">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2748">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4ee15-2749">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2749">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4ee15-2750">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2750">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4ee15-2751">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2751">`location` no longer required</span></span>
  * <span data-ttu-id="4ee15-2752">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2752">Add name and ID support for target</span></span>
  * <span data-ttu-id="4ee15-2753">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2753">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4ee15-2754">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2754">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4ee15-2755">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2755">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4ee15-2756">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2756">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4ee15-2757">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2757">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4ee15-2758">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2758">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2759">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2759">Network</span></span>

* <span data-ttu-id="4ee15-2760">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2760">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4ee15-2761">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2761">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4ee15-2762">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2762">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4ee15-2763">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2763">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4ee15-2764">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2764">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4ee15-2765">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2765">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4ee15-2766">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2766">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4ee15-2767">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2767">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4ee15-2768">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2768">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4ee15-2769">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2769">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4ee15-2770">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2770">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4ee15-2771">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2771">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4ee15-2772">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2772">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4ee15-2773">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2773">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4ee15-2774">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2774">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4ee15-2775">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2775">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4ee15-2776">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2776">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4ee15-2777">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2777">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4ee15-2778">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2778">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4ee15-2779">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2779">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4ee15-2780">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2780">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4ee15-2781">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2781">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4ee15-2782">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2782">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4ee15-2783">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2783">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4ee15-2784">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2784">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4ee15-2785">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2785">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4ee15-2786">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2786">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2787">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2787">Profile</span></span>

* <span data-ttu-id="4ee15-2788">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2788">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4ee15-2789">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2789">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4ee15-2790">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2790">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4ee15-2791">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2791">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4ee15-2792">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2792">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4ee15-2793">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4ee15-2793">RDBMS</span></span>

* <span data-ttu-id="4ee15-2794">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2794">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4ee15-2795">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2795">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4ee15-2796">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2796">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4ee15-2797">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2797">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2798">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2798">Resource</span></span>

* <span data-ttu-id="4ee15-2799">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2799">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4ee15-2800">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2800">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4ee15-2801">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2801">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4ee15-2802">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2802">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4ee15-2803">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2803">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4ee15-2804">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2804">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4ee15-2805">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2805">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4ee15-2806">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2806">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2807">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2807">Role</span></span>

* <span data-ttu-id="4ee15-2808">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2808">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4ee15-2809">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2809">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4ee15-2810">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2810">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4ee15-2811">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2811">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4ee15-2812">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2812">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4ee15-2813">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4ee15-2813">Service Fabric</span></span>
* <span data-ttu-id="4ee15-2814">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2814">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4ee15-2815">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2815">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4ee15-2816">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2816">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2817">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2817">SQL</span></span>

* <span data-ttu-id="4ee15-2818">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2818">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4ee15-2819">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2819">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4ee15-2820">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2820">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2821">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2821">Storage</span></span>

* <span data-ttu-id="4ee15-2822">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2822">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4ee15-2823">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2823">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4ee15-2824">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2824">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4ee15-2825">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4ee15-2825">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4ee15-2826">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2826">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4ee15-2827">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2827">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2828">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2828">VM</span></span>

* <span data-ttu-id="4ee15-2829">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2829">Support configuring nsg</span></span>
* <span data-ttu-id="4ee15-2830">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2830">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4ee15-2831">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2831">Support managed service identities</span></span>
* <span data-ttu-id="4ee15-2832">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2832">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4ee15-2833">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2833">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4ee15-2834">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2834">May 10, 2017</span></span>

<span data-ttu-id="4ee15-2835">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4ee15-2835">Version 2.0.6</span></span>

* <span data-ttu-id="4ee15-2836">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2836">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4ee15-2837">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2837">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4ee15-2838">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2838">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4ee15-2839">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2839">Include Cognitive Services module</span></span>
* <span data-ttu-id="4ee15-2840">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2840">Include Service Fabric module</span></span>
* <span data-ttu-id="4ee15-2841">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2841">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4ee15-2842">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2842">Add support for CDN commands</span></span>
* <span data-ttu-id="4ee15-2843">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2843">Remove Container module</span></span>
* <span data-ttu-id="4ee15-2844">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2844">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4ee15-2845">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2845">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4ee15-2846">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2846">Core</span></span>

* <span data-ttu-id="4ee15-2847">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2847">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4ee15-2848">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2848">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4ee15-2849">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2849">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4ee15-2850">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2850">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4ee15-2851">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2851">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4ee15-2852">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2852">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4ee15-2853">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2853">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4ee15-2854">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2854">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4ee15-2855">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2855">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4ee15-2856">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2856">core: Improved performance</span></span>
* <span data-ttu-id="4ee15-2857">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2857">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4ee15-2858">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2858">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2859">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2859">ACS</span></span>

* <span data-ttu-id="4ee15-2860">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2860">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4ee15-2861">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2861">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4ee15-2862">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2862">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4ee15-2863">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2863">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2864">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-2864">AppService</span></span>

* <span data-ttu-id="4ee15-2865">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2865">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4ee15-2866">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2866">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4ee15-2867">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2867">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4ee15-2868">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2868">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4ee15-2869">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2869">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4ee15-2870">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2870">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4ee15-2871">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2871">support slot swap with preview</span></span>
* <span data-ttu-id="4ee15-2872">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2872">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4ee15-2873">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2873">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4ee15-2874">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4ee15-2874">CosmosDB</span></span>

* <span data-ttu-id="4ee15-2875">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2875">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4ee15-2876">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2876">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4ee15-2877">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2877">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4ee15-2878">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2878">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4ee15-2879">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4ee15-2879">Data Lake Analytics</span></span>

* <span data-ttu-id="4ee15-2880">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2880">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4ee15-2881">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2881">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4ee15-2882">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2882">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4ee15-2883">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="4ee15-2883">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4ee15-2884">Таблица</span><span class="sxs-lookup"><span data-stu-id="4ee15-2884">Table</span></span>
  * <span data-ttu-id="4ee15-2885">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="4ee15-2885">Table valued function</span></span>
  * <span data-ttu-id="4ee15-2886">Просмотр</span><span class="sxs-lookup"><span data-stu-id="4ee15-2886">View</span></span>
  * <span data-ttu-id="4ee15-2887">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2887">Table Statistics.</span></span> <span data-ttu-id="4ee15-2888">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2888">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4ee15-2889">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4ee15-2889">Data Lake Store</span></span>

* <span data-ttu-id="4ee15-2890">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2890">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4ee15-2891">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2891">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4ee15-2892">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2892">missed help for access show.</span></span> <span data-ttu-id="4ee15-2893">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2893">adding it.</span></span> <span data-ttu-id="4ee15-2894">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4ee15-2894">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4ee15-2895">Поиск</span><span class="sxs-lookup"><span data-stu-id="4ee15-2895">Find</span></span>

* <span data-ttu-id="4ee15-2896">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2896">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4ee15-2897">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4ee15-2897">KeyVault</span></span>

* <span data-ttu-id="4ee15-2898">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2898">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4ee15-2899">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2899">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4ee15-2900">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2900">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4ee15-2901">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2901">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4ee15-2902">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2902">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4ee15-2903">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4ee15-2903">Lab</span></span>

* <span data-ttu-id="4ee15-2904">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2904">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4ee15-2905">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2905">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4ee15-2906">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2906">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4ee15-2907">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2907">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4ee15-2908">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2908">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4ee15-2909">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="4ee15-2909">Monitor</span></span>

* <span data-ttu-id="4ee15-2910">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2910">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4ee15-2911">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2911">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4ee15-2912">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-2912">Network</span></span>

* <span data-ttu-id="4ee15-2913">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2913">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4ee15-2914">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2914">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4ee15-2915">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2915">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4ee15-2916">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2916">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4ee15-2917">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2917">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4ee15-2918">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2918">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4ee15-2919">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2919">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4ee15-2920">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2920">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4ee15-2921">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2921">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4ee15-2922">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="4ee15-2922">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4ee15-2923">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2923">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4ee15-2924">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2924">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4ee15-2925">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2925">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4ee15-2926">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2926">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4ee15-2927">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2927">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4ee15-2928">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2928">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4ee15-2929">Профиль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2929">Profile</span></span>

* <span data-ttu-id="4ee15-2930">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2930">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4ee15-2931">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2931">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4ee15-2932">Redis</span><span class="sxs-lookup"><span data-stu-id="4ee15-2932">Redis</span></span>

* <span data-ttu-id="4ee15-2933">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2933">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4ee15-2934">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2934">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4ee15-2935">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4ee15-2935">Resource</span></span>

* <span data-ttu-id="4ee15-2936">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2936">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4ee15-2937">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2937">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4ee15-2938">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2938">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4ee15-2939">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2939">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4ee15-2940">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4ee15-2940">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4ee15-2941">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2941">Add docs for az lock update.</span></span> <span data-ttu-id="4ee15-2942">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4ee15-2942">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4ee15-2943">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2943">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4ee15-2944">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4ee15-2944">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4ee15-2945">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2945">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4ee15-2946">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4ee15-2946">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4ee15-2947">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2947">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4ee15-2948">Роль</span><span class="sxs-lookup"><span data-stu-id="4ee15-2948">Role</span></span>

* <span data-ttu-id="4ee15-2949">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2949">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4ee15-2950">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2950">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4ee15-2951">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2951">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4ee15-2952">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2952">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4ee15-2953">SQL</span><span class="sxs-lookup"><span data-stu-id="4ee15-2953">SQL</span></span>

* <span data-ttu-id="4ee15-2954">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2954">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4ee15-2955">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2955">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4ee15-2956">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-2956">Storage</span></span>

* <span data-ttu-id="4ee15-2957">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2957">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4ee15-2958">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2958">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4ee15-2959">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2959">Add support for large block blob upload</span></span>
* <span data-ttu-id="4ee15-2960">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2960">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-2961">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-2961">VM</span></span>

* <span data-ttu-id="4ee15-2962">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2962">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4ee15-2963">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="4ee15-2963">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4ee15-2964">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4ee15-2964">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4ee15-2965">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4ee15-2965">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4ee15-2966">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2966">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4ee15-2967">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2967">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4ee15-2968">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2968">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4ee15-2969">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2969">April 3, 2017</span></span>

<span data-ttu-id="4ee15-2970">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4ee15-2970">Version 2.0.2</span></span>

<span data-ttu-id="4ee15-2971">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2971">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4ee15-2972">Core</span><span class="sxs-lookup"><span data-stu-id="4ee15-2972">Core</span></span>

* <span data-ttu-id="4ee15-2973">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2973">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4ee15-2974">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2974">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4ee15-2975">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2975">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4ee15-2976">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2976">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4ee15-2977">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2977">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4ee15-2978">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="4ee15-2978">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4ee15-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2979">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4ee15-2980">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2980">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4ee15-2981">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2981">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4ee15-2982">ACS</span><span class="sxs-lookup"><span data-stu-id="4ee15-2982">ACS</span></span>

* <span data-ttu-id="4ee15-2983">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2983">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4ee15-2984">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="4ee15-2984">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4ee15-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2985">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4ee15-2986">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="4ee15-2986">Add support for windows clusters.</span></span> <span data-ttu-id="4ee15-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2987">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4ee15-2988">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="4ee15-2988">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4ee15-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2989">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4ee15-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="4ee15-2990">AppService</span></span>

* <span data-ttu-id="4ee15-2991">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2991">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4ee15-2992">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2992">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4ee15-2993">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2993">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4ee15-2994">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2994">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4ee15-2995">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4ee15-2995">DataLake</span></span>

* <span data-ttu-id="4ee15-2996">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2996">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4ee15-2997">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4ee15-2997">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4ee15-2998">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4ee15-2998">DocuemntDB</span></span>

* <span data-ttu-id="4ee15-2999">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-2999">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4ee15-3000">ВМ</span><span class="sxs-lookup"><span data-stu-id="4ee15-3000">VM</span></span>

* <span data-ttu-id="4ee15-3001">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3001">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4ee15-3002">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3002">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4ee15-3003">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3003">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4ee15-3004">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3004">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4ee15-3005">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3005">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4ee15-3006">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3006">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="4ee15-3007">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3007">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4ee15-3008">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3008">February 27, 2017</span></span>

<span data-ttu-id="4ee15-3009">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4ee15-3009">Version 2.0.0</span></span>

<span data-ttu-id="4ee15-3010">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="4ee15-3010">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4ee15-3011">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="4ee15-3011">Container Service (acs)</span></span>
- <span data-ttu-id="4ee15-3012">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="4ee15-3012">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4ee15-3013">Сеть</span><span class="sxs-lookup"><span data-stu-id="4ee15-3013">Networking</span></span>
- <span data-ttu-id="4ee15-3014">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4ee15-3014">Storage</span></span>

<span data-ttu-id="4ee15-3015">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3015">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4ee15-3016">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3016">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4ee15-3017">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3017">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4ee15-3018">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3018">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4ee15-3019">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4ee15-3019">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4ee15-3020">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="4ee15-3020">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4ee15-3021">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="4ee15-3021">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4ee15-3022">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="4ee15-3022">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4ee15-3023">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4ee15-3023">Provide feedback from the command line with the `az feedback` command</span></span>

