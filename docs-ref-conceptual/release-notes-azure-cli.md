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
ms.openlocfilehash: 39e4710a29ac57730919b82ab76b9c9a4b9ca786
ms.sourcegitcommit: 43d4f838d132ab9bcfa59dbda3b544c06373b6a9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ab16c-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ab16c-104">Azure CLI 2.0 release notes</span></span>

## <a name="august-15-2017"></a><span data-ttu-id="ab16c-105">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-105">August 15, 2017</span></span>

<span data-ttu-id="ab16c-106">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ab16c-106">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ab16c-107">ACS</span><span class="sxs-lookup"><span data-stu-id="ab16c-107">ACS</span></span>

* <span data-ttu-id="ab16c-108">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ab16c-108">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ab16c-109">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ab16c-109">Appservice</span></span>

* <span data-ttu-id="ab16c-110">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="ab16c-110">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ab16c-111">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="ab16c-111">Event Grid</span></span>

* <span data-ttu-id="ab16c-112">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ab16c-112">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ab16c-113">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-113">August 11, 2017</span></span>

<span data-ttu-id="ab16c-114">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ab16c-114">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ab16c-115">ACS</span><span class="sxs-lookup"><span data-stu-id="ab16c-115">ACS</span></span>

* <span data-ttu-id="ab16c-116">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ab16c-116">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ab16c-117">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="ab16c-117">Batch</span></span>

* <span data-ttu-id="ab16c-118">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ab16c-118">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ab16c-119">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="ab16c-119">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ab16c-120">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ab16c-120">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ab16c-121">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="ab16c-121">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ab16c-122">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="ab16c-122">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ab16c-123">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-123">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ab16c-124">Компонент</span><span class="sxs-lookup"><span data-stu-id="ab16c-124">Component</span></span>

* <span data-ttu-id="ab16c-125">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="ab16c-125">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ab16c-126">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ab16c-126">Container</span></span>

* <span data-ttu-id="ab16c-127">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="ab16c-127">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ab16c-128">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ab16c-128">Data Lake Store</span></span>

* <span data-ttu-id="ab16c-129">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="ab16c-129">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ab16c-130">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="ab16c-130">Event Grid</span></span>

* <span data-ttu-id="ab16c-131">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ab16c-131">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ab16c-132">Сеть</span><span class="sxs-lookup"><span data-stu-id="ab16c-132">Network</span></span>

* <span data-ttu-id="ab16c-133">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="ab16c-133">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ab16c-134">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-134">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ab16c-135">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-135">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ab16c-136">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-136">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ab16c-137">Профиль</span><span class="sxs-lookup"><span data-stu-id="ab16c-137">Profile</span></span>

* <span data-ttu-id="ab16c-138">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="ab16c-138">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ab16c-139">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ab16c-139">Storage</span></span>

* <span data-ttu-id="ab16c-140">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ab16c-140">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ab16c-141">ВМ</span><span class="sxs-lookup"><span data-stu-id="ab16c-141">VM</span></span>

* <span data-ttu-id="ab16c-142">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="ab16c-142">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ab16c-143">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-143">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ab16c-144">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="ab16c-144">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ab16c-145">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="ab16c-145">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ab16c-146">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ab16c-146">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ab16c-147">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-147">July 28, 2017</span></span>

<span data-ttu-id="ab16c-148">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ab16c-148">Version 2.0.12</span></span>

* <span data-ttu-id="ab16c-149">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ab16c-149">Added container commands</span></span>
* <span data-ttu-id="ab16c-150">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ab16c-150">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ab16c-151">Core</span><span class="sxs-lookup"><span data-stu-id="ab16c-151">Core</span></span>

