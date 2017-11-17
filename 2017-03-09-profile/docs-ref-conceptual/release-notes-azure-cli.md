---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
keywords: "Azure CLI 2.0, заметки о выпуске"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: e893b99349bbf2a5eec8af254158eb07001f1da7
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="6cfcd-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="6cfcd-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="6cfcd-105">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-105">August 28, 2017</span></span>

<span data-ttu-id="6cfcd-106">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="6cfcd-106">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="6cfcd-107">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="6cfcd-107">CLI</span></span>

* <span data-ttu-id="6cfcd-108">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-108">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="6cfcd-109">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-109">ACS</span></span>

* <span data-ttu-id="6cfcd-110">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-110">Corrected preview regions.</span></span>
* <span data-ttu-id="6cfcd-111">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-111">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="6cfcd-112">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-112">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="6cfcd-113">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="6cfcd-113">Appservice</span></span>

* <span data-ttu-id="6cfcd-114">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-114">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="6cfcd-115">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-115">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="6cfcd-116">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-116">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="6cfcd-117">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-117">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="6cfcd-118">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-118">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="6cfcd-119">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="6cfcd-119">IoT</span></span>

* <span data-ttu-id="6cfcd-120">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-120">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="6cfcd-121">Сеть</span><span class="sxs-lookup"><span data-stu-id="6cfcd-121">Network</span></span>

* <span data-ttu-id="6cfcd-122">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-122">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6cfcd-123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-123">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="6cfcd-124">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-124">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6cfcd-125">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6cfcd-126">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-126">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="6cfcd-127">Профиль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-127">Profile</span></span>

* <span data-ttu-id="6cfcd-128">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-128">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6cfcd-129">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6cfcd-129">Service Fabric</span></span>

* <span data-ttu-id="6cfcd-130">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-130">Preview release</span></span>
* <span data-ttu-id="6cfcd-131">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-131">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="6cfcd-132">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-132">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="6cfcd-133">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-133">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="6cfcd-134">Хранилище</span><span class="sxs-lookup"><span data-stu-id="6cfcd-134">Storage</span></span>

* <span data-ttu-id="6cfcd-135">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-135">Enabled setting blob tier</span></span>
* <span data-ttu-id="6cfcd-136">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-136">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="6cfcd-137">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-137">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="6cfcd-138">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-138">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="6cfcd-139">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-139">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="6cfcd-140">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-140">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="6cfcd-141">ВМ</span><span class="sxs-lookup"><span data-stu-id="6cfcd-141">VM</span></span>

* <span data-ttu-id="6cfcd-142">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-142">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="6cfcd-143">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-143">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="6cfcd-144">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-144">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="6cfcd-145">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-145">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="6cfcd-146">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-146">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="6cfcd-147">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-147">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="6cfcd-148">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-148">August 15, 2017</span></span>

<span data-ttu-id="6cfcd-149">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="6cfcd-149">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="6cfcd-150">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-150">ACS</span></span>

* <span data-ttu-id="6cfcd-151">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-151">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="6cfcd-152">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="6cfcd-152">Appservice</span></span>

* <span data-ttu-id="6cfcd-153">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-153">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="6cfcd-154">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="6cfcd-154">Event Grid</span></span>

* <span data-ttu-id="6cfcd-155">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-155">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="6cfcd-156">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-156">August 11, 2017</span></span>

<span data-ttu-id="6cfcd-157">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="6cfcd-157">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="6cfcd-158">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-158">ACS</span></span>

* <span data-ttu-id="6cfcd-159">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-159">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="6cfcd-160">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="6cfcd-160">Batch</span></span>

* <span data-ttu-id="6cfcd-161">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-161">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="6cfcd-162">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-162">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="6cfcd-163">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-163">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="6cfcd-164">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-164">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="6cfcd-165">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-165">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="6cfcd-166">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-166">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="6cfcd-167">Компонент</span><span class="sxs-lookup"><span data-stu-id="6cfcd-167">Component</span></span>

* <span data-ttu-id="6cfcd-168">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-168">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="6cfcd-169">Контейнер</span><span class="sxs-lookup"><span data-stu-id="6cfcd-169">Container</span></span>

* <span data-ttu-id="6cfcd-170">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-170">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="6cfcd-171">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6cfcd-171">Data Lake Store</span></span>

* <span data-ttu-id="6cfcd-172">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-172">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="6cfcd-173">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="6cfcd-173">Event Grid</span></span>