* <span data-ttu-id="ab16c-152">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ab16c-152">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ab16c-153">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ab16c-153">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ab16c-154">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ab16c-154">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ab16c-155">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="ab16c-155">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ab16c-156">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="ab16c-156">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ab16c-157">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="ab16c-157">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ab16c-158">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ab16c-158">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ab16c-159">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="ab16c-159">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ab16c-160">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="ab16c-160">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ab16c-161">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="ab16c-161">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ab16c-162">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="ab16c-162">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ab16c-163">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="ab16c-163">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ab16c-164">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ab16c-164">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ab16c-165">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ab16c-165">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ab16c-166">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ab16c-166">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ab16c-167">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="ab16c-167">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ab16c-168">ACR</span><span class="sxs-lookup"><span data-stu-id="ab16c-168">ACR</span></span>

* <span data-ttu-id="ab16c-169">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ab16c-169">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ab16c-170">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ab16c-170">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ab16c-171">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="ab16c-171">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ab16c-172">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ab16c-172">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ab16c-173">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="ab16c-173">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ab16c-174">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="ab16c-174">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ab16c-175">ACS</span><span class="sxs-lookup"><span data-stu-id="ab16c-175">ACS</span></span>

* <span data-ttu-id="ab16c-176">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ab16c-176">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ab16c-177">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ab16c-177">Appservice</span></span>

* <span data-ttu-id="ab16c-178">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="ab16c-178">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ab16c-179">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="ab16c-179">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ab16c-180">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-180">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ab16c-181">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="ab16c-181">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ab16c-182">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="ab16c-182">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ab16c-183">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="ab16c-183">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ab16c-184">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="ab16c-184">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ab16c-185">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="ab16c-185">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ab16c-186">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="ab16c-186">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ab16c-187">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-187">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ab16c-188">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="ab16c-188">Batch</span></span>

* <span data-ttu-id="ab16c-189">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="ab16c-189">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ab16c-190">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-190">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ab16c-191">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-191">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ab16c-192">CDN</span><span class="sxs-lookup"><span data-stu-id="ab16c-192">CDN</span></span>

* <span data-ttu-id="ab16c-193">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="ab16c-193">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="ab16c-194">Облако</span><span class="sxs-lookup"><span data-stu-id="ab16c-194">Cloud</span></span>

* <span data-ttu-id="ab16c-195">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ab16c-195">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ab16c-196">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="ab16c-196">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ab16c-197">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="ab16c-197">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ab16c-198">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ab16c-198">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ab16c-199">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-199">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ab16c-200">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ab16c-200">CosmosDB</span></span>

* <span data-ttu-id="ab16c-201">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="ab16c-201">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ab16c-202">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="ab16c-202">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ab16c-203">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ab16c-203">Data Lake Analytics</span></span>

* <span data-ttu-id="ab16c-204">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-204">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ab16c-205">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-205">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ab16c-206">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-206">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ab16c-207">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ab16c-207">Data Lake Store</span></span>

* <span data-ttu-id="ab16c-208">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-208">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ab16c-209">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="ab16c-209">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ab16c-210">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-210">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ab16c-211">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ab16c-211">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ab16c-212">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="ab16c-212">Interactive</span></span>

* <span data-ttu-id="ab16c-213">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="ab16c-213">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ab16c-214">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="ab16c-214">Increased test coverage</span></span>
* <span data-ttu-id="ab16c-215">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="ab16c-215">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ab16c-216">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="ab16c-216">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ab16c-217">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="ab16c-217">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ab16c-218">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="ab16c-218">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ab16c-219">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ab16c-219">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ab16c-220">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-220">Added `--progress` flag</span></span>
* <span data-ttu-id="ab16c-221">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-221">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ab16c-222">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="ab16c-222">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ab16c-223">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ab16c-223">IoT</span></span>

* <span data-ttu-id="ab16c-224">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="ab16c-224">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ab16c-225">(3934).</span><span class="sxs-lookup"><span data-stu-id="ab16c-225">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ab16c-226">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ab16c-226">Key vault</span></span>

* <span data-ttu-id="ab16c-227">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="ab16c-227">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ab16c-228">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ab16c-228">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ab16c-229">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ab16c-229">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ab16c-230">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ab16c-230">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ab16c-231">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-231">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ab16c-232">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="ab16c-232">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ab16c-233">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ab16c-233">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ab16c-234">(3307).</span><span class="sxs-lookup"><span data-stu-id="ab16c-234">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ab16c-235">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ab16c-235">Lab</span></span>

* <span data-ttu-id="ab16c-236">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-236">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ab16c-237">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-237">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ab16c-238">Монитор</span><span class="sxs-lookup"><span data-stu-id="ab16c-238">Monitor</span></span>

* <span data-ttu-id="ab16c-239">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="ab16c-239">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ab16c-240">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-240">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ab16c-241">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-241">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ab16c-242">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-242">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ab16c-243">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-243">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ab16c-244">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="ab16c-244">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ab16c-245">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="ab16c-245">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ab16c-246">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="ab16c-246">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ab16c-247">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ab16c-247">`location` no longer required</span></span>
  * <span data-ttu-id="ab16c-248">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="ab16c-248">Add name and ID support for target</span></span>
  * <span data-ttu-id="ab16c-249">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="ab16c-249">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ab16c-250">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ab16c-250">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ab16c-251">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="ab16c-251">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ab16c-252">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="ab16c-252">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ab16c-253">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-253">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ab16c-254">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-254">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ab16c-255">Сеть</span><span class="sxs-lookup"><span data-stu-id="ab16c-255">Network</span></span>

* <span data-ttu-id="ab16c-256">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-256">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ab16c-257">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-257">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ab16c-258">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ab16c-258">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ab16c-259">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-259">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ab16c-260">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-260">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ab16c-261">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-261">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ab16c-262">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-262">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ab16c-263">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-263">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ab16c-264">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-264">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ab16c-265">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-265">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ab16c-266">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-266">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ab16c-267">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-267">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ab16c-268">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-268">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ab16c-269">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-269">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ab16c-270">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-270">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ab16c-271">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-271">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ab16c-272">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ab16c-272">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ab16c-273">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-273">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ab16c-274">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-274">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ab16c-275">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-275">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ab16c-276">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-276">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ab16c-277">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-277">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ab16c-278">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-278">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ab16c-279">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ab16c-279">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ab16c-280">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ab16c-280">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ab16c-281">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ab16c-281">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ab16c-282">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ab16c-282">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ab16c-283">Профиль</span><span class="sxs-lookup"><span data-stu-id="ab16c-283">Profile</span></span>

* <span data-ttu-id="ab16c-284">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ab16c-284">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ab16c-285">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ab16c-285">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ab16c-286">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ab16c-286">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ab16c-287">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="ab16c-287">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ab16c-288">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="ab16c-288">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ab16c-289">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ab16c-289">RDBMS</span></span>

* <span data-ttu-id="ab16c-290">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="ab16c-290">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ab16c-291">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="ab16c-291">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ab16c-292">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="ab16c-292">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ab16c-293">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="ab16c-293">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ab16c-294">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ab16c-294">Resource</span></span>

* <span data-ttu-id="ab16c-295">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-295">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ab16c-296">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-296">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ab16c-297">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-297">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ab16c-298">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-298">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ab16c-299">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="ab16c-299">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ab16c-300">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-300">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ab16c-301">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="ab16c-301">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ab16c-302">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-302">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ab16c-303">Роль</span><span class="sxs-lookup"><span data-stu-id="ab16c-303">Role</span></span>

* <span data-ttu-id="ab16c-304">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ab16c-304">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ab16c-305">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="ab16c-305">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ab16c-306">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="ab16c-306">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ab16c-307">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ab16c-307">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ab16c-308">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-308">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ab16c-309">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ab16c-309">Service Fabric</span></span>
* <span data-ttu-id="ab16c-310">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="ab16c-310">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ab16c-311">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="ab16c-311">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ab16c-312">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="ab16c-312">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ab16c-313">SQL</span><span class="sxs-lookup"><span data-stu-id="ab16c-313">SQL</span></span>

* <span data-ttu-id="ab16c-314">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-314">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ab16c-315">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-315">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ab16c-316">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-316">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ab16c-317">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ab16c-317">Storage</span></span>