* <span data-ttu-id="6cfcd-174">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="6cfcd-174">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="6cfcd-175">Сеть</span><span class="sxs-lookup"><span data-stu-id="6cfcd-175">Network</span></span>

* <span data-ttu-id="6cfcd-176">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-176">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="6cfcd-177">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-177">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="6cfcd-178">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-178">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="6cfcd-179">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-179">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="6cfcd-180">Профиль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-180">Profile</span></span>

* <span data-ttu-id="6cfcd-181">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-181">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="6cfcd-182">Хранилище</span><span class="sxs-lookup"><span data-stu-id="6cfcd-182">Storage</span></span>

* <span data-ttu-id="6cfcd-183">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-183">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="6cfcd-184">ВМ</span><span class="sxs-lookup"><span data-stu-id="6cfcd-184">VM</span></span>

* <span data-ttu-id="6cfcd-185">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-185">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="6cfcd-186">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-186">Exposed `list-skus` command</span></span>
* <span data-ttu-id="6cfcd-187">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-187">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="6cfcd-188">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-188">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="6cfcd-189">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-189">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="6cfcd-190">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-190">July 28, 2017</span></span>

<span data-ttu-id="6cfcd-191">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="6cfcd-191">Version 2.0.12</span></span>

* <span data-ttu-id="6cfcd-192">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-192">Added container commands</span></span>
* <span data-ttu-id="6cfcd-193">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-193">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="6cfcd-194">Core</span><span class="sxs-lookup"><span data-stu-id="6cfcd-194">Core</span></span>

* <span data-ttu-id="6cfcd-195">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-195">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="6cfcd-196">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-196">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="6cfcd-197">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-197">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="6cfcd-198">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-198">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="6cfcd-199">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-199">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="6cfcd-200">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-200">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="6cfcd-201">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-201">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6cfcd-202">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-202">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="6cfcd-203">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-203">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="6cfcd-204">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-204">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="6cfcd-205">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-205">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="6cfcd-206">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-206">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="6cfcd-207">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-207">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="6cfcd-208">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-208">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="6cfcd-209">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-209">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="6cfcd-210">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-210">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="6cfcd-211">ACR</span><span class="sxs-lookup"><span data-stu-id="6cfcd-211">ACR</span></span>

* <span data-ttu-id="6cfcd-212">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-212">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="6cfcd-213">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-213">Support SKU update for managed registries</span></span>
* <span data-ttu-id="6cfcd-214">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-214">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="6cfcd-215">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-215">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="6cfcd-216">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-216">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="6cfcd-217">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-217">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="6cfcd-218">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-218">ACS</span></span>

* <span data-ttu-id="6cfcd-219">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-219">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="6cfcd-220">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="6cfcd-220">Appservice</span></span>

* <span data-ttu-id="6cfcd-221">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-221">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="6cfcd-222">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-222">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="6cfcd-223">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-223">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="6cfcd-224">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-224">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="6cfcd-225">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-225">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="6cfcd-226">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-226">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="6cfcd-227">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-227">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="6cfcd-228">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-228">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="6cfcd-229">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-229">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="6cfcd-230">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-230">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="6cfcd-231">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="6cfcd-231">Batch</span></span>

* <span data-ttu-id="6cfcd-232">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-232">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="6cfcd-233">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-233">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="6cfcd-234">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-234">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="6cfcd-235">CDN</span><span class="sxs-lookup"><span data-stu-id="6cfcd-235">CDN</span></span>

* <span data-ttu-id="6cfcd-236">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-236">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="6cfcd-237">Облако</span><span class="sxs-lookup"><span data-stu-id="6cfcd-237">Cloud</span></span>

* <span data-ttu-id="6cfcd-238">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-238">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="6cfcd-239">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-239">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="6cfcd-240">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-240">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="6cfcd-241">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-241">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="6cfcd-242">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-242">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6cfcd-243">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6cfcd-243">CosmosDB</span></span>

* <span data-ttu-id="6cfcd-244">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-244">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="6cfcd-245">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-245">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6cfcd-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6cfcd-246">Data Lake Analytics</span></span>

* <span data-ttu-id="6cfcd-247">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-247">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="6cfcd-248">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-248">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="6cfcd-249">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-249">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6cfcd-250">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6cfcd-250">Data Lake Store</span></span>

* <span data-ttu-id="6cfcd-251">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-251">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="6cfcd-252">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-252">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="6cfcd-253">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-253">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="6cfcd-254">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-254">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="6cfcd-255">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="6cfcd-255">Interactive</span></span>

* <span data-ttu-id="6cfcd-256">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-256">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="6cfcd-257">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-257">Increased test coverage</span></span>
* <span data-ttu-id="6cfcd-258">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-258">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="6cfcd-259">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-259">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="6cfcd-260">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-260">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="6cfcd-261">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-261">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="6cfcd-262">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-262">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6cfcd-263">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-263">Added `--progress` flag</span></span>
* <span data-ttu-id="6cfcd-264">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-264">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="6cfcd-265">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-265">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="6cfcd-266">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="6cfcd-266">IoT</span></span>

* <span data-ttu-id="6cfcd-267">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="6cfcd-267">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="6cfcd-268">(3934).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-268">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="6cfcd-269">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="6cfcd-269">Key vault</span></span>

* <span data-ttu-id="6cfcd-270">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="6cfcd-270">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="6cfcd-271">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-271">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="6cfcd-272">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-272">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6cfcd-273">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-273">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6cfcd-274">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-274">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="6cfcd-275">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-275">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="6cfcd-276">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="6cfcd-276">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="6cfcd-277">(3307).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-277">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="6cfcd-278">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="6cfcd-278">Lab</span></span>

* <span data-ttu-id="6cfcd-279">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-279">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="6cfcd-280">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-280">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="6cfcd-281">Монитор</span><span class="sxs-lookup"><span data-stu-id="6cfcd-281">Monitor</span></span>

* <span data-ttu-id="6cfcd-282">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-282">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="6cfcd-283">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-283">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="6cfcd-284">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-284">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="6cfcd-285">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-285">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="6cfcd-286">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-286">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="6cfcd-287">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="6cfcd-287">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="6cfcd-288">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-288">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="6cfcd-289">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-289">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="6cfcd-290">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-290">`location` no longer required</span></span>
  * <span data-ttu-id="6cfcd-291">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-291">Add name and ID support for target</span></span>
  * <span data-ttu-id="6cfcd-292">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-292">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="6cfcd-293">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-293">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="6cfcd-294">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-294">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="6cfcd-295">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-295">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="6cfcd-296">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-296">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="6cfcd-297">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-297">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="6cfcd-298">Сеть</span><span class="sxs-lookup"><span data-stu-id="6cfcd-298">Network</span></span>

* <span data-ttu-id="6cfcd-299">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-299">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="6cfcd-300">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-300">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="6cfcd-301">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-301">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="6cfcd-302">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-302">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="6cfcd-303">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-303">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="6cfcd-304">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-304">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="6cfcd-305">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-305">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="6cfcd-306">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-306">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="6cfcd-307">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-307">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="6cfcd-308">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-308">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="6cfcd-309">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-309">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="6cfcd-310">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-310">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="6cfcd-311">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-311">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="6cfcd-312">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-312">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="6cfcd-313">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-313">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="6cfcd-314">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-314">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="6cfcd-315">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-315">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="6cfcd-316">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-316">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="6cfcd-317">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-317">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="6cfcd-318">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-318">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="6cfcd-319">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-319">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="6cfcd-320">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-320">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="6cfcd-321">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-321">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="6cfcd-322">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-322">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="6cfcd-323">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-323">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="6cfcd-324">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-324">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="6cfcd-325">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-325">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="6cfcd-326">Профиль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-326">Profile</span></span>

* <span data-ttu-id="6cfcd-327">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-327">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="6cfcd-328">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-328">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="6cfcd-329">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-329">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="6cfcd-330">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-330">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="6cfcd-331">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-331">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="6cfcd-332">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="6cfcd-332">RDBMS</span></span>

* <span data-ttu-id="6cfcd-333">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-333">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="6cfcd-334">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-334">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="6cfcd-335">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-335">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="6cfcd-336">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-336">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="6cfcd-337">Ресурс</span><span class="sxs-lookup"><span data-stu-id="6cfcd-337">Resource</span></span>

* <span data-ttu-id="6cfcd-338">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-338">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="6cfcd-339">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-339">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="6cfcd-340">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-340">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="6cfcd-341">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-341">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="6cfcd-342">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-342">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="6cfcd-343">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-343">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="6cfcd-344">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-344">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="6cfcd-345">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-345">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="6cfcd-346">Роль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-346">Role</span></span>