* <span data-ttu-id="ab16c-318">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="ab16c-318">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ab16c-319">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="ab16c-319">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ab16c-320">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="ab16c-320">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ab16c-321">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ab16c-321">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="ab16c-322">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="ab16c-322">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="ab16c-323">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="ab16c-323">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ab16c-324">ВМ</span><span class="sxs-lookup"><span data-stu-id="ab16c-324">VM</span></span>

* <span data-ttu-id="ab16c-325">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="ab16c-325">Support configuring nsg</span></span>
* <span data-ttu-id="ab16c-326">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="ab16c-326">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ab16c-327">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ab16c-327">Support managed service identities</span></span>
* <span data-ttu-id="ab16c-328">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-328">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="ab16c-329">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="ab16c-329">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ab16c-330">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-330">May 10, 2017</span></span>

<span data-ttu-id="ab16c-331">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ab16c-331">Version 2.0.6</span></span>

* <span data-ttu-id="ab16c-332">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ab16c-332">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ab16c-333">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="ab16c-333">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ab16c-334">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ab16c-334">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="ab16c-335">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ab16c-335">Include Cognitive Services module.</span></span>
* <span data-ttu-id="ab16c-336">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ab16c-336">Include Service Fabric module.</span></span>
* <span data-ttu-id="ab16c-337">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="ab16c-337">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="ab16c-338">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="ab16c-338">Add support for CDN commands.</span></span>
* <span data-ttu-id="ab16c-339">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="ab16c-339">Remove Container module.</span></span>
* <span data-ttu-id="ab16c-340">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-340">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ab16c-341">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-341">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ab16c-342">Core</span><span class="sxs-lookup"><span data-stu-id="ab16c-342">Core</span></span>

* <span data-ttu-id="ab16c-343">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="ab16c-343">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="ab16c-344">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-344">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ab16c-345">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-345">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ab16c-346">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-346">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ab16c-347">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-347">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ab16c-348">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-348">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ab16c-349">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-349">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ab16c-350">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-350">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ab16c-351">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-351">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ab16c-352">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="ab16c-352">core: Improved performance</span></span>
* <span data-ttu-id="ab16c-353">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="ab16c-353">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ab16c-354">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="ab16c-354">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ab16c-355">ACS</span><span class="sxs-lookup"><span data-stu-id="ab16c-355">ACS</span></span>

* <span data-ttu-id="ab16c-356">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="ab16c-356">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ab16c-357">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="ab16c-357">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ab16c-358">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="ab16c-358">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ab16c-359">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-359">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ab16c-360">AppService</span><span class="sxs-lookup"><span data-stu-id="ab16c-360">AppService</span></span>

* <span data-ttu-id="ab16c-361">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="ab16c-361">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ab16c-362">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-362">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ab16c-363">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="ab16c-363">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ab16c-364">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ab16c-364">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ab16c-365">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ab16c-365">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ab16c-366">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-366">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ab16c-367">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="ab16c-367">support slot swap with preview</span></span>
* <span data-ttu-id="ab16c-368">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-368">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ab16c-369">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-369">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ab16c-370">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ab16c-370">CosmosDB</span></span>

* <span data-ttu-id="ab16c-371">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ab16c-371">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="ab16c-372">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="ab16c-372">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ab16c-373">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="ab16c-373">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ab16c-374">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="ab16c-374">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ab16c-375">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="ab16c-375">Data Lake Analytics</span></span>

* <span data-ttu-id="ab16c-376">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="ab16c-376">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="ab16c-377">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="ab16c-377">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ab16c-378">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-378">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ab16c-379">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="ab16c-379">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ab16c-380">Таблица</span><span class="sxs-lookup"><span data-stu-id="ab16c-380">Table</span></span>
  * <span data-ttu-id="ab16c-381">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="ab16c-381">Table valued function</span></span>
  * <span data-ttu-id="ab16c-382">Просмотр</span><span class="sxs-lookup"><span data-stu-id="ab16c-382">View</span></span>
  * <span data-ttu-id="ab16c-383">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="ab16c-383">Table Statistics.</span></span> <span data-ttu-id="ab16c-384">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="ab16c-384">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ab16c-385">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="ab16c-385">Data Lake Store</span></span>