* <span data-ttu-id="6cfcd-347">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-347">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="6cfcd-348">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-348">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="6cfcd-349">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-349">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="6cfcd-350">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-350">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="6cfcd-351">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-351">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6cfcd-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6cfcd-352">Service Fabric</span></span>
* <span data-ttu-id="6cfcd-353">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-353">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="6cfcd-354">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-354">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="6cfcd-355">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-355">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="6cfcd-356">SQL</span><span class="sxs-lookup"><span data-stu-id="6cfcd-356">SQL</span></span>

* <span data-ttu-id="6cfcd-357">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-357">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="6cfcd-358">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-358">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="6cfcd-359">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-359">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="6cfcd-360">Хранилище</span><span class="sxs-lookup"><span data-stu-id="6cfcd-360">Storage</span></span>

* <span data-ttu-id="6cfcd-361">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-361">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="6cfcd-362">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-362">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="6cfcd-363">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-363">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="6cfcd-364">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="6cfcd-364">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="6cfcd-365">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-365">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="6cfcd-366">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-366">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="6cfcd-367">ВМ</span><span class="sxs-lookup"><span data-stu-id="6cfcd-367">VM</span></span>

* <span data-ttu-id="6cfcd-368">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-368">Support configuring nsg</span></span>
* <span data-ttu-id="6cfcd-369">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-369">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="6cfcd-370">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-370">Support managed service identities</span></span>
* <span data-ttu-id="6cfcd-371">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-371">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="6cfcd-372">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-372">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="6cfcd-373">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-373">May 10, 2017</span></span>

<span data-ttu-id="6cfcd-374">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="6cfcd-374">Version 2.0.6</span></span>

* <span data-ttu-id="6cfcd-375">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-375">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="6cfcd-376">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-376">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="6cfcd-377">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-377">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="6cfcd-378">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-378">Include Cognitive Services module.</span></span>
* <span data-ttu-id="6cfcd-379">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-379">Include Service Fabric module.</span></span>
* <span data-ttu-id="6cfcd-380">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-380">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="6cfcd-381">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-381">Add support for CDN commands.</span></span>
* <span data-ttu-id="6cfcd-382">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-382">Remove Container module.</span></span>
* <span data-ttu-id="6cfcd-383">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-383">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="6cfcd-384">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-384">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="6cfcd-385">Core</span><span class="sxs-lookup"><span data-stu-id="6cfcd-385">Core</span></span>

* <span data-ttu-id="6cfcd-386">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-386">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="6cfcd-387">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-387">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="6cfcd-388">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-388">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="6cfcd-389">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-389">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="6cfcd-390">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-390">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="6cfcd-391">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-391">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="6cfcd-392">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-392">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="6cfcd-393">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-393">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="6cfcd-394">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-394">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="6cfcd-395">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-395">core: Improved performance</span></span>
* <span data-ttu-id="6cfcd-396">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-396">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="6cfcd-397">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-397">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="6cfcd-398">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-398">ACS</span></span>

* <span data-ttu-id="6cfcd-399">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-399">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="6cfcd-400">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-400">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="6cfcd-401">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-401">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="6cfcd-402">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-402">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="6cfcd-403">AppService</span><span class="sxs-lookup"><span data-stu-id="6cfcd-403">AppService</span></span>

* <span data-ttu-id="6cfcd-404">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-404">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="6cfcd-405">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-405">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="6cfcd-406">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-406">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="6cfcd-407">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-407">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="6cfcd-408">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-408">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="6cfcd-409">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-409">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="6cfcd-410">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-410">support slot swap with preview</span></span>
* <span data-ttu-id="6cfcd-411">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-411">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="6cfcd-412">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-412">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6cfcd-413">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6cfcd-413">CosmosDB</span></span>

* <span data-ttu-id="6cfcd-414">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-414">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="6cfcd-415">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-415">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="6cfcd-416">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-416">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="6cfcd-417">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-417">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6cfcd-418">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="6cfcd-418">Data Lake Analytics</span></span>

* <span data-ttu-id="6cfcd-419">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-419">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="6cfcd-420">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-420">Add support for new catalog item type: package.</span></span> <span data-ttu-id="6cfcd-421">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-421">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="6cfcd-422">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="6cfcd-422">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="6cfcd-423">Таблица</span><span class="sxs-lookup"><span data-stu-id="6cfcd-423">Table</span></span>
  * <span data-ttu-id="6cfcd-424">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="6cfcd-424">Table valued function</span></span>
  * <span data-ttu-id="6cfcd-425">Просмотр</span><span class="sxs-lookup"><span data-stu-id="6cfcd-425">View</span></span>
  * <span data-ttu-id="6cfcd-426">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-426">Table Statistics.</span></span> <span data-ttu-id="6cfcd-427">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-427">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6cfcd-428">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="6cfcd-428">Data Lake Store</span></span>