* <span data-ttu-id="ab16c-386">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="ab16c-386">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="ab16c-387">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-387">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ab16c-388">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="ab16c-388">missed help for access show.</span></span> <span data-ttu-id="ab16c-389">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="ab16c-389">adding it.</span></span> <span data-ttu-id="ab16c-390">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ab16c-390">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ab16c-391">Поиск</span><span class="sxs-lookup"><span data-stu-id="ab16c-391">Find</span></span>

* <span data-ttu-id="ab16c-392">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="ab16c-392">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ab16c-393">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ab16c-393">KeyVault</span></span>

* <span data-ttu-id="ab16c-394">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="ab16c-394">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ab16c-395">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="ab16c-395">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="ab16c-396">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="ab16c-396">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ab16c-397">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="ab16c-397">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="ab16c-398">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-398">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ab16c-399">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ab16c-399">Lab</span></span>

* <span data-ttu-id="ab16c-400">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ab16c-400">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="ab16c-401">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ab16c-401">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="ab16c-402">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ab16c-402">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="ab16c-403">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ab16c-403">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="ab16c-404">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ab16c-404">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="ab16c-405">Монитор</span><span class="sxs-lookup"><span data-stu-id="ab16c-405">Monitor</span></span>

* <span data-ttu-id="ab16c-406">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-406">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ab16c-407">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-407">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ab16c-408">Сеть</span><span class="sxs-lookup"><span data-stu-id="ab16c-408">Network</span></span>

* <span data-ttu-id="ab16c-409">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-409">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="ab16c-410">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-410">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="ab16c-411">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-411">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="ab16c-412">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-412">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="ab16c-413">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ab16c-413">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="ab16c-414">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="ab16c-414">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="ab16c-415">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-415">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="ab16c-416">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ab16c-416">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="ab16c-417">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-417">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="ab16c-418">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="ab16c-418">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ab16c-419">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-419">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="ab16c-420">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-420">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="ab16c-421">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="ab16c-421">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="ab16c-422">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="ab16c-422">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="ab16c-423">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="ab16c-423">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="ab16c-424">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="ab16c-424">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="ab16c-425">Профиль</span><span class="sxs-lookup"><span data-stu-id="ab16c-425">Profile</span></span>

* <span data-ttu-id="ab16c-426">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-426">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ab16c-427">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-427">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ab16c-428">Redis</span><span class="sxs-lookup"><span data-stu-id="ab16c-428">Redis</span></span>

* <span data-ttu-id="ab16c-429">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="ab16c-429">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ab16c-430">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="ab16c-430">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="ab16c-431">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ab16c-431">Resource</span></span>

* <span data-ttu-id="ab16c-432">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-432">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ab16c-433">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-433">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ab16c-434">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-434">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ab16c-435">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="ab16c-435">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ab16c-436">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ab16c-436">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ab16c-437">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="ab16c-437">Add docs for az lock update.</span></span> <span data-ttu-id="ab16c-438">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ab16c-438">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ab16c-439">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="ab16c-439">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ab16c-440">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ab16c-440">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ab16c-441">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ab16c-441">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ab16c-442">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ab16c-442">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ab16c-443">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-443">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ab16c-444">Роль</span><span class="sxs-lookup"><span data-stu-id="ab16c-444">Role</span></span>

* <span data-ttu-id="ab16c-445">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-445">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ab16c-446">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-446">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ab16c-447">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-447">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ab16c-448">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="ab16c-448">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ab16c-449">SQL</span><span class="sxs-lookup"><span data-stu-id="ab16c-449">SQL</span></span>

* <span data-ttu-id="ab16c-450">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ab16c-450">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="ab16c-451">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-451">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ab16c-452">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ab16c-452">Storage</span></span>

* <span data-ttu-id="ab16c-453">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-453">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="ab16c-454">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ab16c-454">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ab16c-455">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ab16c-455">Add support for large block blob upload</span></span>
* <span data-ttu-id="ab16c-456">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ab16c-456">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ab16c-457">ВМ</span><span class="sxs-lookup"><span data-stu-id="ab16c-457">VM</span></span>

* <span data-ttu-id="ab16c-458">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="ab16c-458">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ab16c-459">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="ab16c-459">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ab16c-460">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ab16c-460">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ab16c-461">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ab16c-461">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ab16c-462">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="ab16c-462">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ab16c-463">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="ab16c-463">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ab16c-464">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-464">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ab16c-465">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-465">April 3, 2017</span></span>

<span data-ttu-id="ab16c-466">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ab16c-466">Version 2.0.2</span></span>

<span data-ttu-id="ab16c-467">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="ab16c-467">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="ab16c-468">Core</span><span class="sxs-lookup"><span data-stu-id="ab16c-468">Core</span></span>

* <span data-ttu-id="ab16c-469">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ab16c-469">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="ab16c-470">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-470">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ab16c-471">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-471">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ab16c-472">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-472">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ab16c-473">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-473">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ab16c-474">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="ab16c-474">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ab16c-475">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-475">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ab16c-476">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ab16c-476">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ab16c-477">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="ab16c-477">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="ab16c-478">ACS</span><span class="sxs-lookup"><span data-stu-id="ab16c-478">ACS</span></span>

* <span data-ttu-id="ab16c-479">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-479">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ab16c-480">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="ab16c-480">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ab16c-481">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-481">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ab16c-482">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="ab16c-482">Add support for windows clusters.</span></span> <span data-ttu-id="ab16c-483">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-483">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ab16c-484">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="ab16c-484">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ab16c-485">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-485">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="ab16c-486">AppService</span><span class="sxs-lookup"><span data-stu-id="ab16c-486">AppService</span></span>

* <span data-ttu-id="ab16c-487">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-487">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ab16c-488">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-488">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ab16c-489">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-489">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ab16c-490">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-490">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="ab16c-491">DataLake</span><span class="sxs-lookup"><span data-stu-id="ab16c-491">DataLake</span></span>

* <span data-ttu-id="ab16c-492">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ab16c-492">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="ab16c-493">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ab16c-493">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="ab16c-494">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ab16c-494">DocuemntDB</span></span>

* <span data-ttu-id="ab16c-495">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-495">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ab16c-496">ВМ</span><span class="sxs-lookup"><span data-stu-id="ab16c-496">VM</span></span>

* <span data-ttu-id="ab16c-497">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-497">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ab16c-498">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-498">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ab16c-499">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-499">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ab16c-500">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-500">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ab16c-501">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-501">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ab16c-502">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-502">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ab16c-503">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="ab16c-503">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ab16c-504">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ab16c-504">February 27, 2017</span></span>

<span data-ttu-id="ab16c-505">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ab16c-505">Version 2.0.0</span></span>

<span data-ttu-id="ab16c-506">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="ab16c-506">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="ab16c-507">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="ab16c-507">General availability applies to these command modules:</span></span>
- <span data-ttu-id="ab16c-508">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="ab16c-508">Container Service (acs)</span></span>
- <span data-ttu-id="ab16c-509">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="ab16c-509">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ab16c-510">Сеть</span><span class="sxs-lookup"><span data-stu-id="ab16c-510">Networking</span></span>
- <span data-ttu-id="ab16c-511">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ab16c-511">Storage</span></span>

<span data-ttu-id="ab16c-512">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="ab16c-512">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="ab16c-513">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="ab16c-513">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="ab16c-514">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-514">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="ab16c-515">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="ab16c-515">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="ab16c-516">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-516">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="ab16c-517">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="ab16c-517">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="ab16c-518">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="ab16c-518">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="ab16c-519">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="ab16c-519">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="ab16c-520">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="ab16c-520">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="ab16c-521">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ab16c-521">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="ab16c-522">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="ab16c-522">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ab16c-523">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="ab16c-523">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ab16c-524">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="ab16c-524">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="ab16c-525">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ab16c-525">Provide feedback from the command line with the `az feedback` command.</span></span>