* <span data-ttu-id="6cfcd-429">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-429">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="6cfcd-430">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-430">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="6cfcd-431">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-431">missed help for access show.</span></span> <span data-ttu-id="6cfcd-432">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-432">adding it.</span></span> <span data-ttu-id="6cfcd-433">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="6cfcd-433">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="6cfcd-434">Поиск</span><span class="sxs-lookup"><span data-stu-id="6cfcd-434">Find</span></span>

* <span data-ttu-id="6cfcd-435">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-435">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="6cfcd-436">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="6cfcd-436">KeyVault</span></span>

* <span data-ttu-id="6cfcd-437">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-437">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="6cfcd-438">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-438">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="6cfcd-439">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-439">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="6cfcd-440">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-440">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="6cfcd-441">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-441">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="6cfcd-442">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="6cfcd-442">Lab</span></span>

* <span data-ttu-id="6cfcd-443">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-443">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="6cfcd-444">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-444">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="6cfcd-445">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-445">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="6cfcd-446">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-446">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="6cfcd-447">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-447">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="6cfcd-448">Монитор</span><span class="sxs-lookup"><span data-stu-id="6cfcd-448">Monitor</span></span>

* <span data-ttu-id="6cfcd-449">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-449">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="6cfcd-450">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-450">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="6cfcd-451">Сеть</span><span class="sxs-lookup"><span data-stu-id="6cfcd-451">Network</span></span>

* <span data-ttu-id="6cfcd-452">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-452">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="6cfcd-453">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-453">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="6cfcd-454">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-454">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="6cfcd-455">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-455">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="6cfcd-456">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-456">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="6cfcd-457">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-457">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="6cfcd-458">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-458">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="6cfcd-459">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-459">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="6cfcd-460">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-460">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="6cfcd-461">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="6cfcd-461">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="6cfcd-462">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-462">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="6cfcd-463">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-463">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="6cfcd-464">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-464">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="6cfcd-465">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-465">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="6cfcd-466">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-466">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="6cfcd-467">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-467">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="6cfcd-468">Профиль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-468">Profile</span></span>

* <span data-ttu-id="6cfcd-469">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-469">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="6cfcd-470">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-470">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="6cfcd-471">Redis</span><span class="sxs-lookup"><span data-stu-id="6cfcd-471">Redis</span></span>

* <span data-ttu-id="6cfcd-472">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-472">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="6cfcd-473">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-473">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="6cfcd-474">Ресурс</span><span class="sxs-lookup"><span data-stu-id="6cfcd-474">Resource</span></span>

* <span data-ttu-id="6cfcd-475">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-475">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="6cfcd-476">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-476">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="6cfcd-477">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-477">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="6cfcd-478">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-478">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="6cfcd-479">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="6cfcd-479">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="6cfcd-480">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-480">Add docs for az lock update.</span></span> <span data-ttu-id="6cfcd-481">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="6cfcd-481">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="6cfcd-482">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-482">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="6cfcd-483">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="6cfcd-483">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="6cfcd-484">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-484">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="6cfcd-485">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="6cfcd-485">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="6cfcd-486">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-486">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="6cfcd-487">Роль</span><span class="sxs-lookup"><span data-stu-id="6cfcd-487">Role</span></span>

* <span data-ttu-id="6cfcd-488">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-488">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="6cfcd-489">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-489">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="6cfcd-490">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-490">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="6cfcd-491">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-491">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="6cfcd-492">SQL</span><span class="sxs-lookup"><span data-stu-id="6cfcd-492">SQL</span></span>

* <span data-ttu-id="6cfcd-493">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-493">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="6cfcd-494">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-494">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="6cfcd-495">Хранилище</span><span class="sxs-lookup"><span data-stu-id="6cfcd-495">Storage</span></span>

* <span data-ttu-id="6cfcd-496">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-496">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="6cfcd-497">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-497">Add support for incremental blob copy</span></span>
* <span data-ttu-id="6cfcd-498">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-498">Add support for large block blob upload</span></span>
* <span data-ttu-id="6cfcd-499">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-499">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="6cfcd-500">ВМ</span><span class="sxs-lookup"><span data-stu-id="6cfcd-500">VM</span></span>

* <span data-ttu-id="6cfcd-501">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-501">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="6cfcd-502">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="6cfcd-502">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="6cfcd-503">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="6cfcd-503">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="6cfcd-504">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="6cfcd-504">az vm/vmss disk</span></span>
  3. <span data-ttu-id="6cfcd-505">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-505">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="6cfcd-506">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-506">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="6cfcd-507">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-507">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="6cfcd-508">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-508">April 3, 2017</span></span>

<span data-ttu-id="6cfcd-509">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="6cfcd-509">Version 2.0.2</span></span>

<span data-ttu-id="6cfcd-510">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-510">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="6cfcd-511">Core</span><span class="sxs-lookup"><span data-stu-id="6cfcd-511">Core</span></span>

* <span data-ttu-id="6cfcd-512">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-512">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="6cfcd-513">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-513">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="6cfcd-514">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-514">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="6cfcd-515">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-515">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6cfcd-516">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-516">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="6cfcd-517">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="6cfcd-517">Add prompting for missing template parameters.</span></span> <span data-ttu-id="6cfcd-518">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-518">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="6cfcd-519">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-519">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="6cfcd-520">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-520">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="6cfcd-521">ACS</span><span class="sxs-lookup"><span data-stu-id="6cfcd-521">ACS</span></span>

* <span data-ttu-id="6cfcd-522">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-522">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="6cfcd-523">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="6cfcd-523">Add support for ssh key password prompting.</span></span> <span data-ttu-id="6cfcd-524">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-524">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="6cfcd-525">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="6cfcd-525">Add support for windows clusters.</span></span> <span data-ttu-id="6cfcd-526">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-526">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="6cfcd-527">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="6cfcd-527">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="6cfcd-528">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-528">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="6cfcd-529">AppService</span><span class="sxs-lookup"><span data-stu-id="6cfcd-529">AppService</span></span>

* <span data-ttu-id="6cfcd-530">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-530">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="6cfcd-531">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-531">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="6cfcd-532">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-532">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="6cfcd-533">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-533">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="6cfcd-534">DataLake</span><span class="sxs-lookup"><span data-stu-id="6cfcd-534">DataLake</span></span>

* <span data-ttu-id="6cfcd-535">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-535">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="6cfcd-536">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-536">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="6cfcd-537">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="6cfcd-537">DocuemntDB</span></span>

* <span data-ttu-id="6cfcd-538">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-538">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="6cfcd-539">ВМ</span><span class="sxs-lookup"><span data-stu-id="6cfcd-539">VM</span></span>

* <span data-ttu-id="6cfcd-540">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-540">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="6cfcd-541">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-541">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="6cfcd-542">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-542">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="6cfcd-543">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-543">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6cfcd-544">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-544">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="6cfcd-545">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-545">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="6cfcd-546">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-546">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="6cfcd-547">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-547">February 27, 2017</span></span>

<span data-ttu-id="6cfcd-548">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="6cfcd-548">Version 2.0.0</span></span>

<span data-ttu-id="6cfcd-549">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-549">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="6cfcd-550">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="6cfcd-550">General availability applies to these command modules:</span></span>
- <span data-ttu-id="6cfcd-551">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="6cfcd-551">Container Service (acs)</span></span>
- <span data-ttu-id="6cfcd-552">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="6cfcd-552">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="6cfcd-553">Сеть</span><span class="sxs-lookup"><span data-stu-id="6cfcd-553">Networking</span></span>
- <span data-ttu-id="6cfcd-554">Хранилище</span><span class="sxs-lookup"><span data-stu-id="6cfcd-554">Storage</span></span>

<span data-ttu-id="6cfcd-555">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-555">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="6cfcd-556">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-556">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="6cfcd-557">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-557">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="6cfcd-558">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-558">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="6cfcd-559">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-559">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="6cfcd-560">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-560">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="6cfcd-561">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-561">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="6cfcd-562">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-562">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="6cfcd-563">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-563">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="6cfcd-564">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="6cfcd-564">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="6cfcd-565">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="6cfcd-565">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="6cfcd-566">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="6cfcd-566">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="6cfcd-567">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="6cfcd-567">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="6cfcd-568">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="6cfcd-568">Provide feedback from the command line with the `az feedback` command.</span></span>

