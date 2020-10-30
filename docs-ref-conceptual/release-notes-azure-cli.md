---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/27/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4e1f03268ccd001d6fe371b1ecdecb869791b198
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687129"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="5550f-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5550f-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="5550f-104">Заметки о текущем выпуске</span><span class="sxs-lookup"><span data-stu-id="5550f-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="october-27-2020"></a><span data-ttu-id="5550f-105">27 октября 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-105">October 27, 2020</span></span>

<span data-ttu-id="5550f-106">Версия 2.14.0</span><span class="sxs-lookup"><span data-stu-id="5550f-106">Version 2.14.0</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-107">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-107">AKS</span></span>

* <span data-ttu-id="5550f-108">Включена поддержка PPG.</span><span class="sxs-lookup"><span data-stu-id="5550f-108">Add PPG support</span></span>
* <span data-ttu-id="5550f-109">Изменено максимальное время ожидания для подсистемы балансировки нагрузки уровня "Стандартный" на значение в 100 минут.</span><span class="sxs-lookup"><span data-stu-id="5550f-109">Update max standard load balancer timeout to 100 minutes</span></span>

### <a name="apim"></a><span data-ttu-id="5550f-110">APIM</span><span class="sxs-lookup"><span data-stu-id="5550f-110">APIM</span></span>

* <span data-ttu-id="5550f-111">Исправлена проблема с созданием экземпляра уровня "Потребление".</span><span class="sxs-lookup"><span data-stu-id="5550f-111">Fix issue with creating consumption tier instance</span></span>

### <a name="app-config"></a><span data-ttu-id="5550f-112">Конфигурация приложения</span><span class="sxs-lookup"><span data-stu-id="5550f-112">App Config</span></span>

* <span data-ttu-id="5550f-113">Исправлен процесс запрашивания пар "ключ — значение" по меткам с разделителями-запятыми.</span><span class="sxs-lookup"><span data-stu-id="5550f-113">Fix querying key-values by comma separated labels</span></span>

### <a name="app-service"></a><span data-ttu-id="5550f-114">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-114">App Service</span></span>

* <span data-ttu-id="5550f-115">Исправлена проблема, при которой команда az webapp up не выполнялась, если у пользователя не было разрешений на запись в родительский каталог проекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-115">Bugfix: az webapp up fails when user doesn't have write permissions to project's parent directory</span></span>
* <span data-ttu-id="5550f-116">Исправление 13777: исправлена проблема с удалением escape-символов из XML.</span><span class="sxs-lookup"><span data-stu-id="5550f-116">Fix #13777: Fix to remove escape chars from XML</span></span>
* <span data-ttu-id="5550f-117">Исправление 15441: исправлена проблема, при которой выполнение az webapp create-remote-connection завершалось сбоем с ошибкой "AttributeError: 'Thread' object has no attribute 'isAlive'" (У объекта Thread нет атрибута isAlive).</span><span class="sxs-lookup"><span data-stu-id="5550f-117">Fix #15441: az webapp create-remote-connection fails with AttributeError: 'Thread' object has no attribute 'isAlive'</span></span>
* <span data-ttu-id="5550f-118">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] az webapp up: добавлены необязательные параметры (среда выполнения и ОС) и обновлены среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-118">[BREAKING CHANGE] az webapp up: add optional params (os & runtime) and updated runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-119">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-119">ARM</span></span>

* <span data-ttu-id="5550f-120">Команды What-If развертывания шаблона сделаны общедоступными.</span><span class="sxs-lookup"><span data-stu-id="5550f-120">Make template deployment What-If commands GA</span></span>
* <span data-ttu-id="5550f-121">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Добавлено подтверждение пользователя для az ts create.</span><span class="sxs-lookup"><span data-stu-id="5550f-121">[BREAKING CHANGE] Add user confirmation for az ts create</span></span>
* <span data-ttu-id="5550f-122">Исправлена проблема с возвращаемыми данными при создании тегов для нескольких ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-122">Fix the returned data when tagging multiple resources</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-123">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-123">Backup</span></span>

* <span data-ttu-id="5550f-124">`az backup policy create`: включена поддержка создания политики резервного копирования IaaSVM из интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="5550f-124">`az backup policy create`: Add support for IaaSVM backup policy creation from CLI</span></span>
* <span data-ttu-id="5550f-125">Увеличено ограничение защиты виртуальных машин со 100 до 1000.</span><span class="sxs-lookup"><span data-stu-id="5550f-125">Increasing VM protection limit from 100 to 1000</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-126">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-126">Compute</span></span>

* <span data-ttu-id="5550f-127">sig image-definition create: добавлен параметр --features.</span><span class="sxs-lookup"><span data-stu-id="5550f-127">sig image-definition create: add --features</span></span>
* <span data-ttu-id="5550f-128">Новая версия API gallery_images 2020-09-30.</span><span class="sxs-lookup"><span data-stu-id="5550f-128">New API version of gallery_images 2020-09-30</span></span>
* <span data-ttu-id="5550f-129">`az vm update / az sig image-version update`: включено обновление виртуальной машины или версии ее образа, даже если в ней используется межклиентский образ.</span><span class="sxs-lookup"><span data-stu-id="5550f-129">`az vm update / az sig image-version update`: Support update vm/image-version even it uses a cross tenant image</span></span>
* <span data-ttu-id="5550f-130">Отключена проверка номеров SKU узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5550f-130">Remove validation of vm host SKUs</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-131">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-131">Cosmos DB</span></span>

* <span data-ttu-id="5550f-132">`az cosmosdb create/update`: улучшено сообщение об ошибке из-за неправильного ввода --locations.</span><span class="sxs-lookup"><span data-stu-id="5550f-132">`az cosmosdb create/update`: Improve error message from incorrect --locations input</span></span>
* <span data-ttu-id="5550f-133">`az cosmosdb sql container create/update`: добавлен параметр --analytical-storage-ttl.</span><span class="sxs-lookup"><span data-stu-id="5550f-133">`az cosmosdb sql container create/update`: Add --analytical-storage-ttl parameter</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-134">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-134">HDInsight</span></span>

* <span data-ttu-id="5550f-135">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] az hdinsight create: удалены два параметра — --public-network-access-type и --outbound-public-network-access-type.</span><span class="sxs-lookup"><span data-stu-id="5550f-135">[BREAKING CHANGE] az hdinsight create: remove two parameters: --public-network-access-type and  --outbound-public-network-access-type</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-136">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-136">IoT Central</span></span>

* <span data-ttu-id="5550f-137">Удалено предупреждение о предварительной версии, так как уже предоставляется общедоступная версия.</span><span class="sxs-lookup"><span data-stu-id="5550f-137">Remove preview warning since it is already GAed</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-138">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-138">Key Vault</span></span>

* <span data-ttu-id="5550f-139">`--enable-soft-delete false` больше не используется при создании или обновлении хранилищ.</span><span class="sxs-lookup"><span data-stu-id="5550f-139">Invalidate `--enable-soft-delete false` while creating or updating vaults</span></span>
* <span data-ttu-id="5550f-140">`--bypass` и `--default-action` используются совместно с параметрами ACL сети при создании хранилищ.</span><span class="sxs-lookup"><span data-stu-id="5550f-140">Make `--bypass` and `--default-action` work together with network acl parameters while creating vaults</span></span>

### <a name="misc"></a><span data-ttu-id="5550f-141">Прочее</span><span class="sxs-lookup"><span data-stu-id="5550f-141">Misc.</span></span>

* <span data-ttu-id="5550f-142">Добавлена коллекция bash-completion в Dockerfile.</span><span class="sxs-lookup"><span data-stu-id="5550f-142">Add bash-completion to Dockerfile</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-143">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-143">RDBMS</span></span>

* <span data-ttu-id="5550f-144">Добавлена команда list-skus, преобразователь таблиц, локальный контекст для Postgres, MySQL, отдельный сервер MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-144">Add List-SKUS Command, Table Transformers, Local Context for Postgres, MySQL, Mariadb Single Server</span></span>
* <span data-ttu-id="5550f-145">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Обновлено имя параметра.</span><span class="sxs-lookup"><span data-stu-id="5550f-145">[BREAKING CHANGE] Parameter name updates.</span></span> <span data-ttu-id="5550f-146">Улучшения в плоскости управления для MySQL и PostgreSQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-146">Improvements to Management Plane for MySQL and PostgreSQL</span></span>
* <span data-ttu-id="5550f-147">`az postgres|mariadb|mysql server create`: обновлен интерфейс создания для Postgres, MySQL и MariaDB — новые поля в выходных данных; представлены новые значения для параметра `--public` в команде CREATE (all,<IP>,<IPRange>,0.0.0.0).</span><span class="sxs-lookup"><span data-stu-id="5550f-147">`az postgres|mariadb|mysql server create` : Update create experience for Postgres, MySQL and MariaDB - new fields in the output , Introduce new values for `--public` parameter in create command (all,<IP>,<IPRange>,0.0.0.0)</span></span>

### <a name="signalr"></a><span data-ttu-id="5550f-148">SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-148">SignalR</span></span>

* <span data-ttu-id="5550f-149">`az signalr create`: добавлен новый параметр `--enable-messaging-logs` для управления процессом создания службой журналов сообщений.</span><span class="sxs-lookup"><span data-stu-id="5550f-149">`az signalr create`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>
* <span data-ttu-id="5550f-150">`az signalr update`: добавлен новый параметр `--enable-messaging-logs` для управления процессом создания службой журналов сообщений.</span><span class="sxs-lookup"><span data-stu-id="5550f-150">`az signalr update`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-151">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-151">SQL</span></span>

* <span data-ttu-id="5550f-152">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Исправлен ответ для имени и значения параметра избыточности хранилища резервных копий для MI.</span><span class="sxs-lookup"><span data-stu-id="5550f-152">[BREAKING CHANGE] Fix response for backup storage redundancy param name and value for MI</span></span>
* <span data-ttu-id="5550f-153">`az sql db audit-policy show`: добавлено расширение для отображения политики аудита базы данных, включая данные о LA и EH.</span><span class="sxs-lookup"><span data-stu-id="5550f-153">`az sql db audit-policy show`: extend to show database's audit policy including LA and EH data</span></span>
* <span data-ttu-id="5550f-154">`az sql db audit-policy update`: добавлено расширение, разрешающее выполнять обновление LA и EH вместе с политикой аудита базы данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-154">`az sql db audit-policy update`: extend to allow LA and EH update along with database's audit policy</span></span>
* <span data-ttu-id="5550f-155">`az sql db audit-policy wait`: переключение интерфейса командной строки в состояние ожидания, пока не будет выполнено условие политики аудита базы данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-155">`az sql db audit-policy wait`: place the CLI in a waiting state until a condition of the database's audit policy is met.</span></span>
* <span data-ttu-id="5550f-156">`az sql server audit-policy show`: добавлено расширение для отображения политики аудита сервера, включая данные о LA и EH.</span><span class="sxs-lookup"><span data-stu-id="5550f-156">`az sql server audit-policy show`: extend to show servers's audit policy including LA and EH data</span></span>
* <span data-ttu-id="5550f-157">`az sql server audit-policy update`: добавлено расширение, разрешающее выполнять обновление LA и EH вместе с политикой аудита сервера.</span><span class="sxs-lookup"><span data-stu-id="5550f-157">`az sql server audit-policy update`: extend to allow LA and EH update along with server's audit policy</span></span>
* <span data-ttu-id="5550f-158">`az sql server audit-policy wait`: переключение интерфейса командной строки в состояние ожидания, пока не будет выполнено условие политики аудита сервера.</span><span class="sxs-lookup"><span data-stu-id="5550f-158">`az sql server audit-policy wait`: place the CLI in a waiting state until a condition of the server's audit policy is met.</span></span>
* <span data-ttu-id="5550f-159">Включена поддержка только AAD для Управляемых экземпляров и серверов SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-159">Add AAD-only Support for SQL Managed Instances and Servers</span></span>
* <span data-ttu-id="5550f-160">`az sql db replica create`: добавлен аргумент --partner-database.</span><span class="sxs-lookup"><span data-stu-id="5550f-160">`az sql db replica create`: Add --partner-database argument</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-161">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-161">Storage</span></span>

* <span data-ttu-id="5550f-162">Исправление 15111: исправлена проблема, при которой выполнение `az storage logging update` завершалось сбоем без дополнительного аргумента.</span><span class="sxs-lookup"><span data-stu-id="5550f-162">Fix #15111: `az storage logging update` fails without optional argument</span></span>
* <span data-ttu-id="5550f-163">Устранена проблема с использованием команды set-tier с именем входа субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-163">Fix bug when using set-tier command with service principal login</span></span>
* <span data-ttu-id="5550f-164">Обновление версии file-datalake до 2020-02-10</span><span class="sxs-lookup"><span data-stu-id="5550f-164">Upgrade version for file datalake to 2020-02-10</span></span>
* <span data-ttu-id="5550f-165">`az storage queue list`: включена поддержка Track2.</span><span class="sxs-lookup"><span data-stu-id="5550f-165">`az storage queue list`: Track2 supported</span></span>
* <span data-ttu-id="5550f-166">`az storage fs access`: включена поддержка рекурсивного управления списками ACL.</span><span class="sxs-lookup"><span data-stu-id="5550f-166">`az storage fs access`: Support managing ACLs recursively</span></span>

### <a name="synapse"></a><span data-ttu-id="5550f-167">Synapse</span><span class="sxs-lookup"><span data-stu-id="5550f-167">Synapse</span></span>

* <span data-ttu-id="5550f-168">Добавлены командлеты, связанные с конвейером, связанной службой, триггером, записной книжкой, потоком данных и набором данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-168">Add pipeline, linked service, trigger, notebook, data flow and dataset related cmdlets</span></span>

## <a name="october-13-2020"></a><span data-ttu-id="5550f-169">13 октября 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-169">October 13, 2020</span></span>

<span data-ttu-id="5550f-170">Версия 2.13.0</span><span class="sxs-lookup"><span data-stu-id="5550f-170">Version 2.13.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-171">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-171">ACR</span></span>

* <span data-ttu-id="5550f-172">`az acr helm`: обновлен устаревший URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5550f-172">`az acr helm`: Update deprecation url</span></span>
* <span data-ttu-id="5550f-173">Внесены изменения в logtemplate и systemtask для Задач ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-173">Add logtemplate and systemtask changes for ACR Tasks</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-174">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-174">AKS</span></span>

* <span data-ttu-id="5550f-175">Включена поддержка virtual-node с aks create: `az aks create --enable-addons virtual-node`.</span><span class="sxs-lookup"><span data-stu-id="5550f-175">Support virtual-node with aks create: `az aks create --enable-addons virtual-node`</span></span>
* <span data-ttu-id="5550f-176">Добавлен вариант использования только образа узла для CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-176">Add node image only option for CLI</span></span>
* <span data-ttu-id="5550f-177">Надстройка kube-dashboard будет отключена по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-177">Expect kube-dashboard addon be disabled by default</span></span>
* <span data-ttu-id="5550f-178">`az aks create/update`: добавлена поддержка LicenseType для Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-178">`az aks create/update`: Add LicenseType support for Windows</span></span>
* <span data-ttu-id="5550f-179">Включена возможность добавления пула точечных узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-179">Support add Spot node pool</span></span>
* <span data-ttu-id="5550f-180">Включена поддержка имен надстроек, определенных в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-180">Honor addon names defined in Azure CLI</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-181">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-181">AMS</span></span>

* <span data-ttu-id="5550f-182">Исправление № 14687. Добавлены группа ресурсов и имя учетной записи в команду az ams streaming-endpoint show.</span><span class="sxs-lookup"><span data-stu-id="5550f-182">Fix #14687: Mixed resource group and account name in command "az ams streaming-endpoint show"</span></span>

### <a name="app-config"></a><span data-ttu-id="5550f-183">Конфигурация приложения</span><span class="sxs-lookup"><span data-stu-id="5550f-183">App Config</span></span>

* <span data-ttu-id="5550f-184">Исправлена проблема с тестированием.</span><span class="sxs-lookup"><span data-stu-id="5550f-184">Fix test bug</span></span>
* <span data-ttu-id="5550f-185">Включена поддержка аутентификации AAD для операций с данными.</span><span class="sxs-lookup"><span data-stu-id="5550f-185">Support AAD auth for data operations</span></span>

### <a name="app-service"></a><span data-ttu-id="5550f-186">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-186">App Service</span></span>

* <span data-ttu-id="5550f-187">`az functionapp deployment source config-zip`: исправлена проблема, из-за которой config-zip вызывает исключение при успешном использовании Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-187">`az functionapp deployment source config-zip`: Fixed an issue where config-zip could throw an exception on success on linux consumption</span></span>
* <span data-ttu-id="5550f-188">Исправление. Улучшены сообщения об ошибках для команд веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-188">Bugfix: Better error messages for webapp commands</span></span>
* <span data-ttu-id="5550f-189">`az appservice domain create, show-terms`: добавлена возможность создания домена службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-189">`az appservice domain create, show-terms`: Add ability to create app service domain</span></span>
* <span data-ttu-id="5550f-190">`az functionapp create`: в Java 11 удален флаг предварительной версии при создании нового приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5550f-190">`az functionapp create`: Removed the preview flag from Java 11 when creating a new function app</span></span>
* <span data-ttu-id="5550f-191">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] az webapp create, az webapp up: обновлены доступные среды выполнения веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-191">[BREAKING CHANGE] az webapp create, az webapp up - Update available webapp runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-192">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-192">ARM</span></span>

* <span data-ttu-id="5550f-193">`az ts`: добавлены новые команды для спецификаций шаблонов.</span><span class="sxs-lookup"><span data-stu-id="5550f-193">`az ts`: Add new commands for template specs</span></span>
* <span data-ttu-id="5550f-194">`az deployment`: добавлена поддержка --template-spec -s.</span><span class="sxs-lookup"><span data-stu-id="5550f-194">`az deployment` : Add support for --template-spec -s</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-195">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-195">Compute</span></span>

* <span data-ttu-id="5550f-196">Устранено ограничение счетчика домена сбоя для создания группы узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-196">Fix host group creation FD count limitation</span></span>
* <span data-ttu-id="5550f-197">Добавлена новая команда для обновления расширений для VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-197">Add new command to support upgrading extensions for VMSS</span></span>
* <span data-ttu-id="5550f-198">Исправлена проблема с отсутствующей ссылкой на образ.</span><span class="sxs-lookup"><span data-stu-id="5550f-198">Fix the image reference is missing issue</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-199">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-199">HDInsight</span></span>

* <span data-ttu-id="5550f-200">`az hdinsight create`: добавлены сведения об устаревании аргументов --public-networrk-access-type и --outbound-public-network-access-type.</span><span class="sxs-lookup"><span data-stu-id="5550f-200">`az hdinsight create`: add deprecate information for argument --public-networrk-access-type and --outbound-public-network-access-type</span></span>
* <span data-ttu-id="5550f-201">`az hdinsight create`: добавлены сведения об устаревании для аргументов `--public-networrk-access-type` и `--outbound-public-network-access-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-201">`az hdinsight create`: add deprecate information for argument `--public-networrk-access-type` and `--outbound-public-network-access-type`</span></span>
* <span data-ttu-id="5550f-202">`az hdinsight create`: добавлен параметр `--idbroker`, чтобы включить поддержку клиента для создания кластера ESP с помощью брокера удостоверений HDInsight.</span><span class="sxs-lookup"><span data-stu-id="5550f-202">`az hdinsight create`:  add parameter `--idbroker` to support customer to create ESP cluster with HDInsight Id Broker</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-203">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-203">IoT Central</span></span>

* <span data-ttu-id="5550f-204">Удален устаревший модуль команды az iotcentral.</span><span class="sxs-lookup"><span data-stu-id="5550f-204">Remove deprecated 'az iotcentral' command module</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-205">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-205">Key Vault</span></span>

* <span data-ttu-id="5550f-206">Включена поддержка `--hsm-name` для `az keyvault key encrypt/decrypt`.</span><span class="sxs-lookup"><span data-stu-id="5550f-206">Support `--hsm-name` for `az keyvault key encrypt/decrypt`</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-207">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-207">Lab</span></span>

* <span data-ttu-id="5550f-208">Исправление № 14127. `__init__()` принимает 1 позиционный аргумент, хотя было указано 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-208">Fix #14127: `__init__()` takes 1 positional argument but 2 were given</span></span>

### <a name="network"></a><span data-ttu-id="5550f-209">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-209">Network</span></span>

* <span data-ttu-id="5550f-210">`az network application-gateway ssl-cert show`: добавлен пример для демонстрации формата сертификата и сведений о получении.</span><span class="sxs-lookup"><span data-stu-id="5550f-210">`az network application-gateway ssl-cert show`: Add example to demonstrate certificate format and fetch information</span></span>
* <span data-ttu-id="5550f-211">`az network application-gateway rule`: включена поддержка параметра --priority.</span><span class="sxs-lookup"><span data-stu-id="5550f-211">`az network application-gateway rule`: Support --priority option</span></span>
* <span data-ttu-id="5550f-212">`az network application-gateway create`: исправлена проблема, из-за которой операция создания не выполнялась без определенного общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="5550f-212">`az network application-gateway create`: Fix bug that cannot create without public IP sepcified</span></span>
* <span data-ttu-id="5550f-213">`az network application-gateway waf-policy managed-rule rule-set add`: включено отображение пользователю ошибки сервера, чтобы предоставить более интуитивно понятное сообщение подсказки.</span><span class="sxs-lookup"><span data-stu-id="5550f-213">`az network application-gateway waf-policy managed-rule rule-set add`: Expose server error to user to give more intuitive hint message.</span></span>
* <span data-ttu-id="5550f-214">`az network application-gateway waf-policy managed-rule rule-set update`: включена поддержка изменения версии типа набора правил.</span><span class="sxs-lookup"><span data-stu-id="5550f-214">`az network application-gateway waf-policy managed-rule rule-set update`: Support to change rule set type version.</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-215">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-215">RDBMS</span></span>

* <span data-ttu-id="5550f-216">Исправление. az postgres flexible-server create: удалена включенная в код версия API из клиента сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-216">Bugfix: az postgres flexible-server create Remove hardcoded API version from network client.</span></span>

### <a name="role"></a><span data-ttu-id="5550f-217">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-217">Role</span></span>

* <span data-ttu-id="5550f-218">Исправление № 15278. `az role assignment list/delete`: запрещены пустые строковые аргументы.</span><span class="sxs-lookup"><span data-stu-id="5550f-218">Fix #15278: `az role assignment list/delete`: Forbid empty string arguments</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-219">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-219">SQL</span></span>

* <span data-ttu-id="5550f-220">`az sql midb log-replay`: включена поддержка службы воспроизведения журналов в управляемой базе данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-220">`az sql midb log-replay`: Support for log replay service on managed database</span></span>
* <span data-ttu-id="5550f-221">Регистр символов для значения параметра избыточности хранилища резервных копий для управляемого экземпляра игнорируется.</span><span class="sxs-lookup"><span data-stu-id="5550f-221">Ignore character casing for backup storage redundancy param value for managed instance</span></span>
* <span data-ttu-id="5550f-222">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] az sql db create: добавлен параметр --backup-storage-redundancy; добавлено предупреждение о неуказанном bsr/bsr == Geo.</span><span class="sxs-lookup"><span data-stu-id="5550f-222">[BREAKING CHANGE] az sql db create: Add --backup-storage-redundancy parameter; add warning for unspecified bsr/bsr == Geo.</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5550f-223">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-223">SQL VM</span></span>

* <span data-ttu-id="5550f-224">`az sql vm show`: добавлены параметры конфигурации для флага --expand.</span><span class="sxs-lookup"><span data-stu-id="5550f-224">`az sql vm show`: Add configuration options to --expand flag</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-225">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-225">Storage</span></span>

* <span data-ttu-id="5550f-226">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage blob copy start`: исправлена проблема с форматом для `--destination-if-modified-since` и `--destination-if-unmodified-since`.</span><span class="sxs-lookup"><span data-stu-id="5550f-226">[BREAKING CHANGE] `az storage blob copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="5550f-227">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage blob incremental-copy start`: исправлена проблема с форматом для `--destination-if-modified-since` и `--destination-if-unmodified-since`.</span><span class="sxs-lookup"><span data-stu-id="5550f-227">[BREAKING CHANGE] `az storage blob incremental-copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="5550f-228">`az storage fs`: исправлена проблема со строкой подключения.</span><span class="sxs-lookup"><span data-stu-id="5550f-228">`az storage fs`: Fix connection string issue</span></span>
* <span data-ttu-id="5550f-229">`az storage share-rm`: реализован уровень доступа для выпуска общедоступной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-229">`az storage share-rm`: GA release access tier</span></span>
* <span data-ttu-id="5550f-230">`az storage container-rm`: добавлена новая группа команд для использования поставщика ресурсов Microsoft.Storage в операциях управления контейнерами.</span><span class="sxs-lookup"><span data-stu-id="5550f-230">`az storage container-rm`: Add a new command group to use the Microsoft.Storage resource provider for container management operations.</span></span>

## <a name="september-29-2020"></a><span data-ttu-id="5550f-231">29 сентября 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-231">September 29, 2020</span></span>

<span data-ttu-id="5550f-232">Версия 2.12.1</span><span class="sxs-lookup"><span data-stu-id="5550f-232">Version 2.12.1</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-233">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-233">RDBMS</span></span>

* <span data-ttu-id="5550f-234">Исправление команды `az postgres flexible-server create`: обновлено свойство VnetName для исключения servername, обновлен регион по умолчанию для MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-234">Hotfix: `az postgres flexible-server create` : Update VnetName to exclude servername and update default region for MySQL</span></span>

## <a name="september-22-2020"></a><span data-ttu-id="5550f-235">22 сентября 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-235">September 22, 2020</span></span>

<span data-ttu-id="5550f-236">Версия 2.12.0</span><span class="sxs-lookup"><span data-stu-id="5550f-236">Version 2.12.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-237">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-237">ACR</span></span>

* <span data-ttu-id="5550f-238">Исправление № 14811. Включена поддержка переопределения dockerignore.</span><span class="sxs-lookup"><span data-stu-id="5550f-238">Fix #14811 Add support for dockerignore override</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-239">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-239">AKS</span></span>

* <span data-ttu-id="5550f-240">В CLI должна быть поддержка пустого файла kubeconfig.</span><span class="sxs-lookup"><span data-stu-id="5550f-240">CLI should tolerate empty kubeconfig</span></span>
* <span data-ttu-id="5550f-241">Исправление № 12871. az aks enable-addons: недопустимый пример автоматически сформированной справки для параметра vitual-node.</span><span class="sxs-lookup"><span data-stu-id="5550f-241">FIX #12871: az aks enable-addons: Autogenerated help example is wrong for vitual-node option</span></span>
* <span data-ttu-id="5550f-242">Удаление устаревших действий соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="5550f-242">Remove legacy aci connector actions</span></span>
* <span data-ttu-id="5550f-243">Включена поддержка надстройки Политики Azure в azure-cli.</span><span class="sxs-lookup"><span data-stu-id="5550f-243">Support azure policy addon in azure-cli</span></span>
* <span data-ttu-id="5550f-244">Исправлена ошибка, связанная с учетом регистра в надстройке панели мониторинга AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-244">Fix case sensitive issue for AKS dashboard addon</span></span>
* <span data-ttu-id="5550f-245">Обновлена версия mgmt-containerservice до 9.4.0 и включена поддержка API 09-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-245">Update mgmt-containerservice to 9.4.0 and enable 09-01 API</span></span>

### <a name="apim"></a><span data-ttu-id="5550f-246">APIM</span><span class="sxs-lookup"><span data-stu-id="5550f-246">APIM</span></span>

* <span data-ttu-id="5550f-247">Включена поддержка команд сущностей product, productapi и namedValue, а также обновлена версия пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5550f-247">Support product / productapi / namedValue entity commands && bump sdk version</span></span>

### <a name="app-config"></a><span data-ttu-id="5550f-248">Конфигурация приложения</span><span class="sxs-lookup"><span data-stu-id="5550f-248">App Config</span></span>

* <span data-ttu-id="5550f-249">Включена поддержка включения и отключения PublicNetworkAccess для существующих хранилищ.</span><span class="sxs-lookup"><span data-stu-id="5550f-249">Support enabling/disabling PublicNetworkAccess for existing stores</span></span>

### <a name="app-service"></a><span data-ttu-id="5550f-250">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-250">App Service</span></span>

* <span data-ttu-id="5550f-251">Включена поддержка ценовой категории "Премиум" версии 3.</span><span class="sxs-lookup"><span data-stu-id="5550f-251">Add support for Premium V3 pricing tier</span></span>
* <span data-ttu-id="5550f-252">Исправление № 12653. Значение false для az webapp log config --application-logging не приводит к отключению.</span><span class="sxs-lookup"><span data-stu-id="5550f-252">Fix #12653: az webapp log config --application-logging false doesn't turn it off</span></span>
* <span data-ttu-id="5550f-253">Исправление № 14684. Удаление ограничений доступа по IP-адресу не работает. № 13837. az webapp create: пример для разных RSgroups для плана и веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-253">Fix #14684: access-restriction remove by ip address does not work; #13837-az webapp create - Example for different RSgroups for Plan and WebApp</span></span>
* <span data-ttu-id="5550f-254">functionapp: включена поддержка пользовательских обработчиков.</span><span class="sxs-lookup"><span data-stu-id="5550f-254">functionapp: Add support for custom handlers.</span></span> <span data-ttu-id="5550f-255">PowerShell 6.2 не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="5550f-255">Deprecated Powershell 6.2.</span></span>
* <span data-ttu-id="5550f-256">functionapp: исправлена ошибка, из-за которой параметр приложения был неправильно задан для пользовательских образов Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-256">functionapp: Fix issue where app setting was being incorrectly set for linux custom images</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-257">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-257">ARM</span></span>

* <span data-ttu-id="5550f-258">`az deployment group/sub/mg/tenant what-if`: отображение игнорируемых изменений ресурсов в последнюю очередь.</span><span class="sxs-lookup"><span data-stu-id="5550f-258">`az deployment group/sub/mg/tenant what-if`: Show "Ignore" resource changes last</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-259">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-259">Compute</span></span>

* <span data-ttu-id="5550f-260">Добавлен новый параметр new license_type в команды создания и обновления виртуальной машины: RHEL_BYOS, SLES_BYOS.</span><span class="sxs-lookup"><span data-stu-id="5550f-260">Add new license_type in vm create/update: RHEL_BYOS, SLES_BYOS</span></span>
* <span data-ttu-id="5550f-261">Обновлена версия API диска до 2020-06-30.</span><span class="sxs-lookup"><span data-stu-id="5550f-261">Upgrade disk API version to 2020-06-30</span></span>
* <span data-ttu-id="5550f-262">disk create: добавлены параметры --logical-sector-size, --tier.</span><span class="sxs-lookup"><span data-stu-id="5550f-262">disk create: add --logical-sector-size, --tier</span></span>
* <span data-ttu-id="5550f-263">Обновление диска: включенна поддержка параметров --disk-iops-read-only, --disk-mbps-read-only, --max-shares.</span><span class="sxs-lookup"><span data-stu-id="5550f-263">disk update: Support --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span></span>
* <span data-ttu-id="5550f-264">Новая команда: disk-encryption-set list-associated-resources.</span><span class="sxs-lookup"><span data-stu-id="5550f-264">New command disk-encryption-set list-associated-resources</span></span>
* <span data-ttu-id="5550f-265">vm boot-diagnostics enable: параметр --storage стал необязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-265">vm boot-diagnostics enable: --storage becomes optional</span></span>
* <span data-ttu-id="5550f-266">Новая команда: vm boot-diagnostics get-boot-log-uris.</span><span class="sxs-lookup"><span data-stu-id="5550f-266">New command: vm boot-diagnostics get-boot-log-uris</span></span>
* <span data-ttu-id="5550f-267">vm boot-diagnostics get-boot-log: включена поддержка управляемого хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-267">vm boot-diagnostics get-boot-log: support managed storage</span></span>

### <a name="config"></a><span data-ttu-id="5550f-268">Config</span><span class="sxs-lookup"><span data-stu-id="5550f-268">Config</span></span>

* <span data-ttu-id="5550f-269">local-context теперь называется config param-persist.</span><span class="sxs-lookup"><span data-stu-id="5550f-269">Rename local-context to config param-persist</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-270">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-270">Cosmos DB</span></span>

* <span data-ttu-id="5550f-271">Включена поддержка API миграции для ресурса пропускной способности для функции автомасштабирования в Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5550f-271">Support for Migration APIs for Throughput resource for Autoscale feature in CosmosDB</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-272">Eventhub</span><span class="sxs-lookup"><span data-stu-id="5550f-272">Eventhub</span></span>

<span data-ttu-id="5550f-273">Добавлены команды кластера и параметр trusted_service_access_enabled для Networkruleset.</span><span class="sxs-lookup"><span data-stu-id="5550f-273">Added Cluster commands and trusted_service_access_enabled parameter for Networkruleset</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-274">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-274">Extension</span></span>

* <span data-ttu-id="5550f-275">`az extension add`: добавлен параметр `--upgrade`, чтобы обновить расширение, если оно уже установлено.</span><span class="sxs-lookup"><span data-stu-id="5550f-275">`az extension add`: Add `--upgrade` option to update the extension if already installed</span></span>
* <span data-ttu-id="5550f-276">Включена динамическая установка по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-276">Turn on dynamic install by default</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-277">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-277">IoT</span></span>

* <span data-ttu-id="5550f-278">Включена минимальная версия TLS при создании Центра Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5550f-278">Enabled minimum TLS version on IoT Hub Create</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-279">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-279">IoT Central</span></span>

* <span data-ttu-id="5550f-280">Операция удаления приложения теперь является длительной.</span><span class="sxs-lookup"><span data-stu-id="5550f-280">App delete operation is now long running operation</span></span>

### <a name="iot-hub"></a><span data-ttu-id="5550f-281">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-281">Iot Hub</span></span>

* <span data-ttu-id="5550f-282">Команда show-connection-string является нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="5550f-282">Deprecated 'show-connection-string' command</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-283">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-283">Key Vault</span></span>

* <span data-ttu-id="5550f-284">Управляемое устройство HSM (общедоступная предварительная версия).</span><span class="sxs-lookup"><span data-stu-id="5550f-284">Managed HSM public preview</span></span>
* <span data-ttu-id="5550f-285">Устранена ошибка, из-за которой параметр `--maxresults` не работал при перечислении ресурсов или версий ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-285">Fix the issue that `--maxresults` does not take effect while listing resources or resource versions</span></span>

### <a name="kusto"></a><span data-ttu-id="5550f-286">Kusto</span><span class="sxs-lookup"><span data-stu-id="5550f-286">Kusto</span></span>

* <span data-ttu-id="5550f-287">Добавлено сообщение об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5550f-287">Add deprecating message</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-288">Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="5550f-288">Monitor</span></span>

* <span data-ttu-id="5550f-289">`az monitor log-analytics workspace linked-storage`: предоставление пользователям подробного сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-289">`az monitor log-analytics workspace linked-storage`: expose detailed error message to customers</span></span>

### <a name="network"></a><span data-ttu-id="5550f-290">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-290">Network</span></span>

* <span data-ttu-id="5550f-291">`az network vnet subnet`: включена поддержка параметров --disable-private-endpoint-network-policies и --disable-private-link-service-network-policies.</span><span class="sxs-lookup"><span data-stu-id="5550f-291">`az network vnet subnet`: Support --disable-private-endpoint-network-policies and --disable-private-link-service-network-policies</span></span>
* <span data-ttu-id="5550f-292">Исправлена ошибка при обновлении flow-log, если подсвойство network_watcher_flow_analytics_configuration имеет значение None.</span><span class="sxs-lookup"><span data-stu-id="5550f-292">Fix bug while updateing flow-log when its subproperty network_watcher_flow_analytics_configuration is None</span></span>
* <span data-ttu-id="5550f-293">Обновлена версия API до 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-293">API version bump to 2020-06-01</span></span>
* <span data-ttu-id="5550f-294">Включена поддержка --tcp-port-behavior при настройке конфигурации TCP Монитора подключений версии 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-294">Support --tcp-port-behavior while configuring a TCP configuration of a Connection Monitor V2</span></span>
* <span data-ttu-id="5550f-295">Включена поддержка дополнительных типов и уровня покрытия при создании конечной точки Монитора подключений версии 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-295">Support more types and coverage level while creating Endpoint of Connection Monitor V2</span></span>
* <span data-ttu-id="5550f-296">Включена поддержка параметра --host-subnet для создания VirtualHub в качестве VirtualRouter.</span><span class="sxs-lookup"><span data-stu-id="5550f-296">Support --host-subnet to create VirtualHub underneath as VirtualRouter</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-297">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-297">RDBMS</span></span>

* <span data-ttu-id="5550f-298">Обновления плоскости управления для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-298">Management Plane updates for PostgreSQL and MySQL</span></span>

### <a name="role"></a><span data-ttu-id="5550f-299">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-299">Role</span></span>

* <span data-ttu-id="5550f-300">`az role assignment create/update`: включена поддержка `--description`, `--condition` и `--condition-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-300">`az role assignment create/update`: Support `--description`, `--condition` and `--condition-version`</span></span>
* <span data-ttu-id="5550f-301">`az ad app permission delete`: включена поддержка `--api-permissions` для удаления определенного `ResourceAccess`.</span><span class="sxs-lookup"><span data-stu-id="5550f-301">`az ad app permission delete`: Support `--api-permissions` to delete specific `ResourceAccess`</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-302">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-302">Service Fabric</span></span>

* <span data-ttu-id="5550f-303">Добавлены команды управляемого кластера и типа узла.</span><span class="sxs-lookup"><span data-stu-id="5550f-303">Add managed cluster and node type commands</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-304">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-304">SQL</span></span>

* <span data-ttu-id="5550f-305">Обновлена версия azure-mgmt-sql до 0.20.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-305">Upgrade azure-mgmt-sql to 0.20.0</span></span>
* <span data-ttu-id="5550f-306">Добавлен необязательный параметр избыточности хранилища резервных копий в командлет для создания MI.</span><span class="sxs-lookup"><span data-stu-id="5550f-306">Add backup storage redundancy optional parameter to MI create cmdlet</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-307">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-307">Storage</span></span>

* <span data-ttu-id="5550f-308">`az storage share-rm stats`: возможность получения сведений об используемых байтах для данных, которые хранятся в общей папке.</span><span class="sxs-lookup"><span data-stu-id="5550f-308">`az storage share-rm stats`: Get the usage bytes of the data stored on the share.</span></span>
* <span data-ttu-id="5550f-309">Общедоступная версия Хранилища BLOB-объектов — PITR.</span><span class="sxs-lookup"><span data-stu-id="5550f-309">GA release storage blob PITR</span></span>
* <span data-ttu-id="5550f-310">`az storage blob query`: включена поддержка ускорения запросов службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-310">`az storage blob query`: Support Azure Storage Query Acceleration</span></span>
* <span data-ttu-id="5550f-311">Включена поддержка обратимого удаления общих папок.</span><span class="sxs-lookup"><span data-stu-id="5550f-311">Support Soft Delete for file share</span></span>
* <span data-ttu-id="5550f-312">`az storage copy`: включена поддержка учетных данных и устаревание `--source-local-path`, `--destination-local-path` и `--destination-account-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-312">`az storage copy`: Add account credentials support and deprecate `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span></span>
* <span data-ttu-id="5550f-313">`az storage account blob-service-properties update`: включена поддержка политики хранения контейнера при удалении.</span><span class="sxs-lookup"><span data-stu-id="5550f-313">`az storage account blob-service-properties update`: Add container delete retention policy support</span></span>

### <a name="synapse"></a><span data-ttu-id="5550f-314">Synapse</span><span class="sxs-lookup"><span data-stu-id="5550f-314">Synapse</span></span>

* <span data-ttu-id="5550f-315">Исправлена опечатка в примере az synapse role assignment (create и delete).</span><span class="sxs-lookup"><span data-stu-id="5550f-315">Fixed typo in example of az synapse role assignment create and delete</span></span>

## <a name="august-28-2020"></a><span data-ttu-id="5550f-316">28 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-316">August 28, 2020</span></span>

<span data-ttu-id="5550f-317">Версия 2.11.1</span><span class="sxs-lookup"><span data-stu-id="5550f-317">Version 2.11.1</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-318">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-318">ACR</span></span>

* <span data-ttu-id="5550f-319">В пул агентов добавлен изолированный уровень.</span><span class="sxs-lookup"><span data-stu-id="5550f-319">Add Isolated Tier to Agent Pool</span></span>
* <span data-ttu-id="5550f-320">Добавлен контекст источника артефакта OCI.</span><span class="sxs-lookup"><span data-stu-id="5550f-320">Add OCI Artifact Source Context</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-321">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-321">AKS</span></span>

* <span data-ttu-id="5550f-322">Исправлена ошибка с созданием кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-322">Fix aks cluster create issue</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-323">Службы Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-323">Cognitive Services</span></span>

* <span data-ttu-id="5550f-324">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Отображены дополнительные условия использования для некоторых API-интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-324">[BREAKING CHANGE] Show additional legal term for certain APIs</span></span>

### <a name="network"></a><span data-ttu-id="5550f-325">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-325">Network</span></span>

* <span data-ttu-id="5550f-326">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Включена возможность создавать общедоступные и частные IP-адреса при создании Шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-326">[BREAKING CHANGE] Allow to create both public and private IP while creating an Application Gateway</span></span>
* <span data-ttu-id="5550f-327">`az network list-service-tags`: добавлены сведения об использовании параметра расположения в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5550f-327">`az network list-service-tags`: add details on location parameter use to the help message</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-328">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="5550f-328">Storage</span></span>

* <span data-ttu-id="5550f-329">`az storage blob list`: включена поддержка свойств OR с новой версией API.</span><span class="sxs-lookup"><span data-stu-id="5550f-329">`az storage blob list`: Support OR properties with new api version</span></span>

## <a name="august-25-2020"></a><span data-ttu-id="5550f-330">25 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-330">August 25, 2020</span></span>

<span data-ttu-id="5550f-331">Версия 2.11.0</span><span class="sxs-lookup"><span data-stu-id="5550f-331">Version 2.11.0</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-332">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-332">AKS</span></span>

* <span data-ttu-id="5550f-333">Из надстройки виртуальных узлов удален тег предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-333">Remove preview tag from Virtual Node add-on</span></span>
* <span data-ttu-id="5550f-334">Добавлен аргумент CMK AKS, используемый при создании кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-334">Add AKS CMK argument in cluster creation</span></span>
* <span data-ttu-id="5550f-335">Задан сетевой профиль при использовании базовой подсистемы балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5550f-335">Set network profile when using basic load balancer.</span></span>
* <span data-ttu-id="5550f-336">Из CLI удалена проверка максимального числа групп pod и включена предварительная обработка.</span><span class="sxs-lookup"><span data-stu-id="5550f-336">Remove max pods validation from CLI and let preflight handle it</span></span>
* <span data-ttu-id="5550f-337">Исправлены ошибки с надстройками, доступными в справочном сообщении в `az aks create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-337">Fixing add-ons available in the help message in `az aks create`</span></span>
* <span data-ttu-id="5550f-338">В основном CLI включена поддержка профиля автомасштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-338">Bring in support for cluster autoscaler profile in core CLI</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-339">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-339">AppService</span></span>

* <span data-ttu-id="5550f-340">`az webapp`: добавлена команда list-instances.</span><span class="sxs-lookup"><span data-stu-id="5550f-340">`az webapp`: Add list-instances command</span></span>
* <span data-ttu-id="5550f-341">`az webapp ssh`: добавлен параметр --instance для подключения к определенному экземпляру.</span><span class="sxs-lookup"><span data-stu-id="5550f-341">`az webapp ssh`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="5550f-342">`az webapp create-remote-connection`: добавлен параметр --instance для подключения к определенному экземпляру.</span><span class="sxs-lookup"><span data-stu-id="5550f-342">`az webapp create-remote-connection`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="5550f-343">Исправление № 14758: az webapp вызывает ошибки при создании приложения Windows с помощью --runtime dotnetcore.</span><span class="sxs-lookup"><span data-stu-id="5550f-343">Fix #14758: az webapp create errors when creating windows app with --runtime dotnetcore</span></span>
* <span data-ttu-id="5550f-344">Исправление № 14701: реализовано functionapp create --assign-identity.</span><span class="sxs-lookup"><span data-stu-id="5550f-344">Fix #14701: Implement functionapp create --assign-identity</span></span>
* <span data-ttu-id="5550f-345">Исправление № 11244: `az webapp auth update`: Добавлен необязательный параметр для обновления client-secret-certificate-thumbprint.</span><span class="sxs-lookup"><span data-stu-id="5550f-345">Fix #11244: `az webapp auth update`: Add optional parameter to update client-secret-certificate-thumbprint</span></span>
* <span data-ttu-id="5550f-346">`az functionapp keys`: добавлены команды, позволяющие пользователям управлять ключами приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5550f-346">`az functionapp keys`: Added commands that allow users to manage their function app keys</span></span>
* <span data-ttu-id="5550f-347">`az functionapp function`: добавлены команды, позволяющие пользователям управлять отдельными функциями.</span><span class="sxs-lookup"><span data-stu-id="5550f-347">`az functionapp function`: Added commands that allow users to manage their individual functions</span></span>
* <span data-ttu-id="5550f-348">`az functionapp function keys`: добавлены команды, позволяющие пользователям управлять ключами функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-348">`az functionapp function keys`: Added commands that allow users to manage their function keys</span></span>
* <span data-ttu-id="5550f-349">Исправление № 14788: az webapp create не получает правильное веб-приложение, если имена являются подстроками.</span><span class="sxs-lookup"><span data-stu-id="5550f-349">Fix #14788: az webapp create not getting correct webapp when names are substrings</span></span>
* <span data-ttu-id="5550f-350">`az functionapp create`: исключена возможность создания Функций 2.x в регионах, которые не поддерживают службу</span><span class="sxs-lookup"><span data-stu-id="5550f-350">`az functionapp create`: Removed ability to create 2.x Functions in regions that don't support it</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-351">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-351">ARM</span></span>

* <span data-ttu-id="5550f-352">`az resource list`: расширены возвращаемые данные `createdTime`, `changedTime` и `provisioningState`.</span><span class="sxs-lookup"><span data-stu-id="5550f-352">`az resource list`: Extend the return data of `createdTime`, `changedTime` and `provisioningState`</span></span>
* <span data-ttu-id="5550f-353">`az resource`: добавлен параметр `--latest-include-preview` для включения поддержки с использованием последней версии API, даже если это предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5550f-353">`az resource`: Add parameter `--latest-include-preview` to support using the latest api-version whether this version is preview</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-354">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-354">ARO</span></span>

* <span data-ttu-id="5550f-355">Улучшен CLI, включая добавление разрешений на проверку таблицы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="5550f-355">CLI enhancements, including route table checking permissions</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-356">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-356">Cloud</span></span>

* <span data-ttu-id="5550f-357">`az cloud register`: исправлена регистрация облаков с использованием файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5550f-357">`az cloud register`: Fix registering clouds with a config file</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-358">Вычисления</span><span class="sxs-lookup"><span data-stu-id="5550f-358">Compute</span></span>

* <span data-ttu-id="5550f-359">Обновлены номера SKU виртуальных машин, поддерживающих ускорение работы в сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-359">Update VM SKUs that support accelerated networking</span></span>
* <span data-ttu-id="5550f-360">`az vm create`: автоматическая установка исправлений в гостевой системе.</span><span class="sxs-lookup"><span data-stu-id="5550f-360">`az vm create`: Automatic in-guest patching</span></span>
* <span data-ttu-id="5550f-361">`az image builder create`: добавлены параметры --vm-size, --os-disk-size, --vnet, --subnet.</span><span class="sxs-lookup"><span data-stu-id="5550f-361">`az image builder create`: Add --vm-size, --os-disk-size, --vnet, --subnet</span></span>
* <span data-ttu-id="5550f-362">Новая команда az vm assess-patches.</span><span class="sxs-lookup"><span data-stu-id="5550f-362">New command az vm assess-patches</span></span>

### <a name="container"></a><span data-ttu-id="5550f-363">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-363">Container</span></span>

* <span data-ttu-id="5550f-364">Исправление № 6235: обновлен текст справки для параметра ports в container create.</span><span class="sxs-lookup"><span data-stu-id="5550f-364">Fix #6235: Update help text for ports parameter in container create</span></span>

### <a name="datalake-store"></a><span data-ttu-id="5550f-365">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5550f-365">Datalake Store</span></span>

* <span data-ttu-id="5550f-366">Устранена ошибка № 14545 с операцией подключения к Data Lake.</span><span class="sxs-lookup"><span data-stu-id="5550f-366">Fix issue #14545 for data lake join operation</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-367">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-367">EventHub</span></span>

* <span data-ttu-id="5550f-368">`az eventhubs eventhub create/update`: изменена документация по destination_name.</span><span class="sxs-lookup"><span data-stu-id="5550f-368">`az eventhubs eventhub create/update`: Change documentation of destination_name</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-369">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-369">Extension</span></span>

* <span data-ttu-id="5550f-370">Добавлена команда `az extension list-versions` для выведения списка всех доступных версий расширения.</span><span class="sxs-lookup"><span data-stu-id="5550f-370">Add `az extension list-versions` command to list all available versions of an extension</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-371">HDInsight</span></span>

* <span data-ttu-id="5550f-372">Включена поддержка создания кластера с конфигурацией автомасштабирования и поддержка управления конфигурацией автомасштабирования.</span><span class="sxs-lookup"><span data-stu-id="5550f-372">Support creating cluster with autoscale configuration and Support managing autoscale configuration</span></span>
* <span data-ttu-id="5550f-373">Включена поддержка создания кластера с шифрованием в узле.</span><span class="sxs-lookup"><span data-stu-id="5550f-373">Support creating cluster with encryption at host</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5550f-374">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-374">IoTCentral</span></span>

* <span data-ttu-id="5550f-375">Улучшения документации по CLI</span><span class="sxs-lookup"><span data-stu-id="5550f-375">CLI documentation improvements</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-376">Azure Monitor</span><span class="sxs-lookup"><span data-stu-id="5550f-376">Monitor</span></span>

* <span data-ttu-id="5550f-377">`az monitor metrics alert create`: включена поддержка RG и Sub в качестве значений области.</span><span class="sxs-lookup"><span data-stu-id="5550f-377">`az monitor metrics alert create`: support RG and Sub as the scope values</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-378">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-378">NetAppFiles</span></span>

* <span data-ttu-id="5550f-379">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] az netappfiles snapshot create: удален параметр file-system-id.</span><span class="sxs-lookup"><span data-stu-id="5550f-379">[BREAKING CHANGE] az netappfiles snapshot create: Removed file-system-id from parameters</span></span>
* <span data-ttu-id="5550f-380">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] az netappfiles snapshot show: удален параметр file-system-id.</span><span class="sxs-lookup"><span data-stu-id="5550f-380">[BREAKING CHANGE] az netappfiles snapshot show: Snapshot no longer has parameter file-system-id</span></span>
* <span data-ttu-id="5550f-381">`az netappfiles account`: в Model ActiveDirectory добавлен новый параметр backup_operators.</span><span class="sxs-lookup"><span data-stu-id="5550f-381">`az netappfiles account`: Model ActiveDirectory has a new parameter backup_operators</span></span>
* <span data-ttu-id="5550f-382">`az netappfiles volume show`: в Model dataProtection добавлен новый параметр snapshot.</span><span class="sxs-lookup"><span data-stu-id="5550f-382">`az netappfiles volume show`: Model dataProtection has a new parameter snapshot</span></span>
* <span data-ttu-id="5550f-383">`az netappfiles volume show`: в Model Volume добавлен новый параметр snapshot_directory_visible.</span><span class="sxs-lookup"><span data-stu-id="5550f-383">`az netappfiles volume show`: Model Volume has a new parameter snapshot_directory_visible</span></span>

### <a name="network"></a><span data-ttu-id="5550f-384">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-384">Network</span></span>

* <span data-ttu-id="5550f-385">`az network dns export`: экспорт FQDN для типов MX, PTR, NS и SRV вместо относительного пути.</span><span class="sxs-lookup"><span data-stu-id="5550f-385">`az network dns export`: export FQDN for MX, PTR, NS and SRV type instead of relative path</span></span>
* <span data-ttu-id="5550f-386">Включена поддержка Приватного канала для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5550f-386">Support private link for managed disks</span></span>
* <span data-ttu-id="5550f-387">`az network application-gateway auth-cert show`: добавлен пример для демонстрации формата сертификата.</span><span class="sxs-lookup"><span data-stu-id="5550f-387">`az network application-gateway auth-cert show`: Add example to demonstrate certificate format</span></span>
* <span data-ttu-id="5550f-388">`az network private-endpoint-connection`: включена поддержка конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-388">`az network private-endpoint-connection`: support app configuration</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-389">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-389">RBAC</span></span>

* <span data-ttu-id="5550f-390">`az ad group create`: включена поддержка указания описания при создании группы.</span><span class="sxs-lookup"><span data-stu-id="5550f-390">`az ad group create`: support specify description when creating a group</span></span>
* <span data-ttu-id="5550f-391">`az role definition create`: печать понятного для пользователя сообщения вместо исключения, если assignableScope является пустым массивом.</span><span class="sxs-lookup"><span data-stu-id="5550f-391">`az role definition create`: print human readable message instead of exception when assignableScope is an empty array</span></span>
* <span data-ttu-id="5550f-392">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az ad sp create-for-rbac`: изменены разрешения по умолчанию для созданного сертификата.</span><span class="sxs-lookup"><span data-stu-id="5550f-392">[BREAKING CHANGE] `az ad sp create-for-rbac`: change default permission of created certificate</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-393">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-393">SQL</span></span>

* <span data-ttu-id="5550f-394">`az sql server audit-policy`: включена поддержка аудита SQL Server.</span><span class="sxs-lookup"><span data-stu-id="5550f-394">`az sql server audit-policy`: Add sql server auditing support</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-395">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="5550f-395">Storage</span></span>

* <span data-ttu-id="5550f-396">`az storage blob copy start-batch`: Исправление № 6018: исправлен параметр --source-sas.</span><span class="sxs-lookup"><span data-stu-id="5550f-396">`az storage blob copy start-batch`: Fix #6018 for --source-sas</span></span>
* <span data-ttu-id="5550f-397">`az storage account or-policy`: включена поддержка политики репликации объектов учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-397">`az storage account or-policy`: Support storage account object replication policy</span></span>
* <span data-ttu-id="5550f-398">Исправлена ошибка № 14083 с обновлением версии пакета хранилища azure-multiapi-storage для выпуска пакета и включения поддержки новой версии API.</span><span class="sxs-lookup"><span data-stu-id="5550f-398">Fix issue #14083 to upgrade azure-multiapi-storage package version for package issue and new api version support</span></span>
* <span data-ttu-id="5550f-399">`az storage blob generate-sas`: добавлены примеры для параметра --ip и уточнено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-399">`az storage blob generate-sas`: add examples for --ip  and refine error message</span></span>
* <span data-ttu-id="5550f-400">`az storage blob list`: исправлена ошибка с next_marker.</span><span class="sxs-lookup"><span data-stu-id="5550f-400">`az storage blob list`: Fix next_marker issue</span></span>

### <a name="synapse"></a><span data-ttu-id="5550f-401">Synapse</span><span class="sxs-lookup"><span data-stu-id="5550f-401">Synapse</span></span>

* <span data-ttu-id="5550f-402">Добавлены командлеты, связанные с рабочей областью, пулом Spark и пулом SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-402">Add workspace, sparkpool, sqlpool related cmdlets</span></span>
* <span data-ttu-id="5550f-403">Добавлены команды, связанные с заданиями Spark, на основе пакета SDK для track2.</span><span class="sxs-lookup"><span data-stu-id="5550f-403">Add spark job releated commands based on track2 sdk</span></span>
* <span data-ttu-id="5550f-404">Добавлены команды, связанные с функцией управления доступом, на основе пакета SDK для track2.</span><span class="sxs-lookup"><span data-stu-id="5550f-404">Add accesscontrol feature related commands based on track2 sdk</span></span>

### <a name="upgrade"></a><span data-ttu-id="5550f-405">Обновление</span><span class="sxs-lookup"><span data-stu-id="5550f-405">Upgrade</span></span>

* <span data-ttu-id="5550f-406">Добавлена команда `az upgrade` для обновления Azure CLI и расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-406">Add `az upgrade` command to upgrade azure cli and extensions</span></span>

## <a name="august-11-2020"></a><span data-ttu-id="5550f-407">11 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-407">August 11, 2020</span></span>

<span data-ttu-id="5550f-408">Версия 2.10.1</span><span class="sxs-lookup"><span data-stu-id="5550f-408">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="5550f-409">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-409">App Service</span></span>

* <span data-ttu-id="5550f-410">Исправление № 9887: включена поддержка веб-приложений и приложений-функций, а также поддержка назначения и удаления управляемых удостоверений пользователя.</span><span class="sxs-lookup"><span data-stu-id="5550f-410">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="5550f-411">Исправление №№ 1382 и 14055: обновлены сообщения об ошибках для az webapp create и az webapp config container set.</span><span class="sxs-lookup"><span data-stu-id="5550f-411">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="5550f-412">`az webapp up`: исправлена логика выбора ASP по умолчанию, когда параметр --plan не указан.</span><span class="sxs-lookup"><span data-stu-id="5550f-412">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-413">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-413">AppConfig</span></span>

* <span data-ttu-id="5550f-414">Включена поддержка включения и отключения PublicNetworkAccess во время создания хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-414">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-415">Вычисления</span><span class="sxs-lookup"><span data-stu-id="5550f-415">Compute</span></span>

* <span data-ttu-id="5550f-416">Включена поддержка связывания диска и моментального снимка с ресурсом доступа к диску.</span><span class="sxs-lookup"><span data-stu-id="5550f-416">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-417">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-417">Lab</span></span>

* <span data-ttu-id="5550f-418">Исправлена ошибка № 7904, связанная с проверкой даты при создании виртуальной машины лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-418">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-419">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5550f-419">Storage</span></span>

* <span data-ttu-id="5550f-420">`az storage blob upload-batch`: исправлена ошибка № 14660, связанная с непозиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="5550f-420">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="5550f-421">04 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-421">August 04, 2020</span></span>

<span data-ttu-id="5550f-422">Версия 2.10.0</span><span class="sxs-lookup"><span data-stu-id="5550f-422">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-423">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-423">AKS</span></span>

* <span data-ttu-id="5550f-424">`az aks update`: изменен аргумент --enable-aad для переноса кластера с поддержкой RBAC за пределами AAD в управляемый AKS кластер AAD.</span><span class="sxs-lookup"><span data-stu-id="5550f-424">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="5550f-425">`az aks install-cli`: добавлены аргументы --kubelogin-version и --kubelogin-install-location для установки kubelogin.</span><span class="sxs-lookup"><span data-stu-id="5550f-425">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="5550f-426">Добавлена команда az aks nodepool get-upgrades.</span><span class="sxs-lookup"><span data-stu-id="5550f-426">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-427">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-427">AMS</span></span>

* <span data-ttu-id="5550f-428">Исправление № 14021: команда az ams account sp не является идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="5550f-428">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="5550f-429">APIM</span><span class="sxs-lookup"><span data-stu-id="5550f-429">APIM</span></span>

* <span data-ttu-id="5550f-430">apim api import: включена поддержка импорта API и расширены другие команды CLI уровня API.</span><span class="sxs-lookup"><span data-stu-id="5550f-430">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="5550f-431">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-431">App Service</span></span>

* <span data-ttu-id="5550f-432">Исправление № 13035: включена проверка для az webapp config access-restriction, чтобы предотвратить добавление дубликатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-432">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-433">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-433">AppConfig</span></span>

* <span data-ttu-id="5550f-434">По умолчанию используется номер SKU "Стандартный", если не указано другое.</span><span class="sxs-lookup"><span data-stu-id="5550f-434">Default to standard sku if not specified</span></span>
* <span data-ttu-id="5550f-435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Поддерживаются параметры с типом содержимого JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-435">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-436">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-436">ARM</span></span>

* <span data-ttu-id="5550f-437">`az resource tag`: исправлена ошибка с добавлением тегов managedApp и устранены некоторые проблемы, связанные с тестами.</span><span class="sxs-lookup"><span data-stu-id="5550f-437">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="5550f-438">`az deployment mg/tenant what-if`: включена поддержка What-If для группы управления и развертывания на уровне арендатора.</span><span class="sxs-lookup"><span data-stu-id="5550f-438">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="5550f-439">`az deployment mg/tenant create`: добавлен параметр --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="5550f-439">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="5550f-440">`az deployment mg/tenant create`: добавлен параметр --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="5550f-440">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="5550f-441">`az deployment mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="5550f-441">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="5550f-442">`az tag`: включена поддержка az tag для параметра идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-442">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-443">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-443">Backup</span></span>

* <span data-ttu-id="5550f-444">Обнаружение элемента или контейнера AFS активируется только при необходимости.</span><span class="sxs-lookup"><span data-stu-id="5550f-444">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-445">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-445">CDN</span></span>

* <span data-ttu-id="5550f-446">Добавлены поля Приватного канала в источник.</span><span class="sxs-lookup"><span data-stu-id="5550f-446">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-447">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-447">Compute</span></span>

* <span data-ttu-id="5550f-448">`az vm/vmss create`: возможность выбора допустимого имени пользователя, если имя пользователя по умолчанию является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="5550f-448">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="5550f-449">`az vm update`: включена поддержка образа для разных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="5550f-449">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="5550f-450">`az disk-access`: добавлена новая группа команд для использования ресурса доступа к диску.</span><span class="sxs-lookup"><span data-stu-id="5550f-450">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="5550f-451">Включена поддержка автоматического размещения выделенной группы узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-451">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="5550f-452">Включена поддержка ppg и spg в режиме оркестрации Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-452">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="5550f-453">Config</span><span class="sxs-lookup"><span data-stu-id="5550f-453">Config</span></span>

* <span data-ttu-id="5550f-454">`az config`: добавлен новый модуль команд `config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-454">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-455">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-455">Extension</span></span>

* <span data-ttu-id="5550f-456">Включена поддержка автоматической установки расширения, если расширение команды не установлено.</span><span class="sxs-lookup"><span data-stu-id="5550f-456">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-457">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-457">HDInsight</span></span>

* <span data-ttu-id="5550f-458">Добавлены три параметра в команду `az hdinsight create` для включения поддержки Приватного канала и шифрования в функции передачи:</span><span class="sxs-lookup"><span data-stu-id="5550f-458">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="5550f-459">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-459">Iot Hub</span></span>

* <span data-ttu-id="5550f-460">Исправление № 7792: создание Центра Интернета вещей не является идемпотентным.</span><span class="sxs-lookup"><span data-stu-id="5550f-460">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-461">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-461">IoT Central</span></span>

* <span data-ttu-id="5550f-462">Добавлен список вариантов параметра для IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5550f-462">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-463">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-463">KeyVault</span></span>

* <span data-ttu-id="5550f-464">`az keyvault key encrypt/decrypt`: добавлен параметр `--data-type` для явного определения типа исходных данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-464">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-465">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-465">Monitor</span></span>

* <span data-ttu-id="5550f-466">`az monitor log-analytics workspace data-export`: включена поддержка пространства имен концентратора событий в качестве назначения.</span><span class="sxs-lookup"><span data-stu-id="5550f-466">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="5550f-467">`az monitor autoscale`: включена поддержка пространства имен и измерений для --condition.</span><span class="sxs-lookup"><span data-stu-id="5550f-467">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-468">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-468">NetAppFiles</span></span>

* <span data-ttu-id="5550f-469">`az volume revert`:  включена поддержка возврата тома к одному из его моментальных снимков.</span><span class="sxs-lookup"><span data-stu-id="5550f-469">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="5550f-470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален командлет `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="5550f-470">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="5550f-471">`az volume show`: добавлен сайт в свойства Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5550f-471">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="5550f-472">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-472">Network</span></span>

* <span data-ttu-id="5550f-473">`az application-gateway private-link add`: включена поддержка определение существующей подсети по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="5550f-473">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="5550f-474">`az network application-gateway waf-policy create`: включена поддержка версии и типа.</span><span class="sxs-lookup"><span data-stu-id="5550f-474">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-475">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-475">Storage</span></span>

* <span data-ttu-id="5550f-476">Исправление № 10302: включена поддержка подбора типа содержимого при синхронизации файлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-476">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="5550f-477">`az storage blob lease`: добавлена возможность применить новую версию API для операций аренды BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-477">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="5550f-478">`az storage fs access`: включена поддержка учетных данных AAD при управлении доступом для учетной записи ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="5550f-478">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="5550f-479">`az storage share-rm create/update`: добавлен аргумент --access-tier для включения поддержки уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="5550f-479">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="5550f-480">16 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-480">July 16, 2020</span></span>

<span data-ttu-id="5550f-481">Версия 2.9.1</span><span class="sxs-lookup"><span data-stu-id="5550f-481">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-482">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-482">AKS</span></span>

* <span data-ttu-id="5550f-483">Явный параметр VMSS в примере команды для Windows удален, так как он теперь используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-483">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-484">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-484">IoT</span></span>

* <span data-ttu-id="5550f-485">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az iot pnp`: удаление предварительной версии команд IoT PNP из основной версии CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-485">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="5550f-486">REST</span><span class="sxs-lookup"><span data-stu-id="5550f-486">REST</span></span>

* <span data-ttu-id="5550f-487">Исправлена ошибка № 14152. `az rest`: URL-адреса ARM принимаются без идентификатора подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-487">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-488">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-488">Storage</span></span>

* <span data-ttu-id="5550f-489">Исправлена ошибка № 14138. Некоторые разрешения стали необязательными.</span><span class="sxs-lookup"><span data-stu-id="5550f-489">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="5550f-490">14 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-490">July 14, 2020</span></span>

<span data-ttu-id="5550f-491">Версия 2.9.0</span><span class="sxs-lookup"><span data-stu-id="5550f-491">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-492">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-492">ACR</span></span>

* <span data-ttu-id="5550f-493">Обработка ссылки на артефакт журнала из реестра для потоковой передачи журналов.</span><span class="sxs-lookup"><span data-stu-id="5550f-493">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="5550f-494">Устарели команды helm2.</span><span class="sxs-lookup"><span data-stu-id="5550f-494">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-495">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-495">AKS</span></span>

* <span data-ttu-id="5550f-496">`az aks create`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="5550f-496">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="5550f-497">`az aks update`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="5550f-497">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="5550f-498">APIM</span><span class="sxs-lookup"><span data-stu-id="5550f-498">APIM</span></span>

* <span data-ttu-id="5550f-499">Добавлены общие команды az apim api.</span><span class="sxs-lookup"><span data-stu-id="5550f-499">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-500">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-500">AppConfig</span></span>

* <span data-ttu-id="5550f-501">Добавлен пример для использования --fields в appconfig revision.</span><span class="sxs-lookup"><span data-stu-id="5550f-501">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-502">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-502">AppService</span></span>

* <span data-ttu-id="5550f-503">`az functionapp create`: включена поддержка Java 11 и PowerShell 7.</span><span class="sxs-lookup"><span data-stu-id="5550f-503">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="5550f-504">Включена поддержка API стеков.</span><span class="sxs-lookup"><span data-stu-id="5550f-504">Added Stacks API Support.</span></span>
* <span data-ttu-id="5550f-505">Исправлена ошибка № 14208, из-за которой создание многоконтейнерного приложения завершается сбоем.</span><span class="sxs-lookup"><span data-stu-id="5550f-505">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="5550f-506">Исправлена ошибка с az webapp create, связанная с использованием вписанных в код стеков среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-506">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-507">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-507">ARM</span></span>

* <span data-ttu-id="5550f-508">`az resource tag`: исправлена ошибка, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerInstance/containerGroups`.</span><span class="sxs-lookup"><span data-stu-id="5550f-508">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-509">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-509">Compute</span></span>

* <span data-ttu-id="5550f-510">Выполнено обновление версии дисков до 2020-05-01 и вычислительных ресурсов до 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-510">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="5550f-511">Включено двойное шифрование набора шифрования диска.</span><span class="sxs-lookup"><span data-stu-id="5550f-511">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="5550f-512">`az vmss update`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-512">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="5550f-513">`az sig image-version create`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-513">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="5550f-514">vm/vmss create. Включено шифрование кэша и передаваемых данных для дисков ОС и данных и временных дисков для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-514">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="5550f-515">Добавлена операция имитации удаления для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-515">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-516">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-516">CosmosDB</span></span>

* <span data-ttu-id="5550f-517">Последние компоненты: Autoscale, IpRules, EnableFreeTier и EnableAnalyticalStorage.</span><span class="sxs-lookup"><span data-stu-id="5550f-517">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5550f-518">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5550f-518">EventGrid</span></span>

* <span data-ttu-id="5550f-519">Включена поддержка CLI для 2020-04-01-preview и отмечены предварительные версии функций как is_Preview=true.</span><span class="sxs-lookup"><span data-stu-id="5550f-519">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="5550f-520">Поиск</span><span class="sxs-lookup"><span data-stu-id="5550f-520">Find</span></span>

* <span data-ttu-id="5550f-521">Исправлена ошибка № 14094, связанная с az find. Исправлена ошибка, из-за которой не удается войти при отключенной телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-521">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-522">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-522">HDInsight</span></span>

* <span data-ttu-id="5550f-523">Добавлены две команды для перезагрузки узла HDInsight.</span><span class="sxs-lookup"><span data-stu-id="5550f-523">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-524">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-524">Monitor</span></span>

* <span data-ttu-id="5550f-525">Удален флаг предварительной версии для команд в рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-525">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="5550f-526">`az monitor diagnostic-settings subscription`: включена поддержка параметров диагностики для подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-526">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="5550f-527">`az monitor metrics`: включена поддержка символов "," и "|" в именах метрик.</span><span class="sxs-lookup"><span data-stu-id="5550f-527">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="5550f-528">`az monitor log-analytics workspace data-export`: включена поддержка экспорта данных аналитики журнала.</span><span class="sxs-lookup"><span data-stu-id="5550f-528">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="5550f-529">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-529">Network</span></span>

* <span data-ttu-id="5550f-530">`az network application-gateway frontend-ip update`: Устарел параметр --public-ip-address.</span><span class="sxs-lookup"><span data-stu-id="5550f-530">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="5550f-531">Выполнено обновление azure-mgmt-network до 11.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-531">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="5550f-532">`az network express-route gateway connection`: включена конфигурация маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="5550f-532">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="5550f-533">`az network virtual-appliance`: Включена поддержка сетевого виртуального устройства Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-533">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="5550f-534">Включена поддержка компонента Приватного канала в Шлюзе приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-534">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="5550f-535">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5550f-535">PolicyInsights</span></span>

* <span data-ttu-id="5550f-536">`az policy state`: добавлена команда trigger-scan для активации оценки соответствия политикам.</span><span class="sxs-lookup"><span data-stu-id="5550f-536">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="5550f-537">`az policy state list`: предоставлены версии сущностей политики в каждой записи соответствия.</span><span class="sxs-lookup"><span data-stu-id="5550f-537">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-538">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-538">Profile</span></span>

* <span data-ttu-id="5550f-539">`az account get-access-token`: включено отображение expiresOn для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5550f-539">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-540">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-540">RDBMS</span></span>

* <span data-ttu-id="5550f-541">Включена поддержка минимальной версии TLS.</span><span class="sxs-lookup"><span data-stu-id="5550f-541">Support Minimum TLS version</span></span>
* <span data-ttu-id="5550f-542">Включено шифрование инфраструктуры для Azure Postgres и MySQL</span><span class="sxs-lookup"><span data-stu-id="5550f-542">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="5550f-543">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5550f-543">Security</span></span>

* <span data-ttu-id="5550f-544">Добавлены команды allowed_connections.</span><span class="sxs-lookup"><span data-stu-id="5550f-544">Add allowed_connections commands</span></span>
* <span data-ttu-id="5550f-545">Добавлены команды адаптивного усиления защиты сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-545">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="5550f-546">Добавлены команды adaptive_application_controls.</span><span class="sxs-lookup"><span data-stu-id="5550f-546">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="5550f-547">Добавлены команды REST az security iot-solution/iot-alerts/iot-recommendations/iot-analytics в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-547">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="5550f-548">Добавлен интерфейс командной строки для обеспечения соответствия нормативным требованиям.</span><span class="sxs-lookup"><span data-stu-id="5550f-548">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="5550f-549">SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-549">SignalR</span></span>

* <span data-ttu-id="5550f-550">Добавлены возможности, включая управление подключениями к частным конечным точкам, сетевыми правилами и вышестоящими компонентами.</span><span class="sxs-lookup"><span data-stu-id="5550f-550">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-551">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-551">SQL</span></span>

* <span data-ttu-id="5550f-552">`az sql mi create`, `az sql mi update`: добавлен параметр `--tags` для поддержки тегов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-552">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="5550f-553">`az sql mi failover`: включена поддержка отработки отказа с основного сайта на дополнительный.</span><span class="sxs-lookup"><span data-stu-id="5550f-553">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-554">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-554">Storage</span></span>

* <span data-ttu-id="5550f-555">`az storage account create/update`: добавлен параметр --allow-blob-public-access для включения и отключения общего доступа к большим двоичным объектам и контейнерам.</span><span class="sxs-lookup"><span data-stu-id="5550f-555">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="5550f-556">`az storage account create/update`: добавлен параметр `--min-tls-version` для настройки минимальной версии TLS, используемой при выполнении запросов к хранилищу.</span><span class="sxs-lookup"><span data-stu-id="5550f-556">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="5550f-557">Удален возврат учетных данных маркера.</span><span class="sxs-lookup"><span data-stu-id="5550f-557">Remove check in token credential</span></span>
* <span data-ttu-id="5550f-558">Исправлено имя учетной записи хранения в примерах.</span><span class="sxs-lookup"><span data-stu-id="5550f-558">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="5550f-559">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="5550f-559">Webapp</span></span>

* <span data-ttu-id="5550f-560">Исправление. az webapp log deployment show: возврат журналов развертывания вместо метаданных журнала.</span><span class="sxs-lookup"><span data-stu-id="5550f-560">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="5550f-561">Исправление. az webapp vnet-integration add: исправлена обработка ошибок при неправильном имени виртуальной сети и включена поддержка идентификатора ресурса виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-561">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="5550f-562">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="5550f-562">June 23, 2020</span></span>

<span data-ttu-id="5550f-563">Версия 2.8.0</span><span class="sxs-lookup"><span data-stu-id="5550f-563">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-564">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-564">ACR</span></span>

* <span data-ttu-id="5550f-565">Добавлена поддержка отключения конечных точек региона и отключения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="5550f-565">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="5550f-566">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az acr login --expose-token` не принимает имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="5550f-566">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-567">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-567">ACS</span></span>

* <span data-ttu-id="5550f-568">Удален частный кластер и API 2019-10-27-preview.</span><span class="sxs-lookup"><span data-stu-id="5550f-568">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-569">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-569">AKS</span></span>

* <span data-ttu-id="5550f-570">Включена поддержка параметра --yes для команды az aks upgrade.</span><span class="sxs-lookup"><span data-stu-id="5550f-570">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="5550f-571">Отменено изменение SKU виртуальной машины по умолчанию на Standard_D2s_v3 (№ 13541).</span><span class="sxs-lookup"><span data-stu-id="5550f-571">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="5550f-572">Добавлена команда az aks update --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="5550f-572">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="5550f-573">Исправлена опечатка в команде az aks update.</span><span class="sxs-lookup"><span data-stu-id="5550f-573">Fix typo in az aks update command</span></span>
* <span data-ttu-id="5550f-574">Включена поддержка пула агентов узла 0 и блокировка ручного масштабирования для пула с поддержкой CAS.</span><span class="sxs-lookup"><span data-stu-id="5550f-574">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="5550f-575">Исправлена опечатка в VirtualMachineScaleSets и обновлены ссылки на версии Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-575">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-576">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-576">AMS</span></span>

* <span data-ttu-id="5550f-577">Изменен текст справки по параметру --expires.</span><span class="sxs-lookup"><span data-stu-id="5550f-577">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-578">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-578">AppService</span></span>

* <span data-ttu-id="5550f-579">`az webapp log deployment show`: включено отображение журнала последнего развертывания или журналов конкретного развертывания, если указан идентификатор развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-579">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="5550f-580">`az webapp log deployment list`: список доступных журналов развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-580">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="5550f-581">Исправление: ошибка поверхности при указании недопустимого имени веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-581">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="5550f-582">Исправлена ошибка № 13261, и-за которой az webapp list-runtimes использует статический список до появления новых доступных API стеков.</span><span class="sxs-lookup"><span data-stu-id="5550f-582">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="5550f-583">`az appservice ase create`: исправлена ошибка создания № 13361.</span><span class="sxs-lookup"><span data-stu-id="5550f-583">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="5550f-584">`az appservice ase list-addresses`: исправлена ошибка изменения SDK № 13140.</span><span class="sxs-lookup"><span data-stu-id="5550f-584">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="5550f-585">Исправлена ошибка создания слота или веб-приложения для контейнеров Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-585">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="5550f-586">`az webapp auth update`: добавлен необязательный параметр для обновления версии среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-586">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="5550f-587">Включена поддержка перечисления, удаления, утверждения и отклонения подключения к частной конечной точке для веб-приложения в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="5550f-587">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="5550f-588">Исправлена ошибка № 13888: включена поддержка команд get, list, create для статических веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-588">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="5550f-589">Улучшены сообщения об ошибках для подключения туннеля SSH.</span><span class="sxs-lookup"><span data-stu-id="5550f-589">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-590">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-590">ARM</span></span>

* <span data-ttu-id="5550f-591">`az tag`: добавлены примеры для параметра -h.</span><span class="sxs-lookup"><span data-stu-id="5550f-591">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="5550f-592">`az deployment group/sub what-if`: добавлен параметр --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="5550f-592">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="5550f-593">`az deployment group/sub/mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="5550f-593">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="5550f-594">`az deployment group/sub/mg/tenant validate`: улучшен формат отображения сообщений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5550f-594">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="5550f-595">`az group export`: добавлены новые параметры `--skip-resource-name-params` и `--skip-all-params` для включения поддержки параметризации с целью пропуска.</span><span class="sxs-lookup"><span data-stu-id="5550f-595">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="5550f-596">Добавлена команда az feature unregister api.</span><span class="sxs-lookup"><span data-stu-id="5550f-596">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-597">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-597">ARO</span></span>

* <span data-ttu-id="5550f-598">Добавлены атрибуты Public и Private в параметры для получения справки по видимости входящего трафика или сервера API.</span><span class="sxs-lookup"><span data-stu-id="5550f-598">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-599">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-599">Batch</span></span>

* <span data-ttu-id="5550f-600">`az batch account create`: добавлен новый параметр `--public-network-access`.</span><span class="sxs-lookup"><span data-stu-id="5550f-600">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="5550f-601">`az batch account create`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-601">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="5550f-602">`az batch account set`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-602">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="5550f-603">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с помощью пользовательского образа свойство --image теперь может ссылаться только на образ Общей коллекции образов.</span><span class="sxs-lookup"><span data-stu-id="5550f-603">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="5550f-604">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с параметром --json-file и указании networkConfiguration свойство publicIPs было перемещено в новое свойство publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5550f-604">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="5550f-605">Это новое свойство также поддерживает новое свойство ipAddressProvisioningType, которое определяет, как пул должен выделять IP-адреса, и свойство publicIPs, которое позволяет настроить список ресурсов PublicIP для использования, когда для ipAddressProvisioningType указано значение UserManaged.</span><span class="sxs-lookup"><span data-stu-id="5550f-605">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="5550f-606">`az network private-link-resource`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="5550f-606">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="5550f-607">`az network private-endpoint-connection`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="5550f-607">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-608">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-608">CDN</span></span>

* <span data-ttu-id="5550f-609">`az cdn custom-domain enable-https`: включена поддержка BYOC.</span><span class="sxs-lookup"><span data-stu-id="5550f-609">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="5550f-610">`az cdn custom-domain enable-https`: исправлена ошибка включения пользовательского HTTPS с использованием управляемых CDN сертификатов для SKU Standard_Verizon и Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5550f-610">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-611">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-611">Cognitive Services</span></span>

* <span data-ttu-id="5550f-612">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az cognitiveservices account` теперь имеет единую структуру для всех команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-612">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="5550f-613">`az cognitiveservices account identity`: добавлена возможность управления удостоверениями для Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5550f-613">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-614">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-614">Compute</span></span>

* <span data-ttu-id="5550f-615">`az image builder`: обновлена версия API до 2020-02-14.</span><span class="sxs-lookup"><span data-stu-id="5550f-615">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="5550f-616">`az image builder create`: добавлен параметр `--identity` для включения поддержки конфигурации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5550f-616">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="5550f-617">`az image builder customizer add`: включена поддержка настройщика Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-617">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="5550f-618">Новая команда `az image builder cancel`.</span><span class="sxs-lookup"><span data-stu-id="5550f-618">New command `az image builder cancel`</span></span>
* <span data-ttu-id="5550f-619">Включено отображение предупреждения, когда пользователь развертывает VMSS, прикрепленные к конкретной версии образа, а не к последней.</span><span class="sxs-lookup"><span data-stu-id="5550f-619">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-620">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-620">Cosmos DB</span></span>

* <span data-ttu-id="5550f-621">`az cosmosdb`: добавлена команда exists в базу данных и группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-621">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="5550f-622">Разрешено создание фиксированных коллекций.</span><span class="sxs-lookup"><span data-stu-id="5550f-622">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-623">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-623">EventHub</span></span>

* <span data-ttu-id="5550f-624">`az eventhubs namespace create` : добавлены параметры управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5550f-624">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-625">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-625">Extension</span></span>

* <span data-ttu-id="5550f-626">Добавлен параметр --version для включения поддержки установки из конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-626">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="5550f-627">Включены расширения CLI для включения пакетов в пространство имен Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-627">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="5550f-628">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-628">Iot Hub</span></span>

* <span data-ttu-id="5550f-629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az iot hub job: удалены устаревшие команды заданий.</span><span class="sxs-lookup"><span data-stu-id="5550f-629">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-630">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-630">KeyVault</span></span>

* <span data-ttu-id="5550f-631">`az keyvault key import`: включена поддержка импорта из строк с помощью двух новых параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-631">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="5550f-632">Включена поддержка шифрования и расшифровки строк или байтов с помощью хранимых ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-632">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-633">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-633">Monitor</span></span>

* <span data-ttu-id="5550f-634">Включена поддержка возможности не дожидаться создания кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-634">Support no wait for cluster creation</span></span>
* <span data-ttu-id="5550f-635">`az monitor log-analytics workspace saved-search`: включена поддержка новых команд для сохраненного поиска.</span><span class="sxs-lookup"><span data-stu-id="5550f-635">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="5550f-636">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-636">Network</span></span>

* <span data-ttu-id="5550f-637">`az network application-gateway address-pool update`: уточнено справочное сообщение и добавлены примеры.</span><span class="sxs-lookup"><span data-stu-id="5550f-637">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="5550f-638">`az network vnet create`: включена поддержка аргумента --nsg.</span><span class="sxs-lookup"><span data-stu-id="5550f-638">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="5550f-639">`az network lb address-pool`: включена поддержка создания внутреннего пула балансировки нагрузки с внутренним адресом.</span><span class="sxs-lookup"><span data-stu-id="5550f-639">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="5550f-640">`az network application-gateway address-pool`: исправлена ошибка с аргументом --add.</span><span class="sxs-lookup"><span data-stu-id="5550f-640">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-641">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-641">RBAC</span></span>

* <span data-ttu-id="5550f-642">`az ad sp create-for-rabc`: включена поддержка имен с пробелом, косой чертой и обратной косой чертой.</span><span class="sxs-lookup"><span data-stu-id="5550f-642">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="5550f-643">`az ad sp create-for-rbac`: уточнено сообщение об ошибке при указании недопустимой области пользователем.</span><span class="sxs-lookup"><span data-stu-id="5550f-643">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="5550f-644">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5550f-644">Security</span></span>

* <span data-ttu-id="5550f-645">Добавлены команды оценки безопасности.</span><span class="sxs-lookup"><span data-stu-id="5550f-645">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-646">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-646">SQL</span></span>

* <span data-ttu-id="5550f-647">`az sql db ltr-policy/ltr-backup`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="5550f-647">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-648">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-648">Storage</span></span>

* <span data-ttu-id="5550f-649">Исправлена проблема с проверкой подлинности для включения поддержки получения токена для параметра --subscription.</span><span class="sxs-lookup"><span data-stu-id="5550f-649">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="5550f-650">`az storage remove`: исправлена ошибка № 13459 с возникновением исключения при сбое операции.</span><span class="sxs-lookup"><span data-stu-id="5550f-650">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="5550f-651">Устранены ошибки № 13012, 13632 и 13657 для удаления неиспользуемых аргументов для команд, связанных с generate-sas.</span><span class="sxs-lookup"><span data-stu-id="5550f-651">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="5550f-652">`az storage logging update`: добавлена проверка версии ведения журнала.</span><span class="sxs-lookup"><span data-stu-id="5550f-652">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="5550f-653">`az storage blob show`: добавлены дополнительные свойства для большого двоичного объекта с использованием пакета SDK для Track 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-653">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="5550f-654">Исправление № 13708: уточнены предупреждающие сообщения об учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-654">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="5550f-655">`az storage share-rm create/update`: включена поддержка протокола NFS и корневого сжатия.</span><span class="sxs-lookup"><span data-stu-id="5550f-655">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="5550f-656">`az storage account create`: включена поддержка двойного шифрования.</span><span class="sxs-lookup"><span data-stu-id="5550f-656">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="5550f-657">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az storage blob/container/file/share/table/queue generate-sas`: параметры --expiry и --permissions являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="5550f-657">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="5550f-658">`az storage blob set-tier`: миграция на Track 2 для включения поддержки настройки приоритета восстановления.</span><span class="sxs-lookup"><span data-stu-id="5550f-658">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="5550f-659">02 июня 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-659">June 02, 2020</span></span>

<span data-ttu-id="5550f-660">Версия 2.7.0</span><span class="sxs-lookup"><span data-stu-id="5550f-660">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-661">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-661">ACR</span></span>

* <span data-ttu-id="5550f-662">Исправлена опечатка в сообщении об ошибке, возникающем при создании токена.</span><span class="sxs-lookup"><span data-stu-id="5550f-662">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-663">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-663">AKS</span></span>

* <span data-ttu-id="5550f-664">Номер SKU виртуальной машины по умолчанию изменен на Standard_D2s_v3.</span><span class="sxs-lookup"><span data-stu-id="5550f-664">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="5550f-665">Исправлен процесс создания назначения ролей для кластера MSI и настраиваемой подсети.</span><span class="sxs-lookup"><span data-stu-id="5550f-665">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-666">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-666">AppService</span></span>

* <span data-ttu-id="5550f-667">Исправлена ошибка 12739, из-за которой команда az appservice list-locations возвращает недопустимые расположения.</span><span class="sxs-lookup"><span data-stu-id="5550f-667">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-668">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-668">ARM</span></span>

* <span data-ttu-id="5550f-669">`az deployment`: Исправлена ошибка 13159, из-за которой отображается неправильное сообщение JSON после удаления комментариев и сжатия.</span><span class="sxs-lookup"><span data-stu-id="5550f-669">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="5550f-670">`az resource tag`: Исправлена ошибка 13255, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerRegistry/registries/webhooks`.</span><span class="sxs-lookup"><span data-stu-id="5550f-670">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="5550f-671">Улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-671">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-672">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-672">ARO</span></span>

* <span data-ttu-id="5550f-673">Исправлена ошибка CLIError, связанная с неправильным флагом для --worker-vm-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="5550f-673">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-674">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-674">EventHub</span></span>

* <span data-ttu-id="5550f-675">Исправлена ошибка 12406, из-за которой аргумент --capture-interval не обновляет intervalInSeconds.</span><span class="sxs-lookup"><span data-stu-id="5550f-675">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-676">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-676">HDInsight</span></span>

* <span data-ttu-id="5550f-677">Объект get_json_object изменен на shell_safe_json_parse.</span><span class="sxs-lookup"><span data-stu-id="5550f-677">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-678">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-678">Monitor</span></span>

* <span data-ttu-id="5550f-679">`az monitor metrics alert`: уточнены нескольких справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="5550f-679">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="5550f-680">`az monitor diagnostic-settings create`: включена поддержка аргумента --export-to-resource-specific.</span><span class="sxs-lookup"><span data-stu-id="5550f-680">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="5550f-681">Включена поддержка восстановления рабочей области LA.</span><span class="sxs-lookup"><span data-stu-id="5550f-681">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="5550f-682">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-682">Network</span></span>

* <span data-ttu-id="5550f-683">`az network dns zone`: включена поддержка символа -.</span><span class="sxs-lookup"><span data-stu-id="5550f-683">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="5550f-684">`az network vpn-connection ipsec-policy`: изменены значения --sa-lifetime и --sa-max-size на более крупные в примере.</span><span class="sxs-lookup"><span data-stu-id="5550f-684">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="5550f-685">Обновление сети до версии 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="5550f-685">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="5550f-686">`az network private-endpoint-connection`: включена поддержка Сетки событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-686">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="5550f-687">`az network express-route list-route-tables`: исправлена ошибка, из-за которой нельзя было перечислять маршруты в виде таблицы.</span><span class="sxs-lookup"><span data-stu-id="5550f-687">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-688">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-688">Packaging</span></span>

* <span data-ttu-id="5550f-689">Добавлен пакет Ubuntu Focal.</span><span class="sxs-lookup"><span data-stu-id="5550f-689">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-690">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-690">RBAC</span></span>

* <span data-ttu-id="5550f-691">`az ad sp credential reset`: изменен процесс создания учетных данных, чтобы не использовать проблемные специальные символы.</span><span class="sxs-lookup"><span data-stu-id="5550f-691">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-692">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-692">Redis</span></span>

* <span data-ttu-id="5550f-693">Исправление 13529: изменена документация по параметру enable_non_ssl_port.</span><span class="sxs-lookup"><span data-stu-id="5550f-693">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-694">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-694">Storage</span></span>

* <span data-ttu-id="5550f-695">`az storage copy`: Добавлен параметр `--follow-symlinks` для включения поддержки символических ссылок.</span><span class="sxs-lookup"><span data-stu-id="5550f-695">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="5550f-696">Включен локальный контекст для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-696">Enable local context for storage account</span></span>
* <span data-ttu-id="5550f-697">`az storage logging`: Исправление 11969: уточнено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-697">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="5550f-698">19 мая 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-698">May 19, 2020</span></span>

<span data-ttu-id="5550f-699">Версия 2.6.0</span><span class="sxs-lookup"><span data-stu-id="5550f-699">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-700">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-700">ACR</span></span>

* <span data-ttu-id="5550f-701">Добавлено время ожидания по умолчанию (5 минут) для любых запросов ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-701">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="5550f-702">Добавлена поддержка отключения доступа к общедоступной сети</span><span class="sxs-lookup"><span data-stu-id="5550f-702">Support disable public network access</span></span>
* <span data-ttu-id="5550f-703">`az acr token create`: предоставляет аргумент --days</span><span class="sxs-lookup"><span data-stu-id="5550f-703">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="5550f-704">`az acr import`: принимает значения аргумента --source, которые содержат имя для входа в имени сервера, добавленное путем исправления на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="5550f-704">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-705">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-705">ACS</span></span>

* <span data-ttu-id="5550f-706">Исправление ошибки: удаление больше не существующих полей</span><span class="sxs-lookup"><span data-stu-id="5550f-706">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-707">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-707">AKS</span></span>

* <span data-ttu-id="5550f-708">Обновлен контекст справки команды uptime-sla</span><span class="sxs-lookup"><span data-stu-id="5550f-708">Update uptime-sla command help context</span></span>
* <span data-ttu-id="5550f-709">Удалена проверка диапазона для обновления числа минут для автомасштабирования</span><span class="sxs-lookup"><span data-stu-id="5550f-709">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="5550f-710">Исправлена ошибка, из-за которой CLI не выдает ошибку, когда пользователь указывает только пароль Windows</span><span class="sxs-lookup"><span data-stu-id="5550f-710">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-711">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-711">AMS</span></span>

* <span data-ttu-id="5550f-712">`az ams transform create`: добавлена возможность создания преобразования с предустановкой FaceDetector</span><span class="sxs-lookup"><span data-stu-id="5550f-712">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="5550f-713">`az ams content-key-policy create` : добавлена возможность создания политики ключа содержимого FairPlay с конфигурацией автономной аренды</span><span class="sxs-lookup"><span data-stu-id="5550f-713">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-714">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-714">AppConfig</span></span>

* <span data-ttu-id="5550f-715">Исправлена ошибка при отображении значений ключей с полями</span><span class="sxs-lookup"><span data-stu-id="5550f-715">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-716">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-716">AppService</span></span>

* <span data-ttu-id="5550f-717">`az functionapp create`: параметр AzureWebJobsDashboard будет задан только в случае отключения AppInsights</span><span class="sxs-lookup"><span data-stu-id="5550f-717">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="5550f-718">Исправление № 10664 — интеграция виртуальной сети — проблема проверки расположения и исправление № 13257 — сбой веб-приложения az в случае необходимости создания группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="5550f-718">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="5550f-719">`az webapp|functionapp config ssl import`: добавлен поиск хранилища ключей в группах ресурсов в подписке и улучшены справка и примеры.</span><span class="sxs-lookup"><span data-stu-id="5550f-719">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="5550f-720">Подключен локальный контекст для службы приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-720">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-721">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-721">ARM</span></span>

* <span data-ttu-id="5550f-722">`az deployment`: устранена проблема, из-за которой templateLink не возвращается при развертывании или проверке template-uri</span><span class="sxs-lookup"><span data-stu-id="5550f-722">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="5550f-723">`az deployment`: устранена проблема, из-за которой развертывание или проверка не поддерживает специально закодированный символ</span><span class="sxs-lookup"><span data-stu-id="5550f-723">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="5550f-724">`az deployment sub/group what-if`: исправлены выравнивание массива и обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="5550f-724">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="5550f-725">`az deployment operation`: изменение сведений об устаревании</span><span class="sxs-lookup"><span data-stu-id="5550f-725">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-726">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-726">ARO</span></span>

* <span data-ttu-id="5550f-727">Добавлены примеры в az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="5550f-727">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="5550f-728">Добавлена функция generate_random_id</span><span class="sxs-lookup"><span data-stu-id="5550f-728">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-729">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-729">Backup</span></span>

* <span data-ttu-id="5550f-730">Разрешен параметр FriendlyName при включении защиты для команды AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="5550f-730">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="5550f-731">Исправлена restore-disks в IaasVM</span><span class="sxs-lookup"><span data-stu-id="5550f-731">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="5550f-732">Добавлен тип BackupManagementType "MAB" в команду item list</span><span class="sxs-lookup"><span data-stu-id="5550f-732">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="5550f-733">Добавлена поддержка повторного обновления политики для элементов с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5550f-733">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="5550f-734">Добавлена функция защиты от возобновления для виртуальной машины Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-734">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="5550f-735">Добавлена поддержка возможности указывать группу ресурсов для хранения instantRP во время создания или изменения политики</span><span class="sxs-lookup"><span data-stu-id="5550f-735">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="5550f-736">CI</span><span class="sxs-lookup"><span data-stu-id="5550f-736">CI</span></span>

* <span data-ttu-id="5550f-737">Поддержка flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="5550f-737">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-738">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-738">Compute</span></span>

* <span data-ttu-id="5550f-739">Новая команда az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="5550f-739">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="5550f-740">`az vm list-skus`: обновлено поведение для параметра --zone — теперь он возвращает все номера SKU типов</span><span class="sxs-lookup"><span data-stu-id="5550f-740">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="5550f-741">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-741">Core</span></span>

* <span data-ttu-id="5550f-742">Обновлено состояние включения и выключения локального контекста на уровне глобального пользователя</span><span class="sxs-lookup"><span data-stu-id="5550f-742">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-743">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-743">Extension</span></span>

* <span data-ttu-id="5550f-744">`az extension add`: добавлен параметр --system для включения установки расширений по системному пути</span><span class="sxs-lookup"><span data-stu-id="5550f-744">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="5550f-745">Реализована поддержка .egg-info для хранения метаданных расширения типа wheel</span><span class="sxs-lookup"><span data-stu-id="5550f-745">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-746">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-746">IoT</span></span>

* <span data-ttu-id="5550f-747">`az iot`: теперь в сообщении для информирования о первом запуске модуля команд Интернета вещей используется точный и современный идентификатор `azure-iot`, который не считается нерекомендуемым.</span><span class="sxs-lookup"><span data-stu-id="5550f-747">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="5550f-748">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-748">IoT Hub</span></span>

* <span data-ttu-id="5550f-749">Добавлена поддержка API 2020-03-01 и команд сетевой изоляции</span><span class="sxs-lookup"><span data-stu-id="5550f-749">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-750">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-750">NetAppFiles</span></span>

* <span data-ttu-id="5550f-751">`az volume create`: добавлен параметр snapshot-id для создания тома. Это позволит пользователям создавать тома из существующего моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="5550f-751">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="5550f-752">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-752">Network</span></span>

* <span data-ttu-id="5550f-753">Исправлена ошибка, из-за которой значение ttl изменялось непредвиденным образом для add-record для dns</span><span class="sxs-lookup"><span data-stu-id="5550f-753">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="5550f-754">`az network public-ip create`: информирование клиентов о выпуске критического изменения</span><span class="sxs-lookup"><span data-stu-id="5550f-754">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="5550f-755">Поддержка универсальных команд для сценария Приватного канала</span><span class="sxs-lookup"><span data-stu-id="5550f-755">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="5550f-756">`az network private-endpoint-connection`: поддержка типов mysql, postgre и mariadb</span><span class="sxs-lookup"><span data-stu-id="5550f-756">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="5550f-757">`az network private-endpoint-connection`: поддержка типов cosmosdb</span><span class="sxs-lookup"><span data-stu-id="5550f-757">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="5550f-758">`az network private-endpoint`: параметр --group-ids теперь является нерекомендуемым и перенаправляется на --group-id</span><span class="sxs-lookup"><span data-stu-id="5550f-758">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="5550f-759">Выходные данные</span><span class="sxs-lookup"><span data-stu-id="5550f-759">Output</span></span>

* <span data-ttu-id="5550f-760">Отображение обновленной инструкции для find, feedback и --help</span><span class="sxs-lookup"><span data-stu-id="5550f-760">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-761">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-761">Packaging</span></span>

* <span data-ttu-id="5550f-762">Создание пакетов MSI/Homebrew с зависимостями, разрешенным из requirements.txt</span><span class="sxs-lookup"><span data-stu-id="5550f-762">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-763">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-763">RBAC</span></span>

* <span data-ttu-id="5550f-764">`az ad sp credential reset`: устранена возможность создания слабых учетных данных</span><span class="sxs-lookup"><span data-stu-id="5550f-764">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-765">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-765">Storage</span></span>

* <span data-ttu-id="5550f-766">`az storage account file-service-properties update/show`: добавлена поддержка свойств файлов для учетной записи хранения</span><span class="sxs-lookup"><span data-stu-id="5550f-766">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="5550f-767">`az storage container create`: исправление № 13373 путем добавления проверяющего элемента управления для общего доступа</span><span class="sxs-lookup"><span data-stu-id="5550f-767">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="5550f-768">Добавлена поддержка track2 для ADLS 2-го поколения</span><span class="sxs-lookup"><span data-stu-id="5550f-768">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="5550f-769">`az storage blob sync`: Включена поддержка `--connection-string`.</span><span class="sxs-lookup"><span data-stu-id="5550f-769">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="5550f-770">`az storage blob sync`: исправлено неверное сообщение об ошибке, которое отображается, когда azcopy не удается найти расположение установки</span><span class="sxs-lookup"><span data-stu-id="5550f-770">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="5550f-771">30 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-771">April 30, 2020</span></span>

<span data-ttu-id="5550f-772">Версия 2.5.1</span><span class="sxs-lookup"><span data-stu-id="5550f-772">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-773">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-773">ACR</span></span>

* <span data-ttu-id="5550f-774">`az acr check-health`: исправлена ошибка DOCKER_PULL_ERROR в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-774">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-775">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-775">Compute</span></span>

* <span data-ttu-id="5550f-776">`az vm list-ip-addresses`: Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="5550f-776">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="5550f-777">Исправлена ошибка создания виртуальной машины, которая возникает, если в профиле облака не задано значение endpoint_vm_image_alias_doc.</span><span class="sxs-lookup"><span data-stu-id="5550f-777">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="5550f-778">`az vmss create`: добавлен параметр --os-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="5550f-778">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-779">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-779">Cosmos DB</span></span>

* <span data-ttu-id="5550f-780">`az cosmosdb create/update`: добавлена поддержка --enable-public-network.</span><span class="sxs-lookup"><span data-stu-id="5550f-780">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-781">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-781">Extension</span></span>

* <span data-ttu-id="5550f-782">Исправлена загрузка неправильных метаданных для расширения типа колеса.</span><span class="sxs-lookup"><span data-stu-id="5550f-782">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-783">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-783">Packaging</span></span>

* <span data-ttu-id="5550f-784">Добавлен скрипт az для Git Bash/Cygwin в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-784">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-785">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-785">SQL</span></span>

* <span data-ttu-id="5550f-786">`az sql instance-pool`: добавлена группа команд для пулов экземпляров.</span><span class="sxs-lookup"><span data-stu-id="5550f-786">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-787">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-787">Storage</span></span>

* <span data-ttu-id="5550f-788">Пакет azure-multiapi-storage обновлен до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-788">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="5550f-789">Добавлена поддержка GZRS при создании и обновлении учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-789">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="5550f-790">`az storage account failover`: добавлена поддержка отработки отказа учетной записи хранения GRS или GZRS.</span><span class="sxs-lookup"><span data-stu-id="5550f-790">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="5550f-791">`az storage blob upload`: добавлен параметр --encryption-scope для указания сведений об области шифрования.</span><span class="sxs-lookup"><span data-stu-id="5550f-791">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="5550f-792">28 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-792">April 28, 2020</span></span>

<span data-ttu-id="5550f-793">Версия 2.5.0</span><span class="sxs-lookup"><span data-stu-id="5550f-793">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-794">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-794">ACS</span></span>

* <span data-ttu-id="5550f-795">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az openshift create: удален параметр --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="5550f-795">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="5550f-796">`az openshift create`: добавлены флаги для поддержки частного кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-796">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="5550f-797">`az openshift`: обновление до версии API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="5550f-797">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="5550f-798">`az openshift`: добавлена команда `update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-798">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-799">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-799">AKS</span></span>

* <span data-ttu-id="5550f-800">`az aks create`: включена поддержка Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-800">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-801">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-801">AppService</span></span>

* <span data-ttu-id="5550f-802">`az webapp deployment source config-zip`: удалена функция перевода в спящий режим после выполнения request.get().</span><span class="sxs-lookup"><span data-stu-id="5550f-802">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-803">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-803">ARM</span></span>

* <span data-ttu-id="5550f-804">Добавлены команды What-If развертывания шаблона.</span><span class="sxs-lookup"><span data-stu-id="5550f-804">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-805">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-805">ARO</span></span>

* <span data-ttu-id="5550f-806">`az aro`: исправлены выходные данные таблицы.</span><span class="sxs-lookup"><span data-stu-id="5550f-806">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="5550f-807">CI</span><span class="sxs-lookup"><span data-stu-id="5550f-807">CI</span></span>

* <span data-ttu-id="5550f-808">Включена поддержка PyTest и прекращена поддержка Nose для автотестов.</span><span class="sxs-lookup"><span data-stu-id="5550f-808">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-809">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-809">Compute</span></span>

* <span data-ttu-id="5550f-810">`az vmss disk detach`: устранена проблема с NoneType для диска данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-810">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="5550f-811">`az vm availability-set list`: включена поддержка отображения списка виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-811">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="5550f-812">`az vm list-skus`: исправлена проблема с отображением формата таблицы.</span><span class="sxs-lookup"><span data-stu-id="5550f-812">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-813">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-813">KeyVault</span></span>

* <span data-ttu-id="5550f-814">Добавлен новый параметр `--enable-rbac-authorization` для использования во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="5550f-814">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-815">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-815">Monitor</span></span>

* <span data-ttu-id="5550f-816">Включена поддержка компонентов CMK в кластере LA.</span><span class="sxs-lookup"><span data-stu-id="5550f-816">Support LA cluster CMK features</span></span>
* <span data-ttu-id="5550f-817">`az monitor log-analytics workspace linked-storage`: включена поддержка функций BYOS.</span><span class="sxs-lookup"><span data-stu-id="5550f-817">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="5550f-818">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-818">Network</span></span>

* <span data-ttu-id="5550f-819">`az network security-partner`: включена поддержка поставщика партнера по безопасности.</span><span class="sxs-lookup"><span data-stu-id="5550f-819">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="5550f-820">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="5550f-820">Privatedns</span></span>

* <span data-ttu-id="5550f-821">Добавлена функция в частной зоне DNS для импорта и экспорта файла зоны.</span><span class="sxs-lookup"><span data-stu-id="5550f-821">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="5550f-822">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-822">April 21, 2020</span></span>

<span data-ttu-id="5550f-823">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="5550f-823">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-824">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-824">ACR</span></span>

* <span data-ttu-id="5550f-825">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="5550f-825">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="5550f-826">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-826">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-827">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-827">AKS</span></span>

* <span data-ttu-id="5550f-828">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-828">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="5550f-829">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="5550f-829">Add --uptime-sla</span></span>
* <span data-ttu-id="5550f-830">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="5550f-830">Update containerservice package</span></span>
* <span data-ttu-id="5550f-831">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-831">Add node public IP support</span></span>
* <span data-ttu-id="5550f-832">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="5550f-832">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-833">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-833">AppConfig</span></span>

* <span data-ttu-id="5550f-834">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="5550f-834">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="5550f-835">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-835">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-836">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-836">AppService</span></span>

* <span data-ttu-id="5550f-837">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-837">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="5550f-838">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-838">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="5550f-839">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="5550f-839">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="5550f-840">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="5550f-840">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="5550f-841">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="5550f-841">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-842">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-842">ARM</span></span>

* <span data-ttu-id="5550f-843">`az deployment create/validate`: добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="5550f-843">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="5550f-844">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-844">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="5550f-845">`az deployment`: удалено значение `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="5550f-845">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="5550f-846">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="5550f-846">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="5550f-847">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-847">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="5550f-848">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="5550f-848">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="5550f-849">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5550f-849">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="5550f-850">ARO</span><span class="sxs-lookup"><span data-stu-id="5550f-850">ARO</span></span>

* <span data-ttu-id="5550f-851">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="5550f-851">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-852">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-852">Batch</span></span>

* <span data-ttu-id="5550f-853">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-853">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-854">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-854">Compute</span></span>

* <span data-ttu-id="5550f-855">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="5550f-855">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="5550f-856">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="5550f-856">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="5550f-857">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-857">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="5550f-858">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="5550f-858">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="5550f-859">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="5550f-859">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="5550f-860">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="5550f-860">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-861">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-861">CosmosDB</span></span>

* <span data-ttu-id="5550f-862">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="5550f-862">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-863">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-863">IoT Central</span></span>

* <span data-ttu-id="5550f-864">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="5550f-864">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="5550f-865">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="5550f-865">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-866">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-866">Monitor</span></span>

* <span data-ttu-id="5550f-867">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="5550f-867">Support private link scenario for monitor</span></span>
* <span data-ttu-id="5550f-868">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="5550f-868">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="5550f-869">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-869">Network</span></span>

* <span data-ttu-id="5550f-870">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="5550f-870">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="5550f-871">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5550f-871">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="5550f-872">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="5550f-872">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="5550f-873">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="5550f-873">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-874">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-874">Packaging</span></span>

* <span data-ttu-id="5550f-875">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="5550f-875">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-876">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-876">RBAC</span></span>

* <span data-ttu-id="5550f-877">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="5550f-877">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-878">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-878">RDBMS</span></span>

* <span data-ttu-id="5550f-879">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-879">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-880">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-880">Service Fabric</span></span>

* <span data-ttu-id="5550f-881">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="5550f-881">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="5550f-882">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки, связанные с устойчивостью и надежностью обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="5550f-882">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-883">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-883">SQL</span></span>

* <span data-ttu-id="5550f-884">Добавлены команды `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="5550f-884">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="5550f-885">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="5550f-885">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-886">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-886">Storage</span></span>

* <span data-ttu-id="5550f-887">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-887">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="5550f-888">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-888">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="5550f-889">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="5550f-889">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="5550f-890">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="5550f-890">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="5550f-891">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="5550f-891">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="5550f-892">Опрос</span><span class="sxs-lookup"><span data-stu-id="5550f-892">Survey</span></span>

* <span data-ttu-id="5550f-893">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="5550f-893">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="5550f-894">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-894">April 01, 2020</span></span>

<span data-ttu-id="5550f-895">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="5550f-895">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-896">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-896">ACR</span></span>

* <span data-ttu-id="5550f-897">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-897">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-898">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-898">Profile</span></span>

* <span data-ttu-id="5550f-899">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="5550f-899">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="5550f-900">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-900">March 31, 2020</span></span>

<span data-ttu-id="5550f-901">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="5550f-901">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-902">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-902">ACR</span></span>

* <span data-ttu-id="5550f-903">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="5550f-903">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="5550f-904">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="5550f-904">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="5550f-905">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="5550f-905">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="5550f-906">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="5550f-906">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="5550f-907">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="5550f-907">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="5550f-908">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="5550f-908">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="5550f-909">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="5550f-909">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-910">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-910">AKS</span></span>

* <span data-ttu-id="5550f-911">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="5550f-911">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="5550f-912">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="5550f-912">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="5550f-913">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="5550f-913">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-914">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-914">AMS</span></span>

* <span data-ttu-id="5550f-915">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="5550f-915">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-916">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-916">AppConfig</span></span>

* <span data-ttu-id="5550f-917">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="5550f-917">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-918">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-918">AppService</span></span>

* <span data-ttu-id="5550f-919">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="5550f-919">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="5550f-920">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="5550f-920">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="5550f-921">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-921">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-922">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-922">ARM</span></span>

* <span data-ttu-id="5550f-923">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="5550f-923">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="5550f-924">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-924">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="5550f-925">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="5550f-925">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="5550f-926">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="5550f-926">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-927">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-927">Backup</span></span>

* <span data-ttu-id="5550f-928">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-928">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="5550f-929">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="5550f-929">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="5550f-930">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="5550f-930">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-931">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-931">Compute</span></span>

* <span data-ttu-id="5550f-932">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="5550f-932">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="5550f-933">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-933">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="5550f-934">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="5550f-934">az vm update: Support --workspace</span></span>
* <span data-ttu-id="5550f-935">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="5550f-935">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="5550f-936">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="5550f-936">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="5550f-937">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-937">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="5550f-938">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-938">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="5550f-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="5550f-939">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-940">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-940">Cosmos DB</span></span>

* <span data-ttu-id="5550f-941">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="5550f-941">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="5550f-942">Docker</span><span class="sxs-lookup"><span data-stu-id="5550f-942">Docker</span></span>

* <span data-ttu-id="5550f-943">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="5550f-943">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-944">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-944">Extension</span></span>

* <span data-ttu-id="5550f-945">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="5550f-945">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-946">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-946">HDInsight</span></span>

* <span data-ttu-id="5550f-947">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-947">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="5550f-948">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="5550f-948">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-949">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-949">IoT</span></span>

* <span data-ttu-id="5550f-950">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="5550f-950">Add codeowner</span></span>
* <span data-ttu-id="5550f-951">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="5550f-951">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="5550f-952">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="5550f-952">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5550f-953">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-953">IoTCentral</span></span>

* <span data-ttu-id="5550f-954">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-954">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-955">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-955">KeyVault</span></span>

* <span data-ttu-id="5550f-956">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-956">Support certificate backup/restore</span></span>
* <span data-ttu-id="5550f-957">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="5550f-957">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="5550f-958">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="5550f-958">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="5550f-959">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-959">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="5550f-960">Блокировка</span><span class="sxs-lookup"><span data-stu-id="5550f-960">Lock</span></span>

* <span data-ttu-id="5550f-961">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-961">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-962">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-962">Monitor</span></span>

* <span data-ttu-id="5550f-963">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="5550f-963">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="5550f-964">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5550f-964">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-965">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-965">NetAppFiles</span></span>

* <span data-ttu-id="5550f-966">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="5550f-966">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="5550f-967">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-967">Network</span></span>

* <span data-ttu-id="5550f-968">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="5550f-968">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="5550f-969">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5550f-969">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="5550f-970">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-970">support host names in application gateway listener</span></span>
* <span data-ttu-id="5550f-971">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="5550f-971">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="5550f-972">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="5550f-972">Support vpn gateway generation</span></span>
* <span data-ttu-id="5550f-973">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="5550f-973">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-974">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-974">Packaging</span></span>

* <span data-ttu-id="5550f-975">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="5550f-975">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-976">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-976">Profile</span></span>

* <span data-ttu-id="5550f-977">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="5550f-977">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-978">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-978">RDBMS</span></span>

* <span data-ttu-id="5550f-979">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-979">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="5550f-980">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-980">March 10, 2020</span></span>

<span data-ttu-id="5550f-981">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="5550f-981">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-982">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-982">ACR</span></span>

* <span data-ttu-id="5550f-983">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="5550f-983">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="5550f-984">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="5550f-984">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="5550f-985">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="5550f-985">Add private link and CMK support</span></span>
* <span data-ttu-id="5550f-986">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="5550f-986">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-987">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-987">AKS</span></span>

* <span data-ttu-id="5550f-988">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5550f-988">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="5550f-989">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="5550f-989">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="5550f-990">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-990">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5550f-991">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="5550f-991">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="5550f-992">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="5550f-992">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="5550f-993">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-993">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="5550f-994">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-994">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="5550f-995">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="5550f-995">add missing / in the dashboard url</span></span>
* <span data-ttu-id="5550f-996">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="5550f-996">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="5550f-997">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="5550f-997">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="5550f-998">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="5550f-998">az aks: Add aad session key support</span></span>
* <span data-ttu-id="5550f-999">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="5550f-999">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="5550f-1000">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="5550f-1000">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1001">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1001">AppConfig</span></span>

* <span data-ttu-id="5550f-1002">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1002">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1003">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1003">AppService</span></span>

* <span data-ttu-id="5550f-1004">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="5550f-1004">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="5550f-1005">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-1005">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="5550f-1006">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1006">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="5550f-1007">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-1007">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="5550f-1008">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-1008">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="5550f-1009">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="5550f-1009">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1010">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1010">ARM</span></span>

* <span data-ttu-id="5550f-1011">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1011">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="5550f-1012">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1012">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="5550f-1013">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1013">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="5550f-1014">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1014">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="5550f-1015">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1015">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="5550f-1016">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1016">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="5550f-1017">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1017">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="5550f-1018">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="5550f-1018">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="5550f-1019">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1019">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="5550f-1020">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1020">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-1021">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-1021">CDN</span></span>

* <span data-ttu-id="5550f-1022">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="5550f-1022">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1023">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1023">Compute</span></span>

* <span data-ttu-id="5550f-1024">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="5550f-1024">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="5550f-1025">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="5550f-1025">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="5550f-1026">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1026">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="5550f-1027">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="5550f-1027">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="5550f-1028">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="5550f-1028">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-1029">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1029">Cosmos DB</span></span>

* <span data-ttu-id="5550f-1030">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-1030">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="5550f-1031">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1031">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-1032">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-1032">KeyVault</span></span>

* <span data-ttu-id="5550f-1033">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1033">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-1034">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-1034">Monitor</span></span>

* <span data-ttu-id="5550f-1035">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1035">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1036">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1036">Network</span></span>

* <span data-ttu-id="5550f-1037">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1037">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="5550f-1038">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-1038">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="5550f-1039">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-1039">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="5550f-1040">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="5550f-1040">az network bastion: support bastion</span></span>
* <span data-ttu-id="5550f-1041">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-1041">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="5550f-1042">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="5550f-1042">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="5550f-1043">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="5550f-1043">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="5550f-1044">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="5550f-1044">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="5550f-1045">Политика</span><span class="sxs-lookup"><span data-stu-id="5550f-1045">Policy</span></span>

* <span data-ttu-id="5550f-1046">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="5550f-1046">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1047">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1047">RBAC</span></span>

* <span data-ttu-id="5550f-1048">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="5550f-1048">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-1049">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-1049">RDBMS</span></span>

* <span data-ttu-id="5550f-1050">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1050">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="5550f-1051">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="5550f-1051">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="5550f-1052">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="5550f-1052">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="5550f-1053">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1053">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="5550f-1054">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1054">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="5550f-1055">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1055">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="5550f-1056">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1056">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="5550f-1057">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1057">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1058">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1058">SQL</span></span>

* <span data-ttu-id="5550f-1059">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="5550f-1059">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="5550f-1060">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="5550f-1060">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="5550f-1061">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1061">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="5550f-1062">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1062">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1063">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1063">Storage</span></span>

* <span data-ttu-id="5550f-1064">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1064">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="5550f-1065">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="5550f-1065">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="5550f-1066">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1066">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="5550f-1067">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1067">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="5550f-1068">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="5550f-1068">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="5550f-1069">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1069">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="5550f-1070">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="5550f-1070">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="5550f-1071">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="5550f-1071">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="5550f-1072">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1072">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="5550f-1073">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1073">February 18, 2020</span></span>

<span data-ttu-id="5550f-1074">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="5550f-1074">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1075">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1075">ACR</span></span>

* <span data-ttu-id="5550f-1076">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1076">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="5550f-1077">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1077">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="5550f-1078">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="5550f-1078">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1079">ACS</span></span>

* <span data-ttu-id="5550f-1080">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1080">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="5550f-1081">Aladdin</span><span class="sxs-lookup"><span data-stu-id="5550f-1081">Aladdin</span></span>

* <span data-ttu-id="5550f-1082">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-1082">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-1083">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1083">AMS</span></span>

* <span data-ttu-id="5550f-1084">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5550f-1084">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1085">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1085">AppConfig</span></span>

* <span data-ttu-id="5550f-1086">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="5550f-1086">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="5550f-1087">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-1087">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="5550f-1088">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1088">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1089">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1089">AppService</span></span>

* <span data-ttu-id="5550f-1090">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="5550f-1090">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="5550f-1091">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1091">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="5550f-1092">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="5550f-1092">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1093">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1093">ARM</span></span>

* <span data-ttu-id="5550f-1094">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="5550f-1094">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="5550f-1095">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="5550f-1095">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-1096">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1096">Backup</span></span>

* <span data-ttu-id="5550f-1097">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="5550f-1097">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="5550f-1098">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="5550f-1098">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1099">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1099">Compute</span></span>

* <span data-ttu-id="5550f-1100">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="5550f-1100">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="5550f-1101">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="5550f-1101">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="5550f-1102">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1102">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="5550f-1103">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-1103">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="5550f-1104">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-1104">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-1105">Eventhub</span><span class="sxs-lookup"><span data-stu-id="5550f-1105">Eventhub</span></span>

* <span data-ttu-id="5550f-1106">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="5550f-1106">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-1107">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-1107">KeyVault</span></span>

* <span data-ttu-id="5550f-1108">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1108">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="5550f-1109">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1109">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="5550f-1110">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="5550f-1110">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1111">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1111">Network</span></span>

* <span data-ttu-id="5550f-1112">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1112">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="5550f-1113">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="5550f-1113">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="5550f-1114">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-1114">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-1115">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-1115">Packaging</span></span>

* <span data-ttu-id="5550f-1116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="5550f-1116">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1117">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1117">Profile</span></span>

* <span data-ttu-id="5550f-1118">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1118">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="5550f-1119">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1119">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="5550f-1120">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="5550f-1120">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="5550f-1121">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="5550f-1121">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="5550f-1122">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-1122">Role</span></span>

* <span data-ttu-id="5550f-1123">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="5550f-1123">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1124">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1124">SQL</span></span>

* <span data-ttu-id="5550f-1125">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="5550f-1125">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1126">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1126">Storage</span></span>

* <span data-ttu-id="5550f-1127">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="5550f-1127">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="5550f-1128">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1128">February 04, 2020</span></span>

<span data-ttu-id="5550f-1129">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="5550f-1129">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1130">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1130">ACS</span></span>

* <span data-ttu-id="5550f-1131">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="5550f-1131">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="5550f-1132">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1132">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1133">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1133">ACR</span></span>

* <span data-ttu-id="5550f-1134">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="5550f-1134">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="5550f-1135">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="5550f-1135">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="5550f-1136">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="5550f-1136">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1137">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1137">AKS</span></span>

* <span data-ttu-id="5550f-1138">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="5550f-1138">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1139">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1139">AppConfig</span></span>

* <span data-ttu-id="5550f-1140">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="5550f-1140">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="5550f-1141">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="5550f-1141">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="5550f-1142">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="5550f-1142">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="5550f-1143">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="5550f-1143">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="5550f-1144">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1144">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1145">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1145">AppService</span></span>

* <span data-ttu-id="5550f-1146">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="5550f-1146">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="5550f-1147">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-1147">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1148">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1148">ARM</span></span>

* <span data-ttu-id="5550f-1149">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1149">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="5550f-1150">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1150">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="5550f-1151">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="5550f-1151">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="5550f-1152">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1152">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="5550f-1153">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1153">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5550f-1154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5550f-1154">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5550f-1155">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="5550f-1155">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1156">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1156">BotService</span></span>

* <span data-ttu-id="5550f-1157">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="5550f-1157">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="5550f-1158">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-1158">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-1159">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-1159">CDN</span></span>

* <span data-ttu-id="5550f-1160">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="5550f-1160">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="5550f-1161">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="5550f-1161">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="5550f-1162">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="5550f-1162">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5550f-1163">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="5550f-1163">Deployment Manager</span></span>

* <span data-ttu-id="5550f-1164">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1164">Add list operation for all resources.</span></span>
* <span data-ttu-id="5550f-1165">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="5550f-1165">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="5550f-1166">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1166">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1167">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1167">IoT</span></span>

* <span data-ttu-id="5550f-1168">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="5550f-1168">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-1169">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-1169">IoT Central</span></span>

* <span data-ttu-id="5550f-1170">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="5550f-1170">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1171">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1171">Key Vault</span></span>

* <span data-ttu-id="5550f-1172">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1172">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="5550f-1173">Разное</span><span class="sxs-lookup"><span data-stu-id="5550f-1173">Misc</span></span>

* <span data-ttu-id="5550f-1174">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="5550f-1174">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1175">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1175">Network</span></span>

* <span data-ttu-id="5550f-1176">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="5550f-1176">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="5550f-1177">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="5550f-1177">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="5550f-1178">Политика</span><span class="sxs-lookup"><span data-stu-id="5550f-1178">Policy</span></span>

* <span data-ttu-id="5550f-1179">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="5550f-1179">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="5550f-1180">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="5550f-1180">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1181">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1181">Profile</span></span>

* <span data-ttu-id="5550f-1182">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="5550f-1182">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1183">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1183">RBAC</span></span>

* <span data-ttu-id="5550f-1184">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-1184">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="5550f-1185">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5550f-1185">Security</span></span>

* <span data-ttu-id="5550f-1186">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1186">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1187">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1187">SQL</span></span>

* <span data-ttu-id="5550f-1188">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="5550f-1188">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="5550f-1189">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-1189">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="5550f-1190">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="5550f-1190">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="5550f-1191">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="5550f-1191">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="5550f-1192">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1192">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="5550f-1193">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1193">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1194">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1194">Storage</span></span>

* <span data-ttu-id="5550f-1195">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-1195">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="5550f-1196">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1196">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="5550f-1197">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="5550f-1197">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="5550f-1198">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1198">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5550f-1199">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1199">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="5550f-1200">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1200">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5550f-1201">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-1201">ServiceFabric</span></span>

* <span data-ttu-id="5550f-1202">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="5550f-1202">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="5550f-1203">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1203">January 13, 2020</span></span>

<span data-ttu-id="5550f-1204">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="5550f-1204">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1205">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1205">Compute</span></span>

* <span data-ttu-id="5550f-1206">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="5550f-1206">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="5550f-1207">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="5550f-1207">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1208">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1208">Storage</span></span>

* <span data-ttu-id="5550f-1209">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="5550f-1209">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="5550f-1210">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1210">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="5550f-1211">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1211">January 07, 2020</span></span>

<span data-ttu-id="5550f-1212">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="5550f-1212">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1213">ACR</span></span>

* <span data-ttu-id="5550f-1214">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="5550f-1214">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="5550f-1215">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="5550f-1215">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1216">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1216">AppConfig</span></span>

* <span data-ttu-id="5550f-1217">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-1217">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="5550f-1218">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1218">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="5550f-1219">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="5550f-1219">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1220">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1220">AppService</span></span>

* <span data-ttu-id="5550f-1221">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1221">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="5550f-1222">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1222">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="5550f-1223">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="5550f-1223">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1224">ARM</span></span>

* <span data-ttu-id="5550f-1225">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1225">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-1226">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1226">Backup</span></span>

* <span data-ttu-id="5550f-1227">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="5550f-1227">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="5550f-1228">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="5550f-1228">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="5550f-1229">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="5550f-1229">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1230">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1230">Compute</span></span>

* <span data-ttu-id="5550f-1231">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5550f-1231">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="5550f-1232">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="5550f-1232">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="5550f-1233">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="5550f-1233">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-1234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-1234">HDInsight</span></span>

* <span data-ttu-id="5550f-1235">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="5550f-1235">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="5550f-1236">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="5550f-1236">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="5550f-1237">Прочее</span><span class="sxs-lookup"><span data-stu-id="5550f-1237">Misc.</span></span>

* <span data-ttu-id="5550f-1238">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="5550f-1238">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="5550f-1239">Центры событий</span><span class="sxs-lookup"><span data-stu-id="5550f-1239">Event Hubs</span></span>

* <span data-ttu-id="5550f-1240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1240">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="5550f-1241">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-1241">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="5550f-1242">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-1242">Service Bus</span></span>

* <span data-ttu-id="5550f-1243">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="5550f-1243">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="5550f-1244">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="5550f-1244">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1245">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1245">RBAC</span></span>

* <span data-ttu-id="5550f-1246">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-1246">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1247">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1247">Storage</span></span>

* <span data-ttu-id="5550f-1248">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="5550f-1248">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="5550f-1249">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1249">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="5550f-1250">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1250">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="5550f-1251">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1251">December 17, 2019</span></span>

<span data-ttu-id="5550f-1252">2.0.78</span><span class="sxs-lookup"><span data-stu-id="5550f-1252">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1253">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1253">ACR</span></span>

* <span data-ttu-id="5550f-1254">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-1254">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1255">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1255">ACS</span></span>

* <span data-ttu-id="5550f-1256">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1256">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-1257">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1257">AMS</span></span>

* <span data-ttu-id="5550f-1258">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="5550f-1258">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1259">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1259">AppConfig</span></span>

* <span data-ttu-id="5550f-1260">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="5550f-1260">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="5550f-1261">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1261">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="5550f-1262">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1262">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1263">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1263">AppService</span></span>

* <span data-ttu-id="5550f-1264">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="5550f-1264">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="5550f-1265">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="5550f-1265">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="5550f-1266">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="5550f-1266">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="5550f-1267">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="5550f-1267">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1268">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1268">ARM</span></span>

* <span data-ttu-id="5550f-1269">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="5550f-1269">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="5550f-1270">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="5550f-1270">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="5550f-1271">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="5550f-1271">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-1272">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1272">Backup</span></span>

* <span data-ttu-id="5550f-1273">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="5550f-1273">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1274">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1274">BotService</span></span>

* <span data-ttu-id="5550f-1275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1275">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="5550f-1276">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="5550f-1276">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="5550f-1277">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1277">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="5550f-1278">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="5550f-1278">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="5550f-1279">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="5550f-1279">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="5550f-1280">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1280">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="5550f-1281">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="5550f-1281">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="5550f-1282">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="5550f-1282">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="5550f-1283">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="5550f-1283">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1284">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1284">Compute</span></span>

* <span data-ttu-id="5550f-1285">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1285">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="5550f-1286">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="5550f-1286">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="5550f-1287">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="5550f-1287">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="5550f-1288">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="5550f-1288">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="5550f-1289">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="5550f-1289">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="5550f-1290">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="5550f-1290">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1291">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1291">Core</span></span>

* <span data-ttu-id="5550f-1292">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="5550f-1292">Removed support for Python 3.4</span></span>
* <span data-ttu-id="5550f-1293">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1293">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="5550f-1294">DLS</span><span class="sxs-lookup"><span data-stu-id="5550f-1294">DLS</span></span>

* <span data-ttu-id="5550f-1295">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="5550f-1295">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="5550f-1296">Установка</span><span class="sxs-lookup"><span data-stu-id="5550f-1296">Install</span></span>

* <span data-ttu-id="5550f-1297">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="5550f-1297">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1298">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1298">IOT</span></span>

* <span data-ttu-id="5550f-1299">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="5550f-1299">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="5550f-1300">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="5550f-1300">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1301">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1301">Key Vault</span></span>

* <span data-ttu-id="5550f-1302">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="5550f-1302">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="5550f-1303">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1303">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="5550f-1304">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1304">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="5550f-1305">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="5550f-1305">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="5550f-1306">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1306">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1307">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1307">Network</span></span>

* <span data-ttu-id="5550f-1308">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="5550f-1308">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="5550f-1309">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1309">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="5550f-1310">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1310">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="5550f-1311">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1311">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="5550f-1312">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="5550f-1312">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-1313">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-1313">Packaging</span></span>

* <span data-ttu-id="5550f-1314">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="5550f-1314">Added back edge builds for pip install</span></span>
* <span data-ttu-id="5550f-1315">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="5550f-1315">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="5550f-1316">Политика</span><span class="sxs-lookup"><span data-stu-id="5550f-1316">Policy</span></span>

* <span data-ttu-id="5550f-1317">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1317">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="5550f-1318">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1318">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-1319">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-1319">Redis</span></span>

* <span data-ttu-id="5550f-1320">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1320">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="5550f-1321">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="5550f-1321">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5550f-1322">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-1322">ServiceFabric</span></span>

* <span data-ttu-id="5550f-1323">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-1323">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="5550f-1324">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="5550f-1324">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1325">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1325">SQL</span></span>

* <span data-ttu-id="5550f-1326">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1326">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1327">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1327">Storage</span></span>

* <span data-ttu-id="5550f-1328">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1328">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="5550f-1329">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="5550f-1329">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="5550f-1330">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1330">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="5550f-1331">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1331">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="5550f-1332">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1332">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="5550f-1333">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1333">November 26, 2019</span></span>

<span data-ttu-id="5550f-1334">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="5550f-1334">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1335">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1335">ACR</span></span>

* <span data-ttu-id="5550f-1336">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5550f-1336">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="5550f-1337">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5550f-1337">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="5550f-1338">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="5550f-1338">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="5550f-1339">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="5550f-1339">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1340">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1340">AKS</span></span>

* <span data-ttu-id="5550f-1341">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="5550f-1341">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1342">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1342">AppConfig</span></span>

* <span data-ttu-id="5550f-1343">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1343">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="5550f-1344">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1344">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="5550f-1345">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1345">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="5550f-1346">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1346">AppService</span></span>

* <span data-ttu-id="5550f-1347">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1347">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="5550f-1348">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="5550f-1348">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="5550f-1349">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="5550f-1349">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-1350">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1350">Backup</span></span>

* <span data-ttu-id="5550f-1351">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="5550f-1351">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="5550f-1352">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="5550f-1352">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1353">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1353">Compute</span></span>

* <span data-ttu-id="5550f-1354">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1354">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="5550f-1355">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="5550f-1355">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="5550f-1356">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="5550f-1356">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="5550f-1357">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="5550f-1357">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="5550f-1358">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="5550f-1358">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="5550f-1359">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-1359">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="5550f-1360">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1360">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="5550f-1361">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="5550f-1361">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="5550f-1362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5550f-1362">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="5550f-1363">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-1363">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1364">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1364">IOT</span></span>

* <span data-ttu-id="5550f-1365">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="5550f-1365">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="5550f-1366">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-1366">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="5550f-1367">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1367">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1368">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1368">Key Vault</span></span>

* <span data-ttu-id="5550f-1369">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1369">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-1370">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-1370">NetAppFiles</span></span>

* <span data-ttu-id="5550f-1371">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1371">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1372">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1372">Network</span></span>

* <span data-ttu-id="5550f-1373">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="5550f-1373">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="5550f-1374">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1374">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="5550f-1375">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="5550f-1375">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="5550f-1376">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="5550f-1376">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="5550f-1377">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1377">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="5550f-1378">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1378">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="5550f-1379">Упаковка</span><span class="sxs-lookup"><span data-stu-id="5550f-1379">Packaging</span></span>

* <span data-ttu-id="5550f-1380">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="5550f-1380">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="5550f-1381">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="5550f-1381">Added support for Python 3.8</span></span>
* <span data-ttu-id="5550f-1382">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="5550f-1382">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1383">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1383">Profile</span></span>

* <span data-ttu-id="5550f-1384">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5550f-1384">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="5550f-1385">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="5550f-1385">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="5550f-1386">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1386">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="5550f-1387">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1387">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="5550f-1388">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="5550f-1388">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1389">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1389">RBAC</span></span>

* <span data-ttu-id="5550f-1390">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="5550f-1390">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-1391">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-1391">Redis</span></span>

* <span data-ttu-id="5550f-1392">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="5550f-1392">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="5550f-1393">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1393">Reservations</span></span>

* <span data-ttu-id="5550f-1394">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="5550f-1394">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="5550f-1395">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="5550f-1395">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="5550f-1396">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="5550f-1396">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="5550f-1397">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="5550f-1397">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="5550f-1398">Rest</span><span class="sxs-lookup"><span data-stu-id="5550f-1398">Rest</span></span>
* <span data-ttu-id="5550f-1399">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="5550f-1399">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1400">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1400">SQL</span></span>

* <span data-ttu-id="5550f-1401">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-1401">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1402">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1402">Storage</span></span>

* <span data-ttu-id="5550f-1403">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1403">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="5550f-1404">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-1404">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="5550f-1405">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="5550f-1405">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="5550f-1406">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="5550f-1406">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="5550f-1407">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1407">November 4, 2019</span></span>

<span data-ttu-id="5550f-1408">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="5550f-1408">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1409">ACR</span></span>

* <span data-ttu-id="5550f-1410">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1410">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="5550f-1411">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="5550f-1411">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="5550f-1412">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="5550f-1412">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1413">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1413">AKS</span></span>

* <span data-ttu-id="5550f-1414">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1414">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="5550f-1415">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-1415">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="5550f-1416">AppConfig</span><span class="sxs-lookup"><span data-stu-id="5550f-1416">AppConfig</span></span>

* <span data-ttu-id="5550f-1417">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1417">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="5550f-1418">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="5550f-1418">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="5550f-1419">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="5550f-1419">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1420">AppService</span></span>

* <span data-ttu-id="5550f-1421">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="5550f-1421">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="5550f-1422">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-1422">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="5550f-1423">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5550f-1423">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="5550f-1424">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="5550f-1424">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="5550f-1425">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1425">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1426">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1426">ARM</span></span>

* <span data-ttu-id="5550f-1427">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1427">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="5550f-1428">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1428">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-1429">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-1429">Backup</span></span>

* <span data-ttu-id="5550f-1430">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="5550f-1430">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1431">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1431">Compute</span></span>

* <span data-ttu-id="5550f-1432">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="5550f-1432">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="5550f-1433">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="5550f-1433">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="5550f-1434">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="5550f-1434">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="5550f-1435">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="5550f-1435">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="5550f-1436">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="5550f-1436">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="5550f-1437">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1437">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="5550f-1438">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5550f-1438">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="5550f-1439">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="5550f-1439">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-1440">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1440">CosmosDB</span></span>

* <span data-ttu-id="5550f-1441">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5550f-1441">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5550f-1442">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5550f-1442">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="5550f-1443">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1443">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5550f-1444">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1444">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5550f-1445">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1445">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="5550f-1446">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1446">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="5550f-1447">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5550f-1447">Fixed typo in help message</span></span>
* <span data-ttu-id="5550f-1448">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1448">database: Added deprecation information</span></span>
* <span data-ttu-id="5550f-1449">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1449">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1450">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1450">IoT</span></span>

* <span data-ttu-id="5550f-1451">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="5550f-1451">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="5550f-1452">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1452">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1453">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1453">Key Vault</span></span>

* <span data-ttu-id="5550f-1454">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="5550f-1454">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="5550f-1455">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1455">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="5550f-1456">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="5550f-1456">NetAppFiles</span></span>

* <span data-ttu-id="5550f-1457">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1457">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="5550f-1458">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="5550f-1458">This new API version includes:</span></span>

    - <span data-ttu-id="5550f-1459">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="5550f-1459">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="5550f-1460">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="5550f-1460">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="5550f-1461">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1461">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="5550f-1462">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="5550f-1462">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1463">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1463">Network</span></span>

* <span data-ttu-id="5550f-1464">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="5550f-1464">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="5550f-1465">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="5550f-1465">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="5550f-1466">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="5550f-1466">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="5550f-1467">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1467">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="5550f-1468">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1468">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="5550f-1469">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1469">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1470">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1470">Profile</span></span>

* <span data-ttu-id="5550f-1471">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1471">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="5550f-1472">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1472">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1473">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1473">RBAC</span></span>

* <span data-ttu-id="5550f-1474">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="5550f-1474">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5550f-1475">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-1475">ServiceFabric</span></span>

* <span data-ttu-id="5550f-1476">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-1476">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1477">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1477">SQL</span></span>

* <span data-ttu-id="5550f-1478">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1478">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1479">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1479">Storage</span></span>

* <span data-ttu-id="5550f-1480">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-1480">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="5550f-1481">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1481">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="5550f-1482">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1482">October 15, 2019</span></span>

<span data-ttu-id="5550f-1483">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="5550f-1483">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1484">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1484">AKS</span></span>

* <span data-ttu-id="5550f-1485">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1485">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="5550f-1486">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1486">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-1487">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1487">AMS</span></span>

* <span data-ttu-id="5550f-1488">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1488">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="5550f-1489">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1489">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1490">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1490">AppService</span></span>

* <span data-ttu-id="5550f-1491">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1491">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="5550f-1492">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1492">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="5550f-1493">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1493">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1494">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1494">ARM</span></span>

* <span data-ttu-id="5550f-1495">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-1495">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1496">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1496">Compute</span></span>

* <span data-ttu-id="5550f-1497">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1497">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="5550f-1498">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="5550f-1498">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="5550f-1499">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="5550f-1499">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="5550f-1500">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1500">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="5550f-1501">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-1501">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="5550f-1502">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1502">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1503">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1503">Core</span></span>

* <span data-ttu-id="5550f-1504">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1504">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1505">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1505">IoT</span></span>

* <span data-ttu-id="5550f-1506">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="5550f-1506">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-1507">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-1507">Monitor</span></span>

* <span data-ttu-id="5550f-1508">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="5550f-1508">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1509">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1509">Network</span></span>

* <span data-ttu-id="5550f-1510">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1510">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="5550f-1511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1511">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1512">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1512">SQL</span></span>

* <span data-ttu-id="5550f-1513">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1513">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1514">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1514">Storage</span></span>

* <span data-ttu-id="5550f-1515">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="5550f-1515">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="5550f-1516">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1516">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="5550f-1517">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1517">September 24, 2019</span></span>

<span data-ttu-id="5550f-1518">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="5550f-1518">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1519">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1519">ACR</span></span>

* <span data-ttu-id="5550f-1520">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1520">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="5550f-1521">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1521">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1522">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1522">AKS</span></span>

* <span data-ttu-id="5550f-1523">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1523">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="5550f-1524">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1524">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="5550f-1525">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1525">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1526">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1526">ARM</span></span>

* <span data-ttu-id="5550f-1527">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-1527">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1528">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1528">Compute</span></span>

* <span data-ttu-id="5550f-1529">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-1529">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5550f-1530">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-1530">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="5550f-1531">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1531">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="5550f-1532">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="5550f-1532">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="5550f-1533">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5550f-1533">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-1534">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1534">Cosmos DB</span></span>

* <span data-ttu-id="5550f-1535">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1535">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="5550f-1536">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1536">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="5550f-1537">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5550f-1537">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5550f-1538">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5550f-1538">EventGrid</span></span>

* <span data-ttu-id="5550f-1539">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="5550f-1539">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1540">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1540">Key Vault</span></span>

* <span data-ttu-id="5550f-1541">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1541">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-1542">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-1542">Monitor</span></span>

* <span data-ttu-id="5550f-1543">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1543">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="5550f-1544">Политика</span><span class="sxs-lookup"><span data-stu-id="5550f-1544">Policy</span></span>

* <span data-ttu-id="5550f-1545">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1545">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="5550f-1546">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1546">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1547">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1547">Storage</span></span>

* <span data-ttu-id="5550f-1548">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1548">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="5550f-1549">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1549">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1550">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1550">ACR</span></span>

* <span data-ttu-id="5550f-1551">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-1551">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-1552">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-1552">AKS</span></span>

* <span data-ttu-id="5550f-1553">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5550f-1553">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="5550f-1554">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1554">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="5550f-1555">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1555">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-1556">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-1556">ARM</span></span>

* <span data-ttu-id="5550f-1557">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="5550f-1557">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-1558">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-1558">Batch</span></span>

* <span data-ttu-id="5550f-1559">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="5550f-1559">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="5550f-1560">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="5550f-1560">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="5550f-1561">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="5550f-1561">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="5550f-1562">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1562">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="5550f-1563">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1563">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="5550f-1564">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="5550f-1564">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="5550f-1565">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1565">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-1566">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-1566">HDInsight</span></span>

* <span data-ttu-id="5550f-1567">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5550f-1567">GA release</span></span>
* <span data-ttu-id="5550f-1568">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-1568">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-1569">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-1569">Key Vault</span></span>

* <span data-ttu-id="5550f-1570">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="5550f-1570">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="5550f-1571">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="5550f-1571">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1572">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1572">Network</span></span>

* <span data-ttu-id="5550f-1573">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="5550f-1573">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="5550f-1574">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="5550f-1574">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="5550f-1575">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1575">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="5550f-1576">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1576">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="5550f-1577">Политика</span><span class="sxs-lookup"><span data-stu-id="5550f-1577">Policy</span></span>

* <span data-ttu-id="5550f-1578">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-1578">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="5550f-1579">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1579">August 27, 2019</span></span>

<span data-ttu-id="5550f-1580">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="5550f-1580">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1581">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1581">ACR</span></span>

* <span data-ttu-id="5550f-1582">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1582">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="5550f-1583">Управление API</span><span class="sxs-lookup"><span data-stu-id="5550f-1583">API Management</span></span>

* <span data-ttu-id="5550f-1584">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1584">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1585">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1585">AppService</span></span>

* <span data-ttu-id="5550f-1586">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="5550f-1586">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="5550f-1587">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-1587">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-1588">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-1588">Keyvault</span></span>

* <span data-ttu-id="5550f-1589">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1589">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1590">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1590">Network</span></span>

* <span data-ttu-id="5550f-1591">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1591">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="5550f-1592">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="5550f-1592">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="5550f-1593">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1593">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="5550f-1594">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="5550f-1594">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1595">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1595">RBAC</span></span>

* <span data-ttu-id="5550f-1596">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="5550f-1596">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5550f-1597">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-1597">ServiceFabric</span></span>

* <span data-ttu-id="5550f-1598">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="5550f-1598">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="5550f-1599">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="5550f-1599">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="5550f-1600">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="5550f-1600">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="5550f-1601">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="5550f-1601">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="5550f-1602">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1602">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="5550f-1603">SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-1603">SignalR</span></span>

* <span data-ttu-id="5550f-1604">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="5550f-1604">Added new commands:</span></span>
  * <span data-ttu-id="5550f-1605">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-1605">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="5550f-1606">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-1606">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="5550f-1607">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-1607">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="5550f-1608">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="5550f-1608">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1609">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1609">Storage</span></span>

* <span data-ttu-id="5550f-1610">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1610">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="5550f-1611">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1611">August 13, 2019</span></span>

<span data-ttu-id="5550f-1612">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="5550f-1612">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1613">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1613">AppService</span></span>

* <span data-ttu-id="5550f-1614">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="5550f-1614">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1615">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1615">BotService</span></span>

* <span data-ttu-id="5550f-1616">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="5550f-1616">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="5550f-1617">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="5550f-1617">CognitiveServices</span></span>

* <span data-ttu-id="5550f-1618">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1618">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-1619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1619">Cosmos DB</span></span>

* <span data-ttu-id="5550f-1620">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="5550f-1620">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="5550f-1621">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1621">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-1622">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-1622">HDInsight</span></span>

<span data-ttu-id="5550f-1623">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1623">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="5550f-1624">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="5550f-1624">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="5550f-1625">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="5550f-1625">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="5550f-1626">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="5550f-1626">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="5550f-1627">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-1627">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="5550f-1628">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1628">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="5550f-1629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="5550f-1629">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="5550f-1630">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="5550f-1630">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="5550f-1631">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="5550f-1631">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="5550f-1632">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="5550f-1632">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="5550f-1633">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1633">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="5550f-1634">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="5550f-1634">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="5550f-1635">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1635">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="5550f-1636">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="5550f-1636">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="5550f-1637">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1637">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="5550f-1638">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1638">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="5550f-1639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1639">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="5550f-1640">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="5550f-1640">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="5550f-1641">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1641">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="5550f-1642">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-1642">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="5550f-1643">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1643">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="5550f-1644">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-1644">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="5550f-1645">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="5550f-1645">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="5550f-1646">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1646">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-1647">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-1647">Interactive</span></span>

* <span data-ttu-id="5550f-1648">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1648">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="5550f-1649">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5550f-1649">Kubernetes</span></span>

* <span data-ttu-id="5550f-1650">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1650">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1651">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1651">Network</span></span>

* <span data-ttu-id="5550f-1652">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1652">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1653">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1653">Profile</span></span>

* <span data-ttu-id="5550f-1654">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="5550f-1654">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="5550f-1655">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-1655">ServiceFabric</span></span>

* <span data-ttu-id="5550f-1656">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="5550f-1656">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="5550f-1657">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="5550f-1657">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1658">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1658">Storage</span></span>

* <span data-ttu-id="5550f-1659">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1659">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="5550f-1660">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1660">July 30, 2019</span></span>

<span data-ttu-id="5550f-1661">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="5550f-1661">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1662">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1662">ACR</span></span>

* <span data-ttu-id="5550f-1663">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="5550f-1663">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="5550f-1664">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1664">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1665">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-1665">Appservice</span></span>

* <span data-ttu-id="5550f-1666">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="5550f-1666">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="5550f-1667">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1667">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="5550f-1668">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="5550f-1668">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1669">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1669">Network</span></span>

* <span data-ttu-id="5550f-1670">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="5550f-1670">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="5550f-1671">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="5550f-1671">Fixes #9604.</span></span> <span data-ttu-id="5550f-1672">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1672">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="5550f-1673">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="5550f-1673">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1674">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1674">RBAC</span></span>

* <span data-ttu-id="5550f-1675">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1675">Added `user update` command</span></span>
* <span data-ttu-id="5550f-1676">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1676">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="5550f-1677">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1677">Use replacement argument `--id`</span></span>
* <span data-ttu-id="5550f-1678">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-1678">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1679">SQL</span></span>

* <span data-ttu-id="5550f-1680">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="5550f-1680">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1681">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1681">Storage</span></span>

* <span data-ttu-id="5550f-1682">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1682">Added `storage remove` command</span></span>
* <span data-ttu-id="5550f-1683">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1683">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-1684">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-1684">VM</span></span>

* <span data-ttu-id="5550f-1685">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1685">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="5550f-1686">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1686">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="5550f-1687">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1687">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="5550f-1688">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1688">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="5550f-1689">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5550f-1689">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="5550f-1690">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1690">July 16, 2019</span></span>

<span data-ttu-id="5550f-1691">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="5550f-1691">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1692">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-1692">Appservice</span></span>

* <span data-ttu-id="5550f-1693">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1693">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="5550f-1694">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="5550f-1694">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="5550f-1695">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1695">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1696">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1696">Core</span></span>

* <span data-ttu-id="5550f-1697">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="5550f-1697">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-1698">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-1698">Batch</span></span>

* <span data-ttu-id="5550f-1699">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1699">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="5550f-1700">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1700">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="5550f-1701">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1701">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="5550f-1702">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1702">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5550f-1703">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5550f-1703">Eventhubs</span></span>

* <span data-ttu-id="5550f-1704">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1704">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-1705">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-1705">RDBMS</span></span>

* <span data-ttu-id="5550f-1706">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="5550f-1706">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="5550f-1707">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1707">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="5550f-1708">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="5550f-1708">Relay</span></span>

* <span data-ttu-id="5550f-1709">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="5550f-1709">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="5550f-1710">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1710">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5550f-1711">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-1711">Servicebus</span></span>

* <span data-ttu-id="5550f-1712">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1712">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1713">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1713">Storage</span></span>

* <span data-ttu-id="5550f-1714">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="5550f-1714">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="5550f-1715">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1715">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="5550f-1716">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1716">July 2, 2019</span></span>

<span data-ttu-id="5550f-1717">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="5550f-1717">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1718">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1718">Core</span></span>

* <span data-ttu-id="5550f-1719">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="5550f-1719">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="5550f-1720">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="5550f-1720">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="5550f-1721">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1721">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1722">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1722">ACR</span></span>

* <span data-ttu-id="5550f-1723">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="5550f-1723">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1724">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-1724">Appservice</span></span>

* <span data-ttu-id="5550f-1725">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1725">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="5550f-1726">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1726">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="5550f-1727">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1727">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="5550f-1728">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-1728">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-1729">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1729">Cosmos DB</span></span>

* <span data-ttu-id="5550f-1730">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1730">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="5550f-1731">DLS</span><span class="sxs-lookup"><span data-stu-id="5550f-1731">DLS</span></span>

* <span data-ttu-id="5550f-1732">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="5550f-1732">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="5550f-1733">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5550f-1733">Feedback</span></span>

* <span data-ttu-id="5550f-1734">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="5550f-1734">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-1735">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-1735">HDInsight</span></span>

* <span data-ttu-id="5550f-1736">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1736">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="5550f-1737">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-1737">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="5550f-1738">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1738">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="5550f-1739">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1739">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="5550f-1740">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1740">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="5550f-1741">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-1741">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="5550f-1742">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1742">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="5550f-1743">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1743">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="5550f-1744">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1744">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="5550f-1745">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="5550f-1745">Managed Services</span></span>

* <span data-ttu-id="5550f-1746">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-1746">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-1747">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-1747">Profile</span></span>
* <span data-ttu-id="5550f-1748">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="5550f-1748">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1749">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1749">RBAC</span></span>

* <span data-ttu-id="5550f-1750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1750">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="5550f-1751">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="5550f-1751">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="5550f-1752">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1752">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="5550f-1753">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="5550f-1753">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-1754">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-1754">RDBMS</span></span>

* <span data-ttu-id="5550f-1755">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-1755">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1756">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1756">SQL</span></span>

* <span data-ttu-id="5550f-1757">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1757">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1758">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1758">Storage</span></span>

* <span data-ttu-id="5550f-1759">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1759">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="5550f-1760">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1760">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="5550f-1761">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-1761">VM</span></span>

* <span data-ttu-id="5550f-1762">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1762">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="5550f-1763">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="5550f-1763">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="5550f-1764">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1764">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="5550f-1765">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1765">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="5550f-1766">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1766">June 18, 2019</span></span>

<span data-ttu-id="5550f-1767">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="5550f-1767">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1768">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1768">Core</span></span>

<span data-ttu-id="5550f-1769">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-1769">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="5550f-1770">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="5550f-1770">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="5550f-1771">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="5550f-1771">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="5550f-1772">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1772">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="5550f-1773">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-1773">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="5550f-1774">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="5550f-1774">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="5550f-1775">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="5550f-1775">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1776">ACR</span></span>
* <span data-ttu-id="5550f-1777">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="5550f-1777">Added 'acr check-health' command</span></span>
* <span data-ttu-id="5550f-1778">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-1778">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1779">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1779">ACS</span></span>
* <span data-ttu-id="5550f-1780">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1780">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-1781">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1781">AMS</span></span>
* <span data-ttu-id="5550f-1782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="5550f-1782">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1783">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1783">AppService</span></span>
* <span data-ttu-id="5550f-1784">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1784">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="5550f-1785">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5550f-1785">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="5550f-1786">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="5550f-1786">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="5550f-1787">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1787">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="5550f-1788">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="5550f-1788">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="5550f-1789">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1789">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-1790">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-1790">Batch</span></span>
* <span data-ttu-id="5550f-1791">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="5550f-1791">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-1792">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-1792">BatchAI</span></span>
* <span data-ttu-id="5550f-1793">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="5550f-1793">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1794">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1794">BotService</span></span>
* <span data-ttu-id="5550f-1795">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="5550f-1795">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-1796">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-1796">CosmosDB</span></span>
* <span data-ttu-id="5550f-1797">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1797">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="5550f-1798">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1798">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="5550f-1799">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="5550f-1799">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="5550f-1800">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="5550f-1800">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5550f-1801">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5550f-1801">EventGrid</span></span>
* <span data-ttu-id="5550f-1802">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="5550f-1802">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="5550f-1803">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="5550f-1803">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="5550f-1804">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="5550f-1804">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="5550f-1805">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1805">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="5550f-1806">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1806">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-1807">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-1807">HDInsight</span></span>
* <span data-ttu-id="5550f-1808">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1808">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1809">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1809">IoT</span></span>
* <span data-ttu-id="5550f-1810">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1810">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="5550f-1811">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="5550f-1811">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1812">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1812">Network</span></span>
* <span data-ttu-id="5550f-1813">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="5550f-1813">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="5550f-1814">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1814">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="5550f-1815">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="5550f-1815">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="5550f-1816">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1816">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-1817">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-1817">Resource</span></span>
* <span data-ttu-id="5550f-1818">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="5550f-1818">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="5550f-1819">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1819">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="5550f-1820">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-1820">ServiceBus</span></span>
* <span data-ttu-id="5550f-1821">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1821">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1822">SQL</span></span>
* <span data-ttu-id="5550f-1823">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1823">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="5550f-1824">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1824">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="5550f-1825">SQLVm</span><span class="sxs-lookup"><span data-stu-id="5550f-1825">SQLVm</span></span>
* <span data-ttu-id="5550f-1826">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1826">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="5550f-1827">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-1827">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1828">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1828">Storage</span></span>
* <span data-ttu-id="5550f-1829">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1829">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="5550f-1830">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-1830">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-1831">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-1831">VM</span></span>
* <span data-ttu-id="5550f-1832">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-1832">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="5550f-1833">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1833">June 4, 2019</span></span>

<span data-ttu-id="5550f-1834">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="5550f-1834">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1835">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1835">Core</span></span>
* <span data-ttu-id="5550f-1836">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="5550f-1836">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1837">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1837">ACR</span></span>
* <span data-ttu-id="5550f-1838">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="5550f-1838">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1839">ACS</span></span>
* <span data-ttu-id="5550f-1840">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-1840">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="5550f-1841">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="5550f-1841">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-1842">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-1842">Batch</span></span>
* <span data-ttu-id="5550f-1843">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="5550f-1843">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1844">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1844">IoT</span></span>
* <span data-ttu-id="5550f-1845">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5550f-1845">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1846">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1846">Network</span></span>
* <span data-ttu-id="5550f-1847">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="5550f-1847">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="5550f-1848">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-1848">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="5550f-1849">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-1849">Resource</span></span>
* <span data-ttu-id="5550f-1850">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="5550f-1850">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="5550f-1851">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-1851">Role</span></span>
* <span data-ttu-id="5550f-1852">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1852">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1853">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1853">Compute</span></span>
* <span data-ttu-id="5550f-1854">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="5550f-1854">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="5550f-1855">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1855">May 21, 2019</span></span>

<span data-ttu-id="5550f-1856">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="5550f-1856">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="5550f-1857">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-1857">Core</span></span>
* <span data-ttu-id="5550f-1858">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1858">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="5550f-1859">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="5550f-1859">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="5550f-1860">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1860">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-1861">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-1861">ACR</span></span>
* <span data-ttu-id="5550f-1862">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="5550f-1862">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1863">ACS</span></span>
* <span data-ttu-id="5550f-1864">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="5550f-1864">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1865">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1865">AppService</span></span>
* <span data-ttu-id="5550f-1866">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="5550f-1866">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="5550f-1867">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="5550f-1867">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="5550f-1868">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1868">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="5550f-1869">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="5550f-1869">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="5550f-1870">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1870">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="5550f-1871">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1871">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="5550f-1872">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="5550f-1872">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1873">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1873">BotService</span></span>
* <span data-ttu-id="5550f-1874">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-1874">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="5550f-1875">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-1875">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-1876">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-1876">Consumption</span></span>
* <span data-ttu-id="5550f-1877">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1877">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-1878">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-1878">IoT</span></span>
* <span data-ttu-id="5550f-1879">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1879">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1880">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1880">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="5550f-1882">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="5550f-1882">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="5550f-1883">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1883">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-1884">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-1884">RDBMS</span></span>
* <span data-ttu-id="5550f-1885">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1885">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-1886">RBAC</span><span class="sxs-lookup"><span data-stu-id="5550f-1886">RBAC</span></span>
* <span data-ttu-id="5550f-1887">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1887">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1888">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1888">Storage</span></span>
* <span data-ttu-id="5550f-1889">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-1889">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="5550f-1890">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5550f-1890">Compute</span></span>
* <span data-ttu-id="5550f-1891">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5550f-1891">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="5550f-1892">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="5550f-1892">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="5550f-1893">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1893">__Note__ : This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="5550f-1894">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="5550f-1894">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="5550f-1895">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1895">May 6, 2019</span></span>

<span data-ttu-id="5550f-1896">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="5550f-1896">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1897">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1897">ACS</span></span>
* <span data-ttu-id="5550f-1898">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1898">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="5550f-1899">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="5550f-1899">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="5550f-1900">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1900">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="5550f-1901">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1901">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1902">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-1902">Appservice</span></span>
* <span data-ttu-id="5550f-1903">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5550f-1903">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="5550f-1904">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1904">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="5550f-1905">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1905">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="5550f-1906">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1906">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="5550f-1907">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1907">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="5550f-1908">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1908">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="5550f-1909">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-1909">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="5550f-1910">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="5550f-1910">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="5550f-1911">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-1911">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="5550f-1912">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1912">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-1913">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-1913">Batch</span></span>
* <span data-ttu-id="5550f-1914">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1914">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-1915">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-1915">Botservice</span></span>
* <span data-ttu-id="5550f-1916">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="5550f-1916">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="5550f-1917">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1917">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="5550f-1918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1918">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="5550f-1919">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1919">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="5550f-1920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1920">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="5550f-1921">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-1921">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="5550f-1922">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1922">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="5550f-1923">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1923">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="5550f-1924">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5550f-1924">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="5550f-1925">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5550f-1925">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="5550f-1926">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="5550f-1926">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="5550f-1927">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1927">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="5550f-1928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1928">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="5550f-1929">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="5550f-1929">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="5550f-1930">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1930">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="5550f-1931">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="5550f-1931">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="5550f-1932">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1932">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5550f-1933">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1933">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="5550f-1934">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="5550f-1934">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="5550f-1935">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1935">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5550f-1936">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1936">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="5550f-1937">Configure</span><span class="sxs-lookup"><span data-stu-id="5550f-1937">Configure</span></span>
* <span data-ttu-id="5550f-1938">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="5550f-1938">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5550f-1939">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5550f-1939">Eventhubs</span></span>
* <span data-ttu-id="5550f-1940">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1940">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5550f-1941">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1941">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1942">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1942">Network</span></span>
* <span data-ttu-id="5550f-1943">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1943">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="5550f-1944">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5550f-1944">Policy Insights</span></span>
* <span data-ttu-id="5550f-1945">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-1945">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="5550f-1946">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-1946">Role</span></span>
* <span data-ttu-id="5550f-1947">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="5550f-1947">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="5550f-1948">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-1948">Service Bus</span></span>
* <span data-ttu-id="5550f-1949">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1949">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5550f-1950">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1950">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="5550f-1951">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5550f-1951">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1952">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1952">SQL</span></span>
* <span data-ttu-id="5550f-1953">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1953">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-1954">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-1954">VM</span></span>
* <span data-ttu-id="5550f-1955">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-1955">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="5550f-1956">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-1956">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="5550f-1957">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1957">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="5550f-1958">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="5550f-1958">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="5550f-1959">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="5550f-1959">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="5550f-1960">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1960">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="5550f-1961">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-1961">April 23, 2019</span></span>

<span data-ttu-id="5550f-1962">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="5550f-1962">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-1963">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-1963">ACS</span></span>
* <span data-ttu-id="5550f-1964">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="5550f-1964">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="5550f-1965">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="5550f-1965">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-1966">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-1966">AMS</span></span>
* <span data-ttu-id="5550f-1967">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="5550f-1967">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-1968">AppService</span></span>
* <span data-ttu-id="5550f-1969">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1969">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="5550f-1970">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-1970">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="5550f-1971">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="5550f-1971">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="5550f-1972">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5550f-1972">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="5550f-1973">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-1973">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="5550f-1974">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="5550f-1974">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="5550f-1975">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="5550f-1975">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="5550f-1976">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="5550f-1976">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="5550f-1977">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1977">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5550f-1978">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="5550f-1978">Deployment Manager</span></span>
* <span data-ttu-id="5550f-1979">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="5550f-1979">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-1980">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-1980">Lab</span></span>
* <span data-ttu-id="5550f-1981">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1981">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="5550f-1982">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-1982">Network</span></span>
* <span data-ttu-id="5550f-1983">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="5550f-1983">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-1984">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-1984">Resource</span></span>
* <span data-ttu-id="5550f-1985">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1985">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="5550f-1986">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1986">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="5550f-1987">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="5550f-1987">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="5550f-1988">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-1988">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-1989">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-1989">SQL</span></span>
* <span data-ttu-id="5550f-1990">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5550f-1990">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="5550f-1991">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1991">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="5550f-1992">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1992">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="5550f-1993">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1993">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-1994">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-1994">Storage</span></span>
* <span data-ttu-id="5550f-1995">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="5550f-1995">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-1996">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-1996">VM</span></span>
* <span data-ttu-id="5550f-1997">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="5550f-1997">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="5550f-1998">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="5550f-1998">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="5550f-1999">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="5550f-1999">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="5550f-2000">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2000">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2001">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2001">Core</span></span>
* <span data-ttu-id="5550f-2002">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="5550f-2002">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2003">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2003">ACR</span></span>
* <span data-ttu-id="5550f-2004">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="5550f-2004">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-2005">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-2005">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="5550f-2008">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2008">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="5550f-2009">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2009">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2010">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2010">AppService</span></span>
* <span data-ttu-id="5550f-2011">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2011">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="5550f-2012">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2012">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="5550f-2013">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2013">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="5550f-2014">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-2014">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="5550f-2015">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-2015">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="5550f-2016">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2016">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="5550f-2017">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-2017">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-2018">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-2018">CDN</span></span>
* <span data-ttu-id="5550f-2019">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2019">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="5550f-2020">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5550f-2020">Feedback</span></span>
* <span data-ttu-id="5550f-2021">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-2021">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="5550f-2022">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2022">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="5550f-2023">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="5550f-2023">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2024">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2024">Monitor</span></span>
* <span data-ttu-id="5550f-2025">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2025">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="5550f-2026">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2026">Network</span></span>
* <span data-ttu-id="5550f-2027">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2027">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="5550f-2028">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2028">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="5550f-2029">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2029">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="5550f-2030">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2030">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="5550f-2031">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="5550f-2031">PrivateDNS</span></span>
* <span data-ttu-id="5550f-2032">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2032">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2033">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2033">Resource</span></span>
* <span data-ttu-id="5550f-2034">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="5550f-2034">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2035">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2035">Role</span></span>
* <span data-ttu-id="5550f-2036">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="5550f-2036">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="5550f-2037">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="5550f-2037">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2038">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2038">SQL</span></span>
* <span data-ttu-id="5550f-2039">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="5550f-2039">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2040">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2040">Storage</span></span>
* <span data-ttu-id="5550f-2041">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2041">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="5550f-2042">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2042">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="5550f-2043">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="5550f-2043">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="5550f-2044">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-2044">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="5550f-2045">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2045">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="5550f-2046">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2046">Core</span></span>
* <span data-ttu-id="5550f-2047">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2047">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="5550f-2048">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="5550f-2048">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-2049">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-2049">Cloud</span></span>
* <span data-ttu-id="5550f-2050">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2050">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2051">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2051">ACR</span></span>
* <span data-ttu-id="5550f-2052">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2052">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="5550f-2053">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2053">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="5550f-2054">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="5550f-2054">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="5550f-2055">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2055">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2056">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2056">AppService</span></span>
* <span data-ttu-id="5550f-2057">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="5550f-2057">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="5550f-2058">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2058">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="5550f-2059">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2059">BOT Service</span></span>
* <span data-ttu-id="5550f-2060">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2060">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="5550f-2061">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="5550f-2061">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="5550f-2062">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2062">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="5550f-2063">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5550f-2063">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-2064">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-2064">CDN</span></span>
* <span data-ttu-id="5550f-2065">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2065">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="5550f-2066">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2066">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="5550f-2067">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2067">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5550f-2068">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5550f-2068">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-2069">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-2069">Cosmosdb</span></span>
* <span data-ttu-id="5550f-2070">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5550f-2070">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="5550f-2071">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5550f-2071">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-2072">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-2072">Interactive</span></span>
* <span data-ttu-id="5550f-2073">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="5550f-2073">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2074">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2074">Monitor</span></span>
* <span data-ttu-id="5550f-2075">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2075">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2076">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2076">Network</span></span>
* <span data-ttu-id="5550f-2077">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2077">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-2078">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-2078">Profile</span></span>
* <span data-ttu-id="5550f-2079">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2079">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="5550f-2080">Postgres</span><span class="sxs-lookup"><span data-stu-id="5550f-2080">Postgres</span></span> 
* <span data-ttu-id="5550f-2081">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2081">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="5550f-2082">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2082">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2083">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2083">Resource</span></span>
* <span data-ttu-id="5550f-2084">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2084">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="5550f-2085">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="5550f-2085">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="5550f-2086">График</span><span class="sxs-lookup"><span data-stu-id="5550f-2086">Graph</span></span>
* <span data-ttu-id="5550f-2087">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2087">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="5550f-2088">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2088">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="5550f-2089">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2089">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="5550f-2090">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="5550f-2090">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="5550f-2091">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="5550f-2091">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2092">носителей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2092">storage</span></span>
* <span data-ttu-id="5550f-2093">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2093">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="5550f-2094">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="5550f-2094">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="5550f-2095">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="5550f-2095">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="5550f-2096">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="5550f-2096">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2097">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2097">VM</span></span>
* <span data-ttu-id="5550f-2098">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2098">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="5550f-2099">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2099">March 12, 2019</span></span>

<span data-ttu-id="5550f-2100">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="5550f-2100">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2101">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2101">Core</span></span>

* <span data-ttu-id="5550f-2102">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="5550f-2102">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2103">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2103">ACR</span></span>

* <span data-ttu-id="5550f-2104">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2104">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2105">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2105">ACS</span></span>

* <span data-ttu-id="5550f-2106">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="5550f-2106">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="5550f-2107">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2107">AppService</span></span>

* <span data-ttu-id="5550f-2108">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-2108">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="5550f-2109">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2109">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="5550f-2110">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-2110">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="5550f-2111">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="5550f-2111">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-2112">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2112">Botservice</span></span>

* <span data-ttu-id="5550f-2113">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5550f-2113">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5550f-2114">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5550f-2114">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5550f-2115">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2115">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="5550f-2116">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="5550f-2116">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2117">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2117">Container</span></span>

* <span data-ttu-id="5550f-2118">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="5550f-2118">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-2119">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-2119">EventHub</span></span>

* <span data-ttu-id="5550f-2120">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="5550f-2120">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="5550f-2121">Поиск</span><span class="sxs-lookup"><span data-stu-id="5550f-2121">Find</span></span>

* <span data-ttu-id="5550f-2122">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="5550f-2122">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-2123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-2123">HDInsight</span></span>

* <span data-ttu-id="5550f-2124">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2124">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2125">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2125">Network</span></span>

* <span data-ttu-id="5550f-2126">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2126">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5550f-2127">Rdbms</span></span>

* <span data-ttu-id="5550f-2128">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2128">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2129">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2129">Role</span></span>

* <span data-ttu-id="5550f-2130">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2130">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="5550f-2131">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-2131">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-2132">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-2132">Service Fabric</span></span>

* <span data-ttu-id="5550f-2133">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="5550f-2133">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="5550f-2134">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2134">February 26, 2019</span></span>

<span data-ttu-id="5550f-2135">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="5550f-2135">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2136">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2136">Core</span></span>

* <span data-ttu-id="5550f-2137">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="5550f-2137">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2138">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2138">ACR</span></span>

* <span data-ttu-id="5550f-2139">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2139">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="5550f-2140">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-2140">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2141">ACS</span></span>

* <span data-ttu-id="5550f-2142">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2142">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2143">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2143">AppService</span></span>

* <span data-ttu-id="5550f-2144">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2144">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2145">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2145">Batch</span></span>
* <span data-ttu-id="5550f-2146">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2146">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="5550f-2147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2147">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="5550f-2148">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2148">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="5550f-2149">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2149">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="5550f-2150">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="5550f-2150">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="5550f-2151">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-2151">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-2152">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-2152">CosmosDB</span></span>

* <span data-ttu-id="5550f-2153">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5550f-2153">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="5550f-2154">Kusto</span><span class="sxs-lookup"><span data-stu-id="5550f-2154">Kusto</span></span>

* <span data-ttu-id="5550f-2155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="5550f-2155">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2156">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2156">Network</span></span>

* <span data-ttu-id="5550f-2157">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-2157">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="5550f-2158">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2158">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="5550f-2159">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2159">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="5550f-2160">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2160">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="5550f-2161">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2161">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="5550f-2162">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-2162">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="5550f-2163">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2163">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2164">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2164">Resource</span></span>

* <span data-ttu-id="5550f-2165">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-2165">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="5550f-2166">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2166">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="5550f-2167">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2167">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="5550f-2168">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2168">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="5550f-2169">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2169">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2170">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2170">Role</span></span>

* <span data-ttu-id="5550f-2171">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2171">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2172">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2172">VM</span></span>

* <span data-ttu-id="5550f-2173">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-2173">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="5550f-2174">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2174">February 12, 2019</span></span>

<span data-ttu-id="5550f-2175">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="5550f-2175">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2176">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2176">Core</span></span>

* <span data-ttu-id="5550f-2177">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="5550f-2177">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="5550f-2178">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-2178">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2179">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2179">ACR</span></span>
* <span data-ttu-id="5550f-2180">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2180">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="5550f-2181">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2181">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2182">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2182">ACS</span></span>
* <span data-ttu-id="5550f-2183">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5550f-2183">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="5550f-2184">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2184">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="5550f-2185">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="5550f-2185">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-2186">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-2186">AMS</span></span>
* <span data-ttu-id="5550f-2187">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2187">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="5550f-2188">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2188">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2189">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2189">Appservice</span></span>
* <span data-ttu-id="5550f-2190">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-2190">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="5550f-2191">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-2191">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="5550f-2192">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2192">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="5550f-2193">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-2193">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="5550f-2194">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2194">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-2195">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2195">Botservice</span></span>
* <span data-ttu-id="5550f-2196">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2196">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="5550f-2197">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2197">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="5550f-2198">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2198">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="5550f-2199">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5550f-2199">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="5550f-2200">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2200">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="5550f-2201">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-2201">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="5550f-2202">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2202">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="5550f-2203">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-2203">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="5550f-2204">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="5550f-2204">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="5550f-2205">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="5550f-2205">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-2206">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-2206">Key Vault</span></span>
* <span data-ttu-id="5550f-2207">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2207">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2208">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2208">Monitor</span></span>
* <span data-ttu-id="5550f-2209">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2209">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2210">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2210">Network</span></span>
* <span data-ttu-id="5550f-2211">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="5550f-2211">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="5550f-2212">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2212">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="5550f-2213">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-2213">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="5550f-2214">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2214">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5550f-2215">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5550f-2215">Policy Insights</span></span>
* <span data-ttu-id="5550f-2216">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2216">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2217">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-2217">RDBMS</span></span>
* <span data-ttu-id="5550f-2218">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-2218">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-2219">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-2219">Redis</span></span>
* <span data-ttu-id="5550f-2220">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5550f-2220">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="5550f-2221">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5550f-2221">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="5550f-2222">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="5550f-2222">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="5550f-2223">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="5550f-2223">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="5550f-2224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2224">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="5550f-2225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="5550f-2225">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="5550f-2226">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5550f-2226">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2227">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2227">Role</span></span>
* <span data-ttu-id="5550f-2228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2228">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5550f-2229">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2229">SQL VM</span></span>
* <span data-ttu-id="5550f-2230">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2230">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2231">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2231">VM</span></span>
* <span data-ttu-id="5550f-2232">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2232">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="5550f-2233">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2233">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="5550f-2234">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="5550f-2234">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="5550f-2235">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2235">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="5550f-2236">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2236">January 31, 2019</span></span>

<span data-ttu-id="5550f-2237">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="5550f-2237">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2238">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2238">Core</span></span>

* <span data-ttu-id="5550f-2239">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="5550f-2239">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="5550f-2240">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2240">January 28, 2019</span></span>

<span data-ttu-id="5550f-2241">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="5550f-2241">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2242">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2242">ACR</span></span>
* <span data-ttu-id="5550f-2243">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2243">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2244">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2244">ACS</span></span>
* <span data-ttu-id="5550f-2245">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2245">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5550f-2246">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="5550f-2246">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="5550f-2247">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2247">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-2248">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-2248">AMS</span></span>
* <span data-ttu-id="5550f-2249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2249">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="5550f-2250">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2250">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2251">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2251">Appservice</span></span>
* <span data-ttu-id="5550f-2252">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2252">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="5550f-2253">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-2253">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="5550f-2254">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5550f-2254">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2255">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2255">Container</span></span>
* <span data-ttu-id="5550f-2256">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2256">Added `container start` command</span></span>
* <span data-ttu-id="5550f-2257">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2257">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5550f-2258">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5550f-2258">EventGrid</span></span>
* <span data-ttu-id="5550f-2259">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2259">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="5550f-2260">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2260">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="5550f-2261">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-2261">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="5550f-2262">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="5550f-2262">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="5550f-2263">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-2263">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-2264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-2264">HDInsight</span></span>
* <span data-ttu-id="5550f-2265">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2265">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="5550f-2266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2266">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="5550f-2267">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2267">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="5550f-2268">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="5550f-2268">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="5550f-2269">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2269">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="5550f-2270">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2270">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-2271">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-2271">IoT</span></span>
* <span data-ttu-id="5550f-2272">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="5550f-2272">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="5550f-2273">Kusto</span><span class="sxs-lookup"><span data-stu-id="5550f-2273">Kusto</span></span>
* <span data-ttu-id="5550f-2274">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5550f-2274">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2275">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2275">Monitor</span></span>
* <span data-ttu-id="5550f-2276">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-2276">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-2277">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-2277">Profile</span></span>
* <span data-ttu-id="5550f-2278">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2278">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2279">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2279">Network</span></span>
* <span data-ttu-id="5550f-2280">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2280">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="5550f-2281">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="5550f-2281">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2282">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2282">Resource</span></span>
* <span data-ttu-id="5550f-2283">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2283">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="5550f-2284">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2284">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="5550f-2285">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2285">SQL Virtual Machine</span></span>
* <span data-ttu-id="5550f-2286">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5550f-2286">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2287">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2287">Storage</span></span>
* <span data-ttu-id="5550f-2288">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="5550f-2288">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="5550f-2289">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="5550f-2289">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2290">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2290">VM</span></span>
* <span data-ttu-id="5550f-2291">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="5550f-2291">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="5550f-2292">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2292">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="5550f-2293">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2293">January 15, 2019</span></span>

<span data-ttu-id="5550f-2294">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="5550f-2294">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2295">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2295">ACR</span></span>
* <span data-ttu-id="5550f-2296">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="5550f-2296">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="5550f-2297">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5550f-2297">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="5550f-2298">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="5550f-2298">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="5550f-2299">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2299">ACS</span></span>
* <span data-ttu-id="5550f-2300">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="5550f-2300">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2301">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2301">Appservice</span></span>
* <span data-ttu-id="5550f-2302">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2302">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="5550f-2303">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-2303">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="5550f-2304">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="5550f-2304">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="5550f-2305">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2305">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-2306">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2306">Botservice</span></span>
* <span data-ttu-id="5550f-2307">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2307">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="5550f-2308">Configure</span><span class="sxs-lookup"><span data-stu-id="5550f-2308">Configure</span></span>
* <span data-ttu-id="5550f-2309">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2309">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-2310">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-2310">CosmosDB</span></span>
* <span data-ttu-id="5550f-2311">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="5550f-2311">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-2312">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-2312">HDInsight</span></span>
* <span data-ttu-id="5550f-2313">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="5550f-2313">Added commands for managing applications</span></span>
* <span data-ttu-id="5550f-2314">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2314">Added commands for managing script actions</span></span>
* <span data-ttu-id="5550f-2315">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="5550f-2315">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="5550f-2316">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2316">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="5550f-2317">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2317">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2318">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2318">Network</span></span>
* <span data-ttu-id="5550f-2319">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-2319">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="5550f-2320">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="5550f-2320">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="5550f-2321">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-2321">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="5550f-2322">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2322">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2323">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2323">Role</span></span>
* <span data-ttu-id="5550f-2324">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5550f-2324">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="5550f-2325">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-2325">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="5550f-2326">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5550f-2326">Security</span></span>
* <span data-ttu-id="5550f-2327">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-2327">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2328">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2328">Storage</span></span>
* <span data-ttu-id="5550f-2329">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="5550f-2329">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="5550f-2330">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2330">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="5550f-2331">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2331">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="5550f-2332">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2332">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="5550f-2333">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2333">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2334">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2334">VM</span></span>
* <span data-ttu-id="5550f-2335">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2335">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="5550f-2336">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2336">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5550f-2337">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2337">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="5550f-2338">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2338">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="5550f-2339">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2339">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="5550f-2340">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2340">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="5550f-2341">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2341">December 20, 2018</span></span>

<span data-ttu-id="5550f-2342">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="5550f-2342">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="5550f-2343">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2343">Appservice</span></span>
* <span data-ttu-id="5550f-2344">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="5550f-2344">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="5550f-2345">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5550f-2345">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="5550f-2346">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-2346">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5550f-2347">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-2347">IoTCentral</span></span>
* <span data-ttu-id="5550f-2348">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="5550f-2348">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2349">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2349">Role</span></span>
* <span data-ttu-id="5550f-2350">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2350">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2351">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2351">SQL</span></span>
* <span data-ttu-id="5550f-2352">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5550f-2352">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2353">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2353">VM</span></span>
* <span data-ttu-id="5550f-2354">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2354">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="5550f-2355">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2355">December 18, 2018</span></span>

<span data-ttu-id="5550f-2356">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="5550f-2356">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="5550f-2357">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2357">ACR</span></span>
* <span data-ttu-id="5550f-2358">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2358">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="5550f-2359">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="5550f-2359">Condensed the table layout for task list</span></span>
* <span data-ttu-id="5550f-2360">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="5550f-2360">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2361">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2361">ACS</span></span>
* <span data-ttu-id="5550f-2362">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2362">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5550f-2363">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="5550f-2363">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="5550f-2364">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5550f-2364">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="5550f-2365">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2365">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="5550f-2366">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2366">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="5550f-2367">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2367">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2368">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2368">Appservice</span></span>
* <span data-ttu-id="5550f-2369">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2369">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="5550f-2370">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2370">Botservice</span></span>
* <span data-ttu-id="5550f-2371">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2371">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="5550f-2372">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="5550f-2372">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="5550f-2373">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="5550f-2373">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="5550f-2374">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="5550f-2374">Reduced Kudu network calls</span></span>
* <span data-ttu-id="5550f-2375">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-2375">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-2376">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-2376">Consumption</span></span>
* <span data-ttu-id="5550f-2377">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2377">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-2378">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-2378">CosmosDB</span></span>
* <span data-ttu-id="5550f-2379">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="5550f-2379">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="5550f-2380">Maps</span><span class="sxs-lookup"><span data-stu-id="5550f-2380">Maps</span></span>
* <span data-ttu-id="5550f-2381">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="5550f-2381">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2382">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2382">Network</span></span>
* <span data-ttu-id="5550f-2383">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2383">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="5550f-2384">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="5550f-2384">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2385">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2385">Resource</span></span>
* <span data-ttu-id="5550f-2386">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2386">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="5550f-2387">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2387">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2388">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2388">Storage</span></span>
*  <span data-ttu-id="5550f-2389">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-2389">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2390">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2390">VM</span></span>
* <span data-ttu-id="5550f-2391">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2391">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="5550f-2392">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2392">December 4, 2018</span></span>

<span data-ttu-id="5550f-2393">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="5550f-2393">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="5550f-2394">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2394">Core</span></span>
* <span data-ttu-id="5550f-2395">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2395">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="5550f-2396">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="5550f-2396">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2397">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2397">Appservice</span></span>
* <span data-ttu-id="5550f-2398">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2398">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="5550f-2399">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="5550f-2399">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2400">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2400">Network</span></span>
* <span data-ttu-id="5550f-2401">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="5550f-2401">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2402">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2402">Role</span></span>
* <span data-ttu-id="5550f-2403">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2403">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="5550f-2404">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2404">VM</span></span>
* <span data-ttu-id="5550f-2405">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5550f-2405">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="5550f-2406">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="5550f-2406">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="5550f-2407">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="5550f-2407">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="5550f-2408">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-2408">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="5550f-2409">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2409">November 20, 2018</span></span>

<span data-ttu-id="5550f-2410">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="5550f-2410">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="5550f-2411">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2411">Core</span></span>
* <span data-ttu-id="5550f-2412">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="5550f-2412">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2413">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2413">ACR</span></span>
* <span data-ttu-id="5550f-2414">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="5550f-2414">Added context token to task step</span></span>
* <span data-ttu-id="5550f-2415">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-2415">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="5550f-2416">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2416">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2417">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-2417">Appservice</span></span>
* <span data-ttu-id="5550f-2418">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2418">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="5550f-2419">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2419">Updated the default `node_version`.</span></span> <span data-ttu-id="5550f-2420">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2420">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="5550f-2421">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="5550f-2421">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="5550f-2422">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5550f-2422">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5550f-2423">IotCentral</span><span class="sxs-lookup"><span data-stu-id="5550f-2423">IotCentral</span></span>
* <span data-ttu-id="5550f-2424">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5550f-2424">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-2425">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-2425">KeyVault</span></span>
* <span data-ttu-id="5550f-2426">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="5550f-2426">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2427">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2427">Network</span></span>
* <span data-ttu-id="5550f-2428">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2428">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="5550f-2429">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2429">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="5550f-2430">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="5550f-2430">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="5550f-2431">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2431">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2432">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5550f-2432">Rdbms</span></span>
* <span data-ttu-id="5550f-2433">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-2433">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="5550f-2434">RBAC:</span><span class="sxs-lookup"><span data-stu-id="5550f-2434">Rbac</span></span>
* <span data-ttu-id="5550f-2435">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2435">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="5550f-2436">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="5550f-2436">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="5550f-2437">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2437">Storage</span></span>
* <span data-ttu-id="5550f-2438">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-2438">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="5550f-2439">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2439">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="5550f-2440">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5550f-2440">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="5550f-2441">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2441">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2442">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2442">VM</span></span>
* <span data-ttu-id="5550f-2443">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="5550f-2443">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="5550f-2444">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2444">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="5550f-2445">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2445">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="5550f-2446">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="5550f-2446">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="5550f-2447">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2447">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="5550f-2448">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2448">Added `snapshot wait` command</span></span>
* <span data-ttu-id="5550f-2449">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2449">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="5550f-2450">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2450">November 6, 2018</span></span>

<span data-ttu-id="5550f-2451">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="5550f-2451">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2452">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2452">Core</span></span>
* <span data-ttu-id="5550f-2453">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="5550f-2453">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2454">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2454">ACR</span></span>
* <span data-ttu-id="5550f-2455">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="5550f-2455">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="5550f-2456">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="5550f-2456">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2457">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2457">ACS</span></span>
* <span data-ttu-id="5550f-2458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2458">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="5550f-2459">Помощник</span><span class="sxs-lookup"><span data-stu-id="5550f-2459">Advisor</span></span>
* <span data-ttu-id="5550f-2460">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5550f-2460">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-2461">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-2461">AMS</span></span>
* <span data-ttu-id="5550f-2462">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="5550f-2462">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="5550f-2463">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="5550f-2463">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="5550f-2464">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2464">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="5550f-2465">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="5550f-2465">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="5550f-2466">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2466">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="5550f-2467">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2467">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="5550f-2468">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2468">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="5550f-2469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2469">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="5550f-2470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2470">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="5550f-2471">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2471">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="5550f-2472">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2472">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="5550f-2473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2473">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="5550f-2474">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="5550f-2474">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="5550f-2475">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="5550f-2475">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="5550f-2476">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2476">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="5550f-2477">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="5550f-2477">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="5550f-2478">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="5550f-2478">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2479">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2479">AppService</span></span>
* <span data-ttu-id="5550f-2480">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="5550f-2480">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="5550f-2481">Configure</span><span class="sxs-lookup"><span data-stu-id="5550f-2481">Configure</span></span>
* <span data-ttu-id="5550f-2482">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-2482">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2483">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2483">Container</span></span>
* <span data-ttu-id="5550f-2484">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="5550f-2484">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="5550f-2485">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5550f-2485">EventHub</span></span>
* <span data-ttu-id="5550f-2486">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2486">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-2487">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-2487">Interactive</span></span>
* <span data-ttu-id="5550f-2488">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="5550f-2488">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2489">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2489">Monitor</span></span>
* <span data-ttu-id="5550f-2490">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2490">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2491">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2491">Network</span></span>
* <span data-ttu-id="5550f-2492">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2492">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="5550f-2493">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5550f-2493">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="5550f-2494">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2494">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="5550f-2495">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-2495">Profile</span></span>
* <span data-ttu-id="5550f-2496">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2496">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2497">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-2497">RDBMS</span></span>
* <span data-ttu-id="5550f-2498">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-2498">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2499">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2499">Resource</span></span>
* <span data-ttu-id="5550f-2500">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2500">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2501">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2501">Role</span></span>
* <span data-ttu-id="5550f-2502">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2502">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="5550f-2503">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2503">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="5550f-2504">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="5550f-2504">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2505">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2505">Storage</span></span>
* <span data-ttu-id="5550f-2506">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2506">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2507">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2507">VM</span></span>
* <span data-ttu-id="5550f-2508">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-2508">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="5550f-2509">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-2509">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="5550f-2510">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="5550f-2510">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="5550f-2511">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="5550f-2511">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="5550f-2512">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-2512">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="5550f-2513">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2513">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="5550f-2514">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2514">October 23, 2018</span></span>

<span data-ttu-id="5550f-2515">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="5550f-2515">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2516">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2516">Core</span></span>
* <span data-ttu-id="5550f-2517">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2517">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="5550f-2518">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2518">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2519">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2519">ACR</span></span>
* <span data-ttu-id="5550f-2520">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="5550f-2520">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-2521">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-2521">CDN</span></span>
* <span data-ttu-id="5550f-2522">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2522">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5550f-2523">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5550f-2523">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2524">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2524">Container</span></span>
* <span data-ttu-id="5550f-2525">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="5550f-2525">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="5550f-2526">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="5550f-2526">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="5550f-2527">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2527">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="5550f-2528">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2528">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="5550f-2529">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2529">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="5550f-2530">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2530">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="5550f-2531">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2531">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-2532">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-2532">CosmosDB</span></span>
* <span data-ttu-id="5550f-2533">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2533">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-2534">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-2534">Interactive</span></span>
* <span data-ttu-id="5550f-2535">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2535">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-2536">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-2536">IoT Central</span></span>
* <span data-ttu-id="5550f-2537">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5550f-2537">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="5550f-2538">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="5550f-2538">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2539">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2539">Monitor</span></span>
* <span data-ttu-id="5550f-2540">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="5550f-2540">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="5550f-2541">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2541">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="5550f-2542">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-2542">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5550f-2543">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-2543">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="5550f-2544">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2544">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="5550f-2545">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="5550f-2545">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="5550f-2546">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="5550f-2546">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="5550f-2547">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-2547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5550f-2548">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-2548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="5550f-2549">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2549">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2550">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2550">Network</span></span>
* <span data-ttu-id="5550f-2551">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5550f-2551">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="5550f-2552">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5550f-2552">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="5550f-2553">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-2553">ServiceBus</span></span>
* <span data-ttu-id="5550f-2554">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5550f-2554">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2555">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2555">SQL</span></span>
* <span data-ttu-id="5550f-2556">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5550f-2556">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2557">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2557">Storage</span></span>
* <span data-ttu-id="5550f-2558">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2558">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="5550f-2559">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="5550f-2559">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2560">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2560">VM</span></span>
* <span data-ttu-id="5550f-2561">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="5550f-2561">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="5550f-2562">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="5550f-2562">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="5550f-2563">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="5550f-2563">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="5550f-2564">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2564">October 16, 2018</span></span>

<span data-ttu-id="5550f-2565">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="5550f-2565">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2566">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2566">VM</span></span>
* <span data-ttu-id="5550f-2567">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2567">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="5550f-2568">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2568">October 9, 2018</span></span>

<span data-ttu-id="5550f-2569">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="5550f-2569">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2570">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2570">Core</span></span>
* <span data-ttu-id="5550f-2571">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="5550f-2571">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2572">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2572">ACR</span></span>
* <span data-ttu-id="5550f-2573">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="5550f-2573">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2574">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2574">ACS</span></span>
* <span data-ttu-id="5550f-2575">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="5550f-2575">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="5550f-2576">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="5550f-2576">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="5550f-2577">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2577">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="5550f-2578">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2578">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2579">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2579">Container</span></span>
* <span data-ttu-id="5550f-2580">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2580">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="5550f-2581">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-2581">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="5550f-2582">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="5550f-2582">Event Hub</span></span>
* <span data-ttu-id="5550f-2583">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2583">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="5550f-2584">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5550f-2584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="5550f-2585">Модули</span><span class="sxs-lookup"><span data-stu-id="5550f-2585">Extensions</span></span>
* <span data-ttu-id="5550f-2586">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="5550f-2586">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5550f-2587">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5550f-2587">HDInsight</span></span>
* <span data-ttu-id="5550f-2588">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-2588">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-2589">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-2589">IoT</span></span>
* <span data-ttu-id="5550f-2590">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2590">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-2591">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-2591">KeyVault</span></span>
* <span data-ttu-id="5550f-2592">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="5550f-2592">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2593">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2593">Network</span></span>
* <span data-ttu-id="5550f-2594">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2594">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="5550f-2595">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="5550f-2595">See #6052</span></span>
* <span data-ttu-id="5550f-2596">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2596">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="5550f-2597">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5550f-2597">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="5550f-2598">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2598">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="5550f-2599">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2599">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="5550f-2600">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2600">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="5550f-2601">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2601">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2602">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2602">Role</span></span>
* <span data-ttu-id="5550f-2603">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2603">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="5550f-2604">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2604">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="5550f-2605">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2605">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="5550f-2606">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="5550f-2606">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="5550f-2607">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-2607">Service Bus</span></span>
* <span data-ttu-id="5550f-2608">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5550f-2608">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2609">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2609">VM</span></span>
* <span data-ttu-id="5550f-2610">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2610">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="5550f-2611">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2611">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="5550f-2612">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2612">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="5550f-2613">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2613">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="5550f-2614">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2614">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="5550f-2615">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="5550f-2615">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="5550f-2616">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2616">September 21, 2018</span></span>

<span data-ttu-id="5550f-2617">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="5550f-2617">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2618">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2618">ACR</span></span>
* <span data-ttu-id="5550f-2619">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-2619">Added ACR Task commands</span></span>
* <span data-ttu-id="5550f-2620">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="5550f-2620">Added quick run command</span></span>
* <span data-ttu-id="5550f-2621">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2621">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="5550f-2622">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-2622">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="5550f-2623">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="5550f-2623">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="5550f-2624">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2624">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2625">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2625">ACS</span></span>
* <span data-ttu-id="5550f-2626">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2626">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="5550f-2627">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2627">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2628">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2628">AppService</span></span>

* <span data-ttu-id="5550f-2629">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="5550f-2629">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="5550f-2630">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="5550f-2630">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="5550f-2631">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2631">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="5550f-2632">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5550f-2632">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2633">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2633">Batch</span></span>
* <span data-ttu-id="5550f-2634">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="5550f-2634">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="5550f-2635">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2635">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="5550f-2636">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2636">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="5550f-2637">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="5550f-2637">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5550f-2638">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-2638">Batch AI</span></span> 
* <span data-ttu-id="5550f-2639">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2639">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-2640">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-2640">Cognitive Services</span></span>
* <span data-ttu-id="5550f-2641">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2641">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="5550f-2642">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2642">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="5550f-2643">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2643">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="5550f-2644">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2644">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="5550f-2645">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5550f-2645">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="5550f-2646">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2646">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2647">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2647">Container</span></span>
* <span data-ttu-id="5550f-2648">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2648">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="5550f-2649">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="5550f-2649">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="5550f-2650">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-2650">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="5550f-2651">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2651">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="5550f-2652">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5550f-2652">Datalake</span></span>
* <span data-ttu-id="5550f-2653">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-2653">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="5550f-2654">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="5550f-2654">Interactive Shell</span></span>
* <span data-ttu-id="5550f-2655">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-2655">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="5550f-2656">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2656">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-2657">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-2657">IoT</span></span>
* <span data-ttu-id="5550f-2658">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2658">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-2659">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5550f-2659">Key Vault</span></span>
* <span data-ttu-id="5550f-2660">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="5550f-2660">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2661">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2661">Network</span></span>
* <span data-ttu-id="5550f-2662">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2662">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="5550f-2663">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2663">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="5550f-2664">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="5550f-2664">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="5550f-2665">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2665">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="5550f-2666">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2666">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="5550f-2667">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2667">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="5550f-2668">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-2668">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="5550f-2669">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2669">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="5550f-2670">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2670">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="5550f-2671">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2671">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="5550f-2672">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2672">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="5550f-2673">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2673">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="5550f-2674">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2674">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="5550f-2675">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="5550f-2675">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="5550f-2676">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2676">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="5550f-2677">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2677">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="5550f-2678">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5550f-2678">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="5550f-2679">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5550f-2679">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2680">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-2680">RDBMS</span></span>
* <span data-ttu-id="5550f-2681">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5550f-2681">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="5550f-2682">резервирование.</span><span class="sxs-lookup"><span data-stu-id="5550f-2682">Reservation</span></span>
* <span data-ttu-id="5550f-2683">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2683">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="5550f-2684">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="5550f-2684">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="5550f-2685">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="5550f-2685">Manage App</span></span>
* <span data-ttu-id="5550f-2686">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5550f-2686">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="5550f-2687">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5550f-2687">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2688">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2688">Role</span></span>
* <span data-ttu-id="5550f-2689">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="5550f-2689">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="5550f-2690">SignalR</span><span class="sxs-lookup"><span data-stu-id="5550f-2690">SignalR</span></span>
* <span data-ttu-id="5550f-2691">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-2691">First release</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2692">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2692">Storage</span></span>
* <span data-ttu-id="5550f-2693">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="5550f-2693">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="5550f-2694">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="5550f-2694">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2695">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2695">VM</span></span>
* <span data-ttu-id="5550f-2696">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="5550f-2696">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="5550f-2697">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2697">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="5550f-2698">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2698">August 28, 2018</span></span>

<span data-ttu-id="5550f-2699">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="5550f-2699">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2700">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2700">Core</span></span>

* <span data-ttu-id="5550f-2701">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5550f-2701">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="5550f-2702">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5550f-2702">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2703">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2703">ACR</span></span>

* <span data-ttu-id="5550f-2704">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5550f-2704">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="5550f-2705">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2705">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2706">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2706">ACS</span></span>

* <span data-ttu-id="5550f-2707">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2707">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="5550f-2708">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-2708">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2709">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2709">AppService</span></span>

* <span data-ttu-id="5550f-2710">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="5550f-2710">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="5550f-2711">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="5550f-2711">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="5550f-2712">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2712">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-2713">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-2713">Backup</span></span>

* <span data-ttu-id="5550f-2714">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2714">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="5550f-2715">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2715">Bot Service</span></span>

* <span data-ttu-id="5550f-2716">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="5550f-2716">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-2717">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-2717">Cognitive Services</span></span>

* <span data-ttu-id="5550f-2718">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="5550f-2718">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-2719">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-2719">IoT</span></span>

* <span data-ttu-id="5550f-2720">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="5550f-2720">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-2721">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-2721">Monitor</span></span>

* <span data-ttu-id="5550f-2722">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-2722">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="5550f-2723">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2723">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2724">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2724">Network</span></span>

* <span data-ttu-id="5550f-2725">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2725">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2726">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2726">Resource</span></span>

* <span data-ttu-id="5550f-2727">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2727">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2728">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2728">Storage</span></span>

* <span data-ttu-id="5550f-2729">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2729">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2730">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2730">VM</span></span>

* <span data-ttu-id="5550f-2731">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5550f-2731">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="5550f-2732">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2732">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="5550f-2733">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2733">Auguest 14, 2018</span></span>

<span data-ttu-id="5550f-2734">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="5550f-2734">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2735">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2735">Core</span></span>

* <span data-ttu-id="5550f-2736">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2736">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="5550f-2737">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="5550f-2737">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="5550f-2738">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="5550f-2738">Telemetry</span></span>

* <span data-ttu-id="5550f-2739">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-2739">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2740">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2740">ACR</span></span>

* <span data-ttu-id="5550f-2741">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2741">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="5550f-2742">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2742">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2743">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2743">ACS</span></span>

* <span data-ttu-id="5550f-2744">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-2744">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="5550f-2745">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="5550f-2745">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="5550f-2746">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5550f-2746">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="5550f-2747">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5550f-2747">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="5550f-2748">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-2748">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="5550f-2749">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2749">AppService</span></span>

* <span data-ttu-id="5550f-2750">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2750">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="5550f-2751">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5550f-2751">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-2752">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-2752">BatchAI</span></span>

* <span data-ttu-id="5550f-2753">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов* .</span><span class="sxs-lookup"><span data-stu-id="5550f-2753">Changed logger output for auto-storage account creation to specifies "resource *group* ".</span></span>        

### <a name="container"></a><span data-ttu-id="5550f-2754">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2754">Container</span></span>

* <span data-ttu-id="5550f-2755">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="5550f-2755">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="5550f-2756">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-2756">IoT</span></span>

* <span data-ttu-id="5550f-2757">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2757">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="5550f-2758">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2758">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="5550f-2759">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-2759">Iot Central</span></span>

* <span data-ttu-id="5550f-2760">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="5550f-2760">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-2761">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-2761">KeyVault</span></span>


* <span data-ttu-id="5550f-2762">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2762">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="5550f-2763">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-2763">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="5550f-2764">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="5550f-2764">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="5550f-2765">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2765">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="5550f-2766">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2766">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="5550f-2767">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="5550f-2767">Relay</span></span>

* <span data-ttu-id="5550f-2768">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-2768">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2769">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2769">Sql</span></span>

* <span data-ttu-id="5550f-2770">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2770">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2771">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2771">Storage</span></span>

* <span data-ttu-id="5550f-2772">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="5550f-2772">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="5550f-2773">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="5550f-2773">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="5550f-2774">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2774">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="5550f-2775">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="5550f-2775">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="5550f-2776">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="5550f-2776">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2777">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2777">VM</span></span>

* <span data-ttu-id="5550f-2778">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="5550f-2778">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="5550f-2779">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2779">July 31, 2018</span></span>

<span data-ttu-id="5550f-2780">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="5550f-2780">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2781">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2781">ACR</span></span>

* <span data-ttu-id="5550f-2782">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2782">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="5550f-2783">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2783">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2784">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2784">ACS</span></span>

* <span data-ttu-id="5550f-2785">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="5550f-2785">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2786">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2786">Batch</span></span>

* <span data-ttu-id="5550f-2787">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="5550f-2787">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2788">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2788">Container</span></span>

* <span data-ttu-id="5550f-2789">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2789">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2790">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2790">Network</span></span>

* <span data-ttu-id="5550f-2791">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="5550f-2791">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="5550f-2792">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2792">Resource</span></span>

* <span data-ttu-id="5550f-2793">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2793">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="5550f-2794">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="5550f-2794">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2795">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2795">Role</span></span>

* <span data-ttu-id="5550f-2796">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5550f-2796">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="5550f-2797">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="5550f-2797">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="5550f-2798">Поиск</span><span class="sxs-lookup"><span data-stu-id="5550f-2798">Search</span></span>

* <span data-ttu-id="5550f-2799">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="5550f-2799">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="5550f-2800">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-2800">Service Bus</span></span>

* <span data-ttu-id="5550f-2801">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5550f-2801">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="5550f-2802">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="5550f-2802">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="5550f-2803">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="5550f-2803">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="5550f-2804">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2804">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2805">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2805">Storage</span></span>

* <span data-ttu-id="5550f-2806">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2806">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="5550f-2807">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="5550f-2807">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2808">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2808">VM</span></span>

* <span data-ttu-id="5550f-2809">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="5550f-2809">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="5550f-2810">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2810">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="5550f-2811">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-2811">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="5550f-2812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="5550f-2812">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="5550f-2813">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2813">July 18, 2018</span></span>

<span data-ttu-id="5550f-2814">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="5550f-2814">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2815">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2815">Core</span></span>

* <span data-ttu-id="5550f-2816">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="5550f-2816">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="5550f-2817">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="5550f-2817">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="5550f-2818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5550f-2818">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2819">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2819">ACR</span></span>

* <span data-ttu-id="5550f-2820">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="5550f-2820">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="5550f-2821">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2821">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="5550f-2822">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="5550f-2822">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="5550f-2823">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-2823">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2824">ACS</span></span>

* <span data-ttu-id="5550f-2825">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="5550f-2825">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2826">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2826">AppService</span></span>

* <span data-ttu-id="5550f-2827">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="5550f-2827">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2828">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2828">Batch</span></span>

* <span data-ttu-id="5550f-2829">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5550f-2829">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="5550f-2830">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="5550f-2830">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5550f-2831">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-2831">Batch AI</span></span>

* <span data-ttu-id="5550f-2832">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2832">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2833">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2833">Container</span></span>

* <span data-ttu-id="5550f-2834">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="5550f-2834">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="5550f-2835">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="5550f-2835">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2836">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2836">Network</span></span>

* <span data-ttu-id="5550f-2837">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2837">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="5550f-2838">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2838">Added `network nic wait`</span></span>
* <span data-ttu-id="5550f-2839">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5550f-2839">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="5550f-2840">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="5550f-2840">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="5550f-2841">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2841">Resource</span></span>

* <span data-ttu-id="5550f-2842">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2842">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="5550f-2843">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2843">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="5550f-2844">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2844">Added `deployment wait` command</span></span>
* <span data-ttu-id="5550f-2845">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="5550f-2845">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2846">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2846">SQL</span></span>

* <span data-ttu-id="5550f-2847">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2847">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="5550f-2848">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2848">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="5550f-2849">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2849">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2850">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2850">Storage</span></span>

* <span data-ttu-id="5550f-2851">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2851">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2852">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2852">VM</span></span>

* <span data-ttu-id="5550f-2853">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2853">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="5550f-2854">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2854">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="5550f-2855">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2855">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5550f-2856">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2856">July 3, 2018</span></span>

<span data-ttu-id="5550f-2857">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="5550f-2857">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-2858">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-2858">AKS</span></span>

* <span data-ttu-id="5550f-2859">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2859">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5550f-2860">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2860">July 3, 2018</span></span>

<span data-ttu-id="5550f-2861">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="5550f-2861">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2862">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2862">Core</span></span>

* <span data-ttu-id="5550f-2863">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="5550f-2863">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2864">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2864">ACR</span></span>

* <span data-ttu-id="5550f-2865">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="5550f-2865">Added polling build status</span></span>
* <span data-ttu-id="5550f-2866">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5550f-2866">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="5550f-2867">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2867">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2868">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2868">ACS</span></span>

* <span data-ttu-id="5550f-2869">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2869">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="5550f-2870">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2870">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="5550f-2871">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2871">Updated options for `aks browse` command.</span></span> <span data-ttu-id="5550f-2872">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2872">Added `--listen-port` support</span></span>
* <span data-ttu-id="5550f-2873">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2873">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="5550f-2874">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="5550f-2874">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="5550f-2875">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2875">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2876">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2876">AppService</span></span>

* <span data-ttu-id="5550f-2877">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2877">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="5550f-2878">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="5550f-2878">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-2879">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-2879">Backup</span></span>

* <span data-ttu-id="5550f-2880">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="5550f-2880">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-2881">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-2881">BatchAI</span></span>

* <span data-ttu-id="5550f-2882">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2882">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-2883">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-2883">Cloud</span></span>

* <span data-ttu-id="5550f-2884">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2884">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="5550f-2885">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-2885">Container</span></span>

* <span data-ttu-id="5550f-2886">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="5550f-2886">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="5550f-2887">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2887">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="5550f-2888">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="5550f-2888">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-2889">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-2889">Extension</span></span>

* <span data-ttu-id="5550f-2890">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="5550f-2890">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2891">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2891">Network</span></span>

* <span data-ttu-id="5550f-2892">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="5550f-2892">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-2893">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5550f-2893">Rdbms</span></span>

* <span data-ttu-id="5550f-2894">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2894">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-2895">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-2895">Resource</span></span>

* <span data-ttu-id="5550f-2896">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2896">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2897">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2897">VM</span></span>

* <span data-ttu-id="5550f-2898">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5550f-2898">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="5550f-2899">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2899">June 25, 2018</span></span>

<span data-ttu-id="5550f-2900">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="5550f-2900">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="5550f-2901">CLI</span><span class="sxs-lookup"><span data-stu-id="5550f-2901">CLI</span></span>

* <span data-ttu-id="5550f-2902">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-2902">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5550f-2903">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2903">June 19, 2018</span></span>

<span data-ttu-id="5550f-2904">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5550f-2904">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2905">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2905">Core</span></span>

* <span data-ttu-id="5550f-2906">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-2906">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2907">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2907">ACR</span></span>

* <span data-ttu-id="5550f-2908">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2908">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5550f-2909">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="5550f-2909">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-2910">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-2910">ACS</span></span>

* <span data-ttu-id="5550f-2911">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2911">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5550f-2912">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2912">Added `--update` support</span></span>
* <span data-ttu-id="5550f-2913">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2913">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5550f-2914">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2914">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5550f-2915">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2915">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5550f-2916">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2916">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5550f-2917">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2917">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5550f-2918">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2918">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2919">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2919">AppService</span></span>

* <span data-ttu-id="5550f-2920">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="5550f-2920">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5550f-2921">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2921">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2922">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2922">Batch</span></span>

* <span data-ttu-id="5550f-2923">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2923">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5550f-2924">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-2924">Batch AI</span></span>

* <span data-ttu-id="5550f-2925">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="5550f-2925">Added support for workspaces.</span></span> <span data-ttu-id="5550f-2926">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2926">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5550f-2927">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2927">Added support for experiments.</span></span> <span data-ttu-id="5550f-2928">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="5550f-2928">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5550f-2929">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="5550f-2929">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5550f-2930">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2930">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5550f-2931">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2931">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5550f-2932">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2932">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="5550f-2933">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="5550f-2933">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5550f-2934">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2934">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5550f-2935">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2935">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5550f-2936">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2936">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5550f-2937">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2937">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5550f-2938">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2938">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5550f-2939">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="5550f-2939">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5550f-2940">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="5550f-2940">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5550f-2941">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2941">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5550f-2942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="5550f-2942">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="5550f-2943">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="5550f-2943">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="5550f-2944">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="5550f-2944">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5550f-2945">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="5550f-2945">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5550f-2946">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="5550f-2946">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5550f-2947">Maps</span><span class="sxs-lookup"><span data-stu-id="5550f-2947">Maps</span></span>

* <span data-ttu-id="5550f-2948">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2948">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5550f-2949">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-2949">Network</span></span>

* <span data-ttu-id="5550f-2950">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="5550f-2950">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5550f-2951">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-2951">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5550f-2952">#6502</span><span class="sxs-lookup"><span data-stu-id="5550f-2952">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5550f-2953">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5550f-2953">Reservations</span></span>

* <span data-ttu-id="5550f-2954">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2954">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5550f-2955">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2955">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5550f-2956">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2956">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5550f-2957">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2957">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5550f-2958">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2958">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5550f-2959">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2959">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5550f-2960">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-2960">Role</span></span>

* <span data-ttu-id="5550f-2961">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5550f-2961">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-2962">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-2962">SQL</span></span>

* <span data-ttu-id="5550f-2963">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-2963">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-2964">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-2964">Storage</span></span>

* <span data-ttu-id="5550f-2965">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-2965">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-2966">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-2966">VM</span></span>

* <span data-ttu-id="5550f-2967">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2967">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5550f-2968">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2968">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5550f-2969">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="5550f-2969">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5550f-2970">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2970">June 13, 2018</span></span>

<span data-ttu-id="5550f-2971">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5550f-2971">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2972">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2972">Core</span></span>

* <span data-ttu-id="5550f-2973">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="5550f-2973">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5550f-2974">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2974">June 13, 2018</span></span>

<span data-ttu-id="5550f-2975">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5550f-2975">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-2976">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-2976">AKS</span></span>

* <span data-ttu-id="5550f-2977">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="5550f-2977">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5550f-2978">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="5550f-2978">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="5550f-2979">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5550f-2979">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5550f-2980">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5550f-2980">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5550f-2981">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5550f-2981">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-2982">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-2982">AppService</span></span>

* <span data-ttu-id="5550f-2983">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="5550f-2983">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5550f-2984">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2984">June 5, 2018</span></span>

<span data-ttu-id="5550f-2985">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5550f-2985">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-2986">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-2986">Interactive</span></span>

* <span data-ttu-id="5550f-2987">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="5550f-2987">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5550f-2988">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-2988">June 5, 2018</span></span>

<span data-ttu-id="5550f-2989">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5550f-2989">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5550f-2990">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-2990">Core</span></span>

* <span data-ttu-id="5550f-2991">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="5550f-2991">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5550f-2992">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-2992">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-2993">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-2993">ACR</span></span>

* <span data-ttu-id="5550f-2994">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="5550f-2994">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5550f-2995">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="5550f-2995">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5550f-2996">AKS</span><span class="sxs-lookup"><span data-stu-id="5550f-2996">AKS</span></span>

* <span data-ttu-id="5550f-2997">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="5550f-2997">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-2998">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-2998">Batch</span></span>

* <span data-ttu-id="5550f-2999">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5550f-2999">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3000">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3000">IOT</span></span>

* <span data-ttu-id="5550f-3001">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="5550f-3001">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3002">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3002">Network</span></span>

* <span data-ttu-id="5550f-3003">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3003">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5550f-3004">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5550f-3004">Policy Insights</span></span>

* <span data-ttu-id="5550f-3005">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3005">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5550f-3006">ARM</span><span class="sxs-lookup"><span data-stu-id="5550f-3006">ARM</span></span>

* <span data-ttu-id="5550f-3007">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3007">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3008">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3008">SQL</span></span>

* <span data-ttu-id="5550f-3009">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="5550f-3009">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5550f-3010">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="5550f-3010">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5550f-3011">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3011">Storage</span></span>

* <span data-ttu-id="5550f-3012">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3012">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3013">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3013">VM</span></span>

* <span data-ttu-id="5550f-3014">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3014">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5550f-3015">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3015">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5550f-3016">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3016">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5550f-3017">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3017">May 22, 2018</span></span>

<span data-ttu-id="5550f-3018">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5550f-3018">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3019">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3019">Core</span></span>

* <span data-ttu-id="5550f-3020">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3020">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3021">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3021">ACS</span></span>

* <span data-ttu-id="5550f-3022">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3022">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5550f-3023">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5550f-3023">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3024">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-3024">AppService</span></span>

* <span data-ttu-id="5550f-3025">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="5550f-3025">Improved generic update commands</span></span>
* <span data-ttu-id="5550f-3026">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3026">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3027">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3027">Container</span></span>

* <span data-ttu-id="5550f-3028">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="5550f-3028">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5550f-3029">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3029">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3030">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3030">Extension</span></span>

* <span data-ttu-id="5550f-3031">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3031">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3032">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3032">Interactive</span></span>

* <span data-ttu-id="5550f-3033">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3033">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5550f-3034">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3034">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-3035">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3035">KeyVault</span></span>

* <span data-ttu-id="5550f-3036">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="5550f-3036">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3037">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3037">Network</span></span>

* <span data-ttu-id="5550f-3038">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="5550f-3038">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5550f-3039">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="5550f-3039">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3040">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3040">SQL</span></span>

* <span data-ttu-id="5550f-3041">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="5550f-3041">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5550f-3042">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3042">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5550f-3043">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3043">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="5550f-3044">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="5550f-3044">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5550f-3045">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5550f-3045">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5550f-3046">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3046">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5550f-3047">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3047">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5550f-3048">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3048">`edition`.</span></span> <span data-ttu-id="5550f-3049">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3049">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5550f-3050">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3050">`elasticPoolName`.</span></span> <span data-ttu-id="5550f-3051">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3051">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5550f-3052">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5550f-3052">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5550f-3053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3053">`edition`.</span></span> <span data-ttu-id="5550f-3054">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3054">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5550f-3055">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3055">`dtu`.</span></span> <span data-ttu-id="5550f-3056">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3056">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5550f-3057">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3057">`databaseDtuMin`.</span></span> <span data-ttu-id="5550f-3058">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3058">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5550f-3059">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3059">`databaseDtuMax`.</span></span> <span data-ttu-id="5550f-3060">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3060">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5550f-3061">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3061">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5550f-3062">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3062">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3063">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3063">Storage</span></span>

* <span data-ttu-id="5550f-3064">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3064">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5550f-3065">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3065">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3066">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3066">VM</span></span>

* <span data-ttu-id="5550f-3067">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3067">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5550f-3068">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3068">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5550f-3069">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3069">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5550f-3070">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3070">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5550f-3071">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3071">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5550f-3072">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3072">May 7, 2018</span></span>

<span data-ttu-id="5550f-3073">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5550f-3073">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3074">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3074">Core</span></span>

* <span data-ttu-id="5550f-3075">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="5550f-3075">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5550f-3076">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3076">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5550f-3077">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3077">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5550f-3078">#5591</span><span class="sxs-lookup"><span data-stu-id="5550f-3078">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5550f-3079">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3079">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5550f-3080">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="5550f-3080">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5550f-3081">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="5550f-3081">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5550f-3082">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3082">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5550f-3083">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3083">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3084">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3084">ACR</span></span>

* <span data-ttu-id="5550f-3085">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-3085">Added ACR Build commands</span></span>
* <span data-ttu-id="5550f-3086">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5550f-3086">Improved resource not found error messages</span></span>
* <span data-ttu-id="5550f-3087">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5550f-3087">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5550f-3088">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="5550f-3088">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5550f-3089">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="5550f-3089">Improved repository commands error messages</span></span>
* <span data-ttu-id="5550f-3090">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3090">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3091">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3091">ACS</span></span>

* <span data-ttu-id="5550f-3092">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3092">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5550f-3093">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="5550f-3093">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5550f-3094">AMS</span><span class="sxs-lookup"><span data-stu-id="5550f-3094">AMS</span></span>

* <span data-ttu-id="5550f-3095">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-3095">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3096">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3096">Appservice</span></span>

* <span data-ttu-id="5550f-3097">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5550f-3097">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5550f-3098">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3098">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5550f-3099">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-3099">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5550f-3100">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3100">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5550f-3101">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-3101">Batch AI</span></span>

* <span data-ttu-id="5550f-3102">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-3102">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-3103">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-3103">Cognitive Services</span></span>

* <span data-ttu-id="5550f-3104">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="5550f-3104">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-3105">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-3105">Consumption</span></span>

* <span data-ttu-id="5550f-3106">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="5550f-3106">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3107">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3107">Container</span></span>

* <span data-ttu-id="5550f-3108">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-3108">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5550f-3109">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-3109">Cosmos DB</span></span>

* <span data-ttu-id="5550f-3110">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-3110">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5550f-3111">DMS</span><span class="sxs-lookup"><span data-stu-id="5550f-3111">DMS</span></span>

* <span data-ttu-id="5550f-3112">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-3112">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3113">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3113">Extension</span></span>

* <span data-ttu-id="5550f-3114">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="5550f-3114">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3115">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3115">Interactive</span></span>

* <span data-ttu-id="5550f-3116">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="5550f-3116">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5550f-3117">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="5550f-3117">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5550f-3118">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3118">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5550f-3119">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3119">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-3120">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-3120">Lab</span></span>

* <span data-ttu-id="5550f-3121">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="5550f-3121">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3122">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3122">Network</span></span>

* <span data-ttu-id="5550f-3123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="5550f-3123">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5550f-3124">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3124">Profile</span></span>

* <span data-ttu-id="5550f-3125">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3125">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5550f-3126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="5550f-3126">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5550f-3127">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3127">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-3128">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-3128">Redis</span></span>

* <span data-ttu-id="5550f-3129">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3129">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5550f-3130">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="5550f-3130">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5550f-3131">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3131">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5550f-3132">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3132">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5550f-3133">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3133">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5550f-3134">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3134">Role</span></span>

* <span data-ttu-id="5550f-3135">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3135">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3136">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3136">Storage</span></span>

* <span data-ttu-id="5550f-3137">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="5550f-3137">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5550f-3138">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3138">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5550f-3139">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="5550f-3139">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5550f-3140">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="5550f-3140">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5550f-3141">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="5550f-3141">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3142">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3142">VM</span></span>

* <span data-ttu-id="5550f-3143">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3143">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5550f-3144">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="5550f-3144">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5550f-3145">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3145">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5550f-3146">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3146">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5550f-3147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="5550f-3147">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5550f-3148">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="5550f-3148">Added write accelerator support</span></span>
* <span data-ttu-id="5550f-3149">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3149">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5550f-3150">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5550f-3150">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5550f-3151">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="5550f-3151">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5550f-3152">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3152">April 10, 2018</span></span>

<span data-ttu-id="5550f-3153">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5550f-3153">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3154">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3154">ACR</span></span>

* <span data-ttu-id="5550f-3155">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="5550f-3155">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3156">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3156">ACS</span></span>

* <span data-ttu-id="5550f-3157">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="5550f-3157">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3158">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3158">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5550f-3160">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3160">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-3161">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5550f-3161">BatchAI</span></span>

* <span data-ttu-id="5550f-3162">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-3162">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="5550f-3163">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3163">Job level mounting</span></span>
  - <span data-ttu-id="5550f-3164">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3164">Environment variables with secret values</span></span>
  - <span data-ttu-id="5550f-3165">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="5550f-3165">Performance counters settings</span></span>
  - <span data-ttu-id="5550f-3166">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3166">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="5550f-3167">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3167">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="5550f-3168">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="5550f-3168">Usage and limits reporting</span></span>
  - <span data-ttu-id="5550f-3169">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3169">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="5550f-3170">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3170">Support for custom images</span></span>
  - <span data-ttu-id="5550f-3171">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="5550f-3171">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5550f-3172">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3172">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5550f-3173">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3173">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5550f-3174">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="5550f-3174">National clouds are supported</span></span>
* <span data-ttu-id="5550f-3175">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5550f-3175">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5550f-3176">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="5550f-3176">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5550f-3177">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3177">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5550f-3178">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5550f-3178">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5550f-3179">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="5550f-3179">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5550f-3180">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="5550f-3180">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5550f-3181">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3181">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5550f-3182">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="5550f-3182">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5550f-3183">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="5550f-3183">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5550f-3184">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3184">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5550f-3185">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="5550f-3185">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5550f-3186">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3186">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5550f-3187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3187">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5550f-3188">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="5550f-3188">Billing</span></span>

* <span data-ttu-id="5550f-3189">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="5550f-3189">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-3190">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-3190">Consumption</span></span>

* <span data-ttu-id="5550f-3191">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3191">Added `marketplace` commands</span></span>
* <span data-ttu-id="5550f-3192">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3192">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5550f-3193">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3193">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5550f-3194">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3194">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5550f-3195">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3195">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5550f-3196">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3196">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3197">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3197">Container</span></span>

* <span data-ttu-id="5550f-3198">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3198">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5550f-3199">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="5550f-3199">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3200">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3200">Extension</span></span>

* <span data-ttu-id="5550f-3201">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3201">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3202">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3202">Interactive</span></span>

* <span data-ttu-id="5550f-3203">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="5550f-3203">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5550f-3204">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3204">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5550f-3205">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3205">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3206">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3206">Network</span></span>

* <span data-ttu-id="5550f-3207">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3207">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5550f-3208">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3208">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="5550f-3209">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="5550f-3209">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="5550f-3210">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3210">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="5550f-3211">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3211">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5550f-3212">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3212">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5550f-3213">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3213">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5550f-3214">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="5550f-3214">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3215">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3215">Profile</span></span>

* <span data-ttu-id="5550f-3216">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3216">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5550f-3217">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3217">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-3218">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-3218">RDBMS</span></span>

* <span data-ttu-id="5550f-3219">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3219">Added `georestore` command</span></span>
* <span data-ttu-id="5550f-3220">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-3220">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3221">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3221">Resource</span></span>

* <span data-ttu-id="5550f-3222">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3222">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5550f-3223">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3223">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3224">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3224">SQL</span></span>

* <span data-ttu-id="5550f-3225">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3225">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3226">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3226">Storage</span></span>

* <span data-ttu-id="5550f-3227">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="5550f-3227">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3228">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3228">VM</span></span>

* <span data-ttu-id="5550f-3229">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="5550f-3229">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5550f-3230">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3230">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="5550f-3232">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3232">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5550f-3233">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-3233">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="5550f-3234">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="5550f-3234">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="5550f-3235">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="5550f-3235">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5550f-3236">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3236">March 27, 2018</span></span>

<span data-ttu-id="5550f-3237">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5550f-3237">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3238">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3238">Core</span></span>

* <span data-ttu-id="5550f-3239">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5550f-3239">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3240">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3240">ACS</span></span>

* <span data-ttu-id="5550f-3241">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5550f-3241">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3242">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3242">Appservice</span></span>

* <span data-ttu-id="5550f-3243">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3243">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5550f-3244">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3244">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-3245">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-3245">Backup</span></span>

* <span data-ttu-id="5550f-3246">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3246">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5550f-3247">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="5550f-3247">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5550f-3248">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5550f-3248">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5550f-3249">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3249">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3250">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3250">Container</span></span>

* <span data-ttu-id="5550f-3251">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3251">Added `container exec` command.</span></span> <span data-ttu-id="5550f-3252">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3252">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5550f-3253">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3253">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3254">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3254">Extension</span></span>

* <span data-ttu-id="5550f-3255">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3255">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5550f-3256">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3256">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5550f-3257">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-3257">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3258">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3258">Interactive</span></span>

* <span data-ttu-id="5550f-3259">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3259">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5550f-3260">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3260">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5550f-3261">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3261">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5550f-3262">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3262">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-3263">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-3263">Lab</span></span>

* <span data-ttu-id="5550f-3264">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3264">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3265">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3265">Monitor</span></span>

* <span data-ttu-id="5550f-3266">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="5550f-3266">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5550f-3267">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3267">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5550f-3268">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="5550f-3268">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3269">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3269">Network</span></span>

* <span data-ttu-id="5550f-3270">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3270">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3271">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3271">Profile</span></span>

* <span data-ttu-id="5550f-3272">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3272">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-3273">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-3273">RDBMS</span></span>

* <span data-ttu-id="5550f-3274">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="5550f-3274">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3275">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3275">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5550f-3277">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3277">Role</span></span>

* <span data-ttu-id="5550f-3278">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3278">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5550f-3279">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3279">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5550f-3280">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="5550f-3280">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5550f-3281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3281">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5550f-3282">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3282">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3283">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3283">Storage</span></span>

* <span data-ttu-id="5550f-3284">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5550f-3284">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5550f-3285">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3285">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3286">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3286">VM</span></span>

* <span data-ttu-id="5550f-3287">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3287">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5550f-3288">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3288">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5550f-3289">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="5550f-3289">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5550f-3290">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="5550f-3290">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5550f-3291">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3291">March 13, 2018</span></span>

<span data-ttu-id="5550f-3292">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5550f-3292">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3293">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3293">ACR</span></span>

* <span data-ttu-id="5550f-3294">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3294">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5550f-3295">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-3295">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5550f-3296">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-3296">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3297">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3297">ACS</span></span>

* <span data-ttu-id="5550f-3298">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="5550f-3298">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5550f-3299">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3299">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5550f-3300">Помощник</span><span class="sxs-lookup"><span data-stu-id="5550f-3300">Advisor</span></span>

* <span data-ttu-id="5550f-3301">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3301">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5550f-3302">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3302">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5550f-3303">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3303">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="5550f-3304">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3304">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5550f-3305">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3305">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3306">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3306">Appservice</span></span>

* <span data-ttu-id="5550f-3307">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5550f-3307">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5550f-3308">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3308">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5550f-3309">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5550f-3309">Eventhubs</span></span>

* <span data-ttu-id="5550f-3310">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3310">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3311">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3311">Extension</span></span>

* <span data-ttu-id="5550f-3312">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="5550f-3312">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3313">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3313">Interactive</span></span>

* <span data-ttu-id="5550f-3314">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="5550f-3314">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5550f-3315">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="5550f-3315">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5550f-3316">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="5550f-3316">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5550f-3317">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3317">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3318">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3318">Monitor</span></span>

* <span data-ttu-id="5550f-3319">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-3319">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5550f-3320">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3320">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5550f-3321">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3321">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5550f-3322">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3322">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3323">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3323">Network</span></span>

* <span data-ttu-id="5550f-3324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3324">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5550f-3325">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5550f-3325">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5550f-3326">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3326">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5550f-3327">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3327">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3328">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3328">Profile</span></span>

* <span data-ttu-id="5550f-3329">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="5550f-3329">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5550f-3330">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3330">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-3331">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-3331">RDBMS</span></span>

* <span data-ttu-id="5550f-3332">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-3332">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5550f-3333">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5550f-3333">Service Bus</span></span>

* <span data-ttu-id="5550f-3334">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3334">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3335">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3335">Storage</span></span>

* <span data-ttu-id="5550f-3336">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="5550f-3336">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5550f-3337">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3337">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3338">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3338">VM</span></span>

* <span data-ttu-id="5550f-3339">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="5550f-3339">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5550f-3340">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5550f-3340">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5550f-3341">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3341">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5550f-3342">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="5550f-3342">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5550f-3343">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="5550f-3343">February 27, 2018</span></span>

<span data-ttu-id="5550f-3344">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5550f-3344">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3345">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3345">Core</span></span>

* <span data-ttu-id="5550f-3346">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="5550f-3346">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5550f-3347">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="5550f-3347">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5550f-3348">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3348">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3349">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3349">ACS</span></span>

* <span data-ttu-id="5550f-3350">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-3350">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5550f-3351">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3351">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5550f-3352">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3352">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5550f-3353">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3353">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3354">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3354">Appservice</span></span>

* <span data-ttu-id="5550f-3355">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5550f-3355">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5550f-3356">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="5550f-3356">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5550f-3357">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5550f-3357">Cognitive Services</span></span>

* <span data-ttu-id="5550f-3358">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5550f-3358">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-3359">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-3359">Consumption</span></span>

* <span data-ttu-id="5550f-3360">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3360">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5550f-3361">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="5550f-3361">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3362">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3362">Container</span></span>

* <span data-ttu-id="5550f-3363">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3363">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3364">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3364">Network</span></span>

* <span data-ttu-id="5550f-3365">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3365">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3366">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3366">Resource</span></span>

* <span data-ttu-id="5550f-3367">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="5550f-3367">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5550f-3368">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3368">Role</span></span>

* <span data-ttu-id="5550f-3369">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3369">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3370">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3370">SQL</span></span>

* <span data-ttu-id="5550f-3371">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3371">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3372">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3372">Storage</span></span>

* <span data-ttu-id="5550f-3373">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3373">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3374">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3374">VM</span></span>

* <span data-ttu-id="5550f-3375">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3375">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5550f-3376">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3376">February 13, 2018</span></span>

<span data-ttu-id="5550f-3377">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5550f-3377">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3378">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3378">Core</span></span>

* <span data-ttu-id="5550f-3379">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="5550f-3379">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3380">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3380">ACS</span></span>

* <span data-ttu-id="5550f-3381">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="5550f-3381">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5550f-3382">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3382">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5550f-3383">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-3383">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5550f-3384">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3384">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5550f-3385">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="5550f-3385">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5550f-3386">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3386">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5550f-3387">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-3387">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5550f-3388">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3388">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3389">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3389">Appservice</span></span>

* <span data-ttu-id="5550f-3390">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3390">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5550f-3391">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3391">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-3392">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-3392">CDN</span></span>

* <span data-ttu-id="5550f-3393">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3393">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3394">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3394">Container</span></span>

* <span data-ttu-id="5550f-3395">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="5550f-3395">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5550f-3396">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3396">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-3397">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-3397">CosmosDB</span></span>

* <span data-ttu-id="5550f-3398">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3398">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3399">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3399">Extension</span></span>

* <span data-ttu-id="5550f-3400">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3400">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5550f-3401">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3401">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5550f-3402">Отзывы</span><span class="sxs-lookup"><span data-stu-id="5550f-3402">Feedback</span></span>

* <span data-ttu-id="5550f-3403">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3403">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3404">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3404">Interactive</span></span>

* <span data-ttu-id="5550f-3405">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5550f-3405">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5550f-3406">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3406">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3407">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3407">IoT</span></span>

* <span data-ttu-id="5550f-3408">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5550f-3408">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5550f-3409">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5550f-3409">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5550f-3410">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3410">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5550f-3411">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3411">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3412">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3412">Monitor</span></span>

* <span data-ttu-id="5550f-3413">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3413">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3414">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3414">Network</span></span>

* <span data-ttu-id="5550f-3415">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5550f-3415">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5550f-3416">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3416">Profile</span></span>

* <span data-ttu-id="5550f-3417">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5550f-3417">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3418">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3418">Resource</span></span>

* <span data-ttu-id="5550f-3419">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3419">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5550f-3420">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3420">Role</span></span>

* <span data-ttu-id="5550f-3421">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="5550f-3421">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3422">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3422">SQL</span></span>

* <span data-ttu-id="5550f-3423">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3423">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5550f-3424">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3424">Added `sql db rename`</span></span>
* <span data-ttu-id="5550f-3425">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-3425">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3426">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3426">Storage</span></span>

* <span data-ttu-id="5550f-3427">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="5550f-3427">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3428">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3428">VM</span></span>

* <span data-ttu-id="5550f-3429">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="5550f-3429">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5550f-3430">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3430">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5550f-3431">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="5550f-3431">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5550f-3432">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3432">January 31, 2018</span></span>

<span data-ttu-id="5550f-3433">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5550f-3433">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3434">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3434">Core</span></span>

* <span data-ttu-id="5550f-3435">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="5550f-3435">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5550f-3436">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-3436">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5550f-3437">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="5550f-3437">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5550f-3438">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="5550f-3438">Use `--verbose` to see</span></span>
* <span data-ttu-id="5550f-3439">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3439">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3440">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3440">ACS</span></span>

* <span data-ttu-id="5550f-3441">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3441">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5550f-3442">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3442">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3443">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3443">Appservice</span></span>

* <span data-ttu-id="5550f-3444">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3444">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5550f-3445">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="5550f-3445">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-3446">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-3446">CDN</span></span>

* <span data-ttu-id="5550f-3447">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3447">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-3448">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-3448">CosmosDB</span></span>

* <span data-ttu-id="5550f-3449">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="5550f-3449">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3450">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3450">Interactive</span></span>

* <span data-ttu-id="5550f-3451">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="5550f-3451">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3452">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3452">Network</span></span>

* <span data-ttu-id="5550f-3453">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3453">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5550f-3454">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-3454">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5550f-3455">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3455">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5550f-3456">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3456">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5550f-3457">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3457">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5550f-3458">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="5550f-3458">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5550f-3459">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="5550f-3459">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5550f-3460">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="5550f-3460">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5550f-3461">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3461">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="5550f-3462">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3462">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3463">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3463">Profile</span></span>

* <span data-ttu-id="5550f-3464">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="5550f-3464">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3465">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3465">Resource</span></span>

* <span data-ttu-id="5550f-3466">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="5550f-3466">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3467">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3467">Storage</span></span>

* <span data-ttu-id="5550f-3468">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-3468">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5550f-3469">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3469">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5550f-3470">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3470">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="5550f-3471">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3471">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5550f-3472">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="5550f-3472">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3473">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3473">VM</span></span>

* <span data-ttu-id="5550f-3474">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="5550f-3474">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5550f-3475">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3475">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5550f-3476">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3476">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5550f-3477">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3477">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5550f-3478">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3478">January 17, 2018</span></span>

<span data-ttu-id="5550f-3479">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5550f-3479">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3480">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3480">ACR</span></span>

* <span data-ttu-id="5550f-3481">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-3481">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5550f-3482">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="5550f-3482">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3483">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3483">ACS</span></span>

* <span data-ttu-id="5550f-3484">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3484">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5550f-3485">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3485">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3486">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3486">Appservice</span></span>

* <span data-ttu-id="5550f-3487">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="5550f-3487">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5550f-3488">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3488">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5550f-3489">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3489">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-3490">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-3490">Backup</span></span>

* <span data-ttu-id="5550f-3491">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-3491">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5550f-3492">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3492">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5550f-3493">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="5550f-3493">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5550f-3494">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="5550f-3494">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5550f-3495">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="5550f-3495">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-3496">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3496">Batch</span></span>

* <span data-ttu-id="5550f-3497">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5550f-3497">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-3498">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-3498">Cloud</span></span>

* <span data-ttu-id="5550f-3499">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3499">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-3500">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-3500">Consumption</span></span>

* <span data-ttu-id="5550f-3501">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3501">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5550f-3502">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3502">Event Grid</span></span>

* <span data-ttu-id="5550f-3503">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3503">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5550f-3504">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3504">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5550f-3505">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3505">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5550f-3506">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3506">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5550f-3507">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3507">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5550f-3508">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3508">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5550f-3509">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3509">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5550f-3510">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3510">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3511">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3511">Interactive</span></span>

* <span data-ttu-id="5550f-3512">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="5550f-3512">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5550f-3513">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="5550f-3513">Fixed errors on startup</span></span>
* <span data-ttu-id="5550f-3514">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5550f-3514">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3515">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3515">IoT</span></span>

* <span data-ttu-id="5550f-3516">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="5550f-3516">Added support for device provisioning service</span></span>
* <span data-ttu-id="5550f-3517">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="5550f-3517">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5550f-3518">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5550f-3518">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3519">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3519">Monitor</span></span>

* <span data-ttu-id="5550f-3520">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3520">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5550f-3521">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3521">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5550f-3522">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="5550f-3522">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3523">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3523">Network</span></span>

* <span data-ttu-id="5550f-3524">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="5550f-3524">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5550f-3525">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="5550f-3525">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3526">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3526">Profile</span></span>

* <span data-ttu-id="5550f-3527">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3527">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5550f-3528">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3528">Role</span></span>

* <span data-ttu-id="5550f-3529">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3529">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-3530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-3530">Service Fabric</span></span>

* <span data-ttu-id="5550f-3531">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5550f-3531">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5550f-3532">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3532">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3533">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3533">VM</span></span>

* <span data-ttu-id="5550f-3534">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3534">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5550f-3535">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="5550f-3535">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5550f-3536">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3536">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5550f-3537">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="5550f-3537">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5550f-3538">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="5550f-3538">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5550f-3539">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3539">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5550f-3540">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3540">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5550f-3541">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3541">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5550f-3542">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3542">December 19, 2017</span></span>

<span data-ttu-id="5550f-3543">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5550f-3543">Version 2.0.23</span></span>

* <span data-ttu-id="5550f-3544">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3544">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3545">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3545">Container</span></span>

* <span data-ttu-id="5550f-3546">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3546">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3547">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3547">Network</span></span>

* <span data-ttu-id="5550f-3548">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3548">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5550f-3549">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3549">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3550">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3550">Storage</span></span>

* <span data-ttu-id="5550f-3551">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="5550f-3551">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3552">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3552">VM</span></span>

* <span data-ttu-id="5550f-3553">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3553">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5550f-3554">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3554">December 5, 2017</span></span>

<span data-ttu-id="5550f-3555">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5550f-3555">Version 2.0.22</span></span>

* <span data-ttu-id="5550f-3556">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3556">Removed `az component` commands.</span></span> <span data-ttu-id="5550f-3557">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3557">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3558">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3558">Core</span></span>
* <span data-ttu-id="5550f-3559">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="5550f-3559">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5550f-3560">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3560">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3561">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3561">ACS</span></span>

* <span data-ttu-id="5550f-3562">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3562">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5550f-3563">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3563">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5550f-3564">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="5550f-3564">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5550f-3565">Помощник</span><span class="sxs-lookup"><span data-stu-id="5550f-3565">Advisor</span></span>

* <span data-ttu-id="5550f-3566">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3566">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3567">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3567">Appservice</span></span>

* <span data-ttu-id="5550f-3568">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3568">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5550f-3569">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3569">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5550f-3570">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3570">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5550f-3571">Потребление</span><span class="sxs-lookup"><span data-stu-id="5550f-3571">Consumption</span></span>

* <span data-ttu-id="5550f-3572">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="5550f-3572">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3573">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3573">Container</span></span>

* <span data-ttu-id="5550f-3574">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3574">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3575">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3575">Monitor</span></span>

* <span data-ttu-id="5550f-3576">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="5550f-3576">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3577">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3577">Resource</span></span>

* <span data-ttu-id="5550f-3578">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="5550f-3578">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5550f-3579">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-3579">Role</span></span>

* <span data-ttu-id="5550f-3580">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3580">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5550f-3581">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="5550f-3581">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5550f-3582">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3582">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3583">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3583">SQL</span></span>

* <span data-ttu-id="5550f-3584">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3584">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5550f-3585">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3585">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3586">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3586">VM</span></span>

* <span data-ttu-id="5550f-3587">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3587">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5550f-3588">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3588">November 14, 2017</span></span>

<span data-ttu-id="5550f-3589">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5550f-3589">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3590">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3590">ACR</span></span>

* <span data-ttu-id="5550f-3591">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="5550f-3591">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5550f-3592">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3592">ACS</span></span>

* <span data-ttu-id="5550f-3593">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="5550f-3593">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5550f-3594">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="5550f-3594">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5550f-3595">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3595">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5550f-3596">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-3596">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5550f-3597">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-3597">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3598">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3598">Appservice</span></span>

* <span data-ttu-id="5550f-3599">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3599">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5550f-3600">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3600">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5550f-3601">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3601">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5550f-3602">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3602">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5550f-3603">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="5550f-3603">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5550f-3604">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="5550f-3604">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-3605">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3605">Batch</span></span>

* <span data-ttu-id="5550f-3606">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3606">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-3607">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5550f-3607">Batchai</span></span>

* <span data-ttu-id="5550f-3608">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3608">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5550f-3609">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3609">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5550f-3610">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3610">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5550f-3611">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3611">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-3612">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-3612">Cloud</span></span>

* <span data-ttu-id="5550f-3613">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3613">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3614">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3614">Container</span></span>

* <span data-ttu-id="5550f-3615">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3615">Added support to open multiple ports</span></span>
* <span data-ttu-id="5550f-3616">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3616">Added container group restart policy</span></span>
* <span data-ttu-id="5550f-3617">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="5550f-3617">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5550f-3618">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="5550f-3618">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5550f-3619">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5550f-3619">Data Lake Analytics</span></span>

* <span data-ttu-id="5550f-3620">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3620">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5550f-3621">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5550f-3621">Data Lake Store</span></span>

* <span data-ttu-id="5550f-3622">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3622">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3623">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3623">Extension</span></span>

* <span data-ttu-id="5550f-3624">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5550f-3624">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5550f-3625">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="5550f-3625">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3626">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3626">IoT</span></span>

* <span data-ttu-id="5550f-3627">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3627">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3628">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3628">Monitor</span></span>

* <span data-ttu-id="5550f-3629">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3629">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3630">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3630">Network</span></span>

* <span data-ttu-id="5550f-3631">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="5550f-3631">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5550f-3632">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3632">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5550f-3633">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5550f-3633">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5550f-3634">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3634">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5550f-3635">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5550f-3635">Reservations</span></span>

* <span data-ttu-id="5550f-3636">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="5550f-3636">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3637">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3637">Resource</span></span>

* <span data-ttu-id="5550f-3638">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3638">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3639">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3639">SQL</span></span>

* <span data-ttu-id="5550f-3640">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3640">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3641">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3641">Storage</span></span>

* <span data-ttu-id="5550f-3642">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-3642">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5550f-3643">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="5550f-3643">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5550f-3644">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3644">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5550f-3645">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3645">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5550f-3646">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3646">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5550f-3647">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3647">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5550f-3648">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3648">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3649">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3649">VM</span></span>

* <span data-ttu-id="5550f-3650">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3650">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5550f-3651">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3651">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5550f-3652">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3652">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5550f-3653">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="5550f-3653">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5550f-3654">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5550f-3654">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5550f-3655">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3655">October 24, 2017</span></span>

<span data-ttu-id="5550f-3656">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5550f-3656">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3657">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3657">Core</span></span>

* <span data-ttu-id="5550f-3658">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="5550f-3658">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3659">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3659">ACR</span></span>

* <span data-ttu-id="5550f-3660">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="5550f-3660">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5550f-3661">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="5550f-3661">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5550f-3662">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="5550f-3662">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3663">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3663">ACS</span></span>

* <span data-ttu-id="5550f-3664">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="5550f-3664">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5550f-3665">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="5550f-3665">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3666">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3666">Appservice</span></span>

* <span data-ttu-id="5550f-3667">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="5550f-3667">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5550f-3668">Компонент</span><span class="sxs-lookup"><span data-stu-id="5550f-3668">Component</span></span>

* <span data-ttu-id="5550f-3669">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="5550f-3669">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3670">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3670">Monitor</span></span>

* <span data-ttu-id="5550f-3671">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3671">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3672">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3672">Resource</span></span>

* <span data-ttu-id="5550f-3673">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="5550f-3673">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5550f-3674">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="5550f-3674">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3675">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3675">VM</span></span>

* <span data-ttu-id="5550f-3676">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5550f-3676">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5550f-3677">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3677">October 9, 2017</span></span>

<span data-ttu-id="5550f-3678">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5550f-3678">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3679">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3679">Core</span></span>

* <span data-ttu-id="5550f-3680">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="5550f-3680">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3681">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3681">Appservice</span></span>

* <span data-ttu-id="5550f-3682">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3682">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-3683">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3683">Batch</span></span>

* <span data-ttu-id="5550f-3684">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5550f-3684">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5550f-3685">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="5550f-3685">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5550f-3686">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3686">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5550f-3687">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3687">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5550f-3688">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5550f-3688">Batchai</span></span>

* <span data-ttu-id="5550f-3689">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5550f-3689">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-3690">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3690">Keyvault</span></span>

* <span data-ttu-id="5550f-3691">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5550f-3691">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5550f-3692">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5550f-3692">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5550f-3693">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3693">Network</span></span>

* <span data-ttu-id="5550f-3694">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="5550f-3694">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5550f-3695">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="5550f-3695">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3696">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3696">Resource</span></span>

* <span data-ttu-id="5550f-3697">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3697">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5550f-3698">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3698">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5550f-3699">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3699">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5550f-3700">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="5550f-3700">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3701">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3701">Sql</span></span>

* <span data-ttu-id="5550f-3702">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="5550f-3702">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5550f-3703">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-3703">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5550f-3704">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-3704">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3705">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3705">Storage</span></span>

* <span data-ttu-id="5550f-3706">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3706">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3707">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="5550f-3707">Vm</span></span>

* <span data-ttu-id="5550f-3708">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3708">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5550f-3709">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3709">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5550f-3710">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3710">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5550f-3711">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3711">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5550f-3712">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="5550f-3712">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5550f-3713">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3713">September 22, 2017</span></span>

<span data-ttu-id="5550f-3714">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5550f-3714">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3715">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3715">Resource</span></span>

* <span data-ttu-id="5550f-3716">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="5550f-3716">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5550f-3717">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="5550f-3717">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5550f-3718">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5550f-3718">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5550f-3719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3719">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3720">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3720">Network</span></span>

* <span data-ttu-id="5550f-3721">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5550f-3721">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5550f-3722">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="5550f-3722">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5550f-3723">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="5550f-3723">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5550f-3724">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3724">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5550f-3725">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3725">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5550f-3726">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3726">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5550f-3727">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3727">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3728">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3728">Storage</span></span>

* <span data-ttu-id="5550f-3729">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="5550f-3729">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5550f-3730">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5550f-3730">Eventgrid</span></span>

* <span data-ttu-id="5550f-3731">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="5550f-3731">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3732">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3732">SQL</span></span>

* <span data-ttu-id="5550f-3733">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-3733">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5550f-3734">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="5550f-3734">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5550f-3735">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3735">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-3736">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3736">Keyvault</span></span>

* <span data-ttu-id="5550f-3737">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="5550f-3737">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3738">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3738">VM</span></span>

* <span data-ttu-id="5550f-3739">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5550f-3739">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5550f-3740">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="5550f-3740">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5550f-3741">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="5550f-3741">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5550f-3742">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5550f-3742">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5550f-3743">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5550f-3743">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5550f-3744">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5550f-3744">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3745">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3745">ACS</span></span>

* <span data-ttu-id="5550f-3746">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5550f-3746">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3747">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3747">Appservice</span></span>

* <span data-ttu-id="5550f-3748">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5550f-3748">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5550f-3749">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="5550f-3749">Backup</span></span>

* <span data-ttu-id="5550f-3750">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5550f-3750">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5550f-3751">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3751">September 11, 2017</span></span>

<span data-ttu-id="5550f-3752">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5550f-3752">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5550f-3753">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3753">Core</span></span>

* <span data-ttu-id="5550f-3754">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5550f-3754">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5550f-3755">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="5550f-3755">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3756">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3756">Acs</span></span>

* <span data-ttu-id="5550f-3757">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3757">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5550f-3758">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-3758">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3759">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3759">Appservice</span></span>

* <span data-ttu-id="5550f-3760">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="5550f-3760">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-3761">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-3761">CDN</span></span>

* <span data-ttu-id="5550f-3762">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3762">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5550f-3763">Расширение</span><span class="sxs-lookup"><span data-stu-id="5550f-3763">Extension</span></span>

* <span data-ttu-id="5550f-3764">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3764">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-3765">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3765">Keyvault</span></span>

* <span data-ttu-id="5550f-3766">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3766">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3767">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3767">Network</span></span>

* <span data-ttu-id="5550f-3768">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5550f-3768">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5550f-3769">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3769">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5550f-3770">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3770">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5550f-3771">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3771">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5550f-3772">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3772">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-3773">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-3773">Resource</span></span>

* <span data-ttu-id="5550f-3774">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3774">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5550f-3775">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3775">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5550f-3776">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3776">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5550f-3777">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="5550f-3777">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-3778">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-3778">SQL</span></span>

* <span data-ttu-id="5550f-3779">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3779">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3780">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3780">VM</span></span>

* <span data-ttu-id="5550f-3781">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5550f-3781">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5550f-3782">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="5550f-3782">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5550f-3783">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3783">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5550f-3784">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="5550f-3784">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5550f-3785">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="5550f-3785">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5550f-3786">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3786">August 31, 2017</span></span>

<span data-ttu-id="5550f-3787">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5550f-3787">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-3788">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3788">Keyvault</span></span>

* <span data-ttu-id="5550f-3789">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3789">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5550f-3790">Sf</span><span class="sxs-lookup"><span data-stu-id="5550f-3790">Sf</span></span>

* <span data-ttu-id="5550f-3791">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="5550f-3791">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3792">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3792">Storage</span></span>

* <span data-ttu-id="5550f-3793">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="5550f-3793">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5550f-3794">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="5550f-3794">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5550f-3795">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3795">August 28, 2017</span></span>

<span data-ttu-id="5550f-3796">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5550f-3796">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5550f-3797">CLI</span><span class="sxs-lookup"><span data-stu-id="5550f-3797">CLI</span></span>

* <span data-ttu-id="5550f-3798">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="5550f-3798">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3799">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3799">ACS</span></span>

* <span data-ttu-id="5550f-3800">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5550f-3800">Corrected preview regions</span></span>
* <span data-ttu-id="5550f-3801">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3801">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5550f-3802">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3802">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3803">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3803">Appservice</span></span>

* <span data-ttu-id="5550f-3804">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3804">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5550f-3805">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3805">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5550f-3806">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3806">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5550f-3807">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="5550f-3807">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5550f-3808">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="5550f-3808">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3809">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3809">IoT</span></span>

* <span data-ttu-id="5550f-3810">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="5550f-3810">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3811">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3811">Network</span></span>

* <span data-ttu-id="5550f-3812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3812">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5550f-3813">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3813">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5550f-3814">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3814">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5550f-3815">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3815">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5550f-3816">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3816">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3817">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3817">Profile</span></span>

* <span data-ttu-id="5550f-3818">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5550f-3818">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-3819">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-3819">Service Fabric</span></span>

* <span data-ttu-id="5550f-3820">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5550f-3820">Preview release</span></span>
* <span data-ttu-id="5550f-3821">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-3821">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5550f-3822">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="5550f-3822">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5550f-3823">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3823">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3824">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3824">Storage</span></span>

* <span data-ttu-id="5550f-3825">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5550f-3825">Enabled setting blob tier</span></span>
* <span data-ttu-id="5550f-3826">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-3826">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5550f-3827">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3827">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5550f-3828">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="5550f-3828">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5550f-3829">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3829">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5550f-3830">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3830">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3831">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3831">VM</span></span>

* <span data-ttu-id="5550f-3832">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3832">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5550f-3833">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3833">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5550f-3834">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="5550f-3834">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5550f-3835">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="5550f-3835">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5550f-3836">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5550f-3836">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5550f-3837">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3837">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5550f-3838">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3838">August 15, 2017</span></span>

<span data-ttu-id="5550f-3839">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5550f-3839">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3840">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3840">ACS</span></span>

* <span data-ttu-id="5550f-3841">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5550f-3841">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3842">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3842">Appservice</span></span>

* <span data-ttu-id="5550f-3843">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="5550f-3843">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5550f-3844">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3844">Event Grid</span></span>

* <span data-ttu-id="5550f-3845">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5550f-3845">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5550f-3846">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3846">August 11, 2017</span></span>

<span data-ttu-id="5550f-3847">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5550f-3847">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3848">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3848">ACS</span></span>

* <span data-ttu-id="5550f-3849">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5550f-3849">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-3850">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3850">Batch</span></span>

* <span data-ttu-id="5550f-3851">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="5550f-3851">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5550f-3852">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="5550f-3852">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5550f-3853">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3853">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5550f-3854">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="5550f-3854">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5550f-3855">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="5550f-3855">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5550f-3856">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="5550f-3856">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5550f-3857">Компонент</span><span class="sxs-lookup"><span data-stu-id="5550f-3857">Component</span></span>

* <span data-ttu-id="5550f-3858">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="5550f-3858">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5550f-3859">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5550f-3859">Container</span></span>

* <span data-ttu-id="5550f-3860">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="5550f-3860">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5550f-3861">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5550f-3861">Data Lake Store</span></span>

* <span data-ttu-id="5550f-3862">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="5550f-3862">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5550f-3863">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3863">Event Grid</span></span>

* <span data-ttu-id="5550f-3864">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="5550f-3864">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3865">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3865">Network</span></span>

* <span data-ttu-id="5550f-3866">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="5550f-3866">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5550f-3867">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3867">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5550f-3868">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3868">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5550f-3869">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3869">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-3870">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-3870">Profile</span></span>

* <span data-ttu-id="5550f-3871">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="5550f-3871">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-3872">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-3872">Storage</span></span>

* <span data-ttu-id="5550f-3873">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5550f-3873">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-3874">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-3874">VM</span></span>

* <span data-ttu-id="5550f-3875">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="5550f-3875">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5550f-3876">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3876">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5550f-3877">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="5550f-3877">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5550f-3878">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="5550f-3878">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5550f-3879">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5550f-3879">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5550f-3880">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-3880">July 28, 2017</span></span>

<span data-ttu-id="5550f-3881">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5550f-3881">Version 2.0.12</span></span>

* <span data-ttu-id="5550f-3882">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3882">Added container commands</span></span>
* <span data-ttu-id="5550f-3883">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3883">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5550f-3884">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-3884">Core</span></span>

* <span data-ttu-id="5550f-3885">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5550f-3885">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5550f-3886">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="5550f-3886">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5550f-3887">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5550f-3887">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5550f-3888">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="5550f-3888">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5550f-3889">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="5550f-3889">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5550f-3890">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="5550f-3890">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5550f-3891">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5550f-3891">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5550f-3892">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="5550f-3892">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5550f-3893">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="5550f-3893">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5550f-3894">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="5550f-3894">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5550f-3895">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="5550f-3895">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5550f-3896">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="5550f-3896">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5550f-3897">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-3897">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5550f-3898">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5550f-3898">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5550f-3899">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5550f-3899">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5550f-3900">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="5550f-3900">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5550f-3901">ACR</span><span class="sxs-lookup"><span data-stu-id="5550f-3901">ACR</span></span>

* <span data-ttu-id="5550f-3902">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3902">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5550f-3903">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5550f-3903">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5550f-3904">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="5550f-3904">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5550f-3905">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="5550f-3905">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5550f-3906">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="5550f-3906">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5550f-3907">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="5550f-3907">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-3908">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-3908">ACS</span></span>

* <span data-ttu-id="5550f-3909">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="5550f-3909">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-3910">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5550f-3910">Appservice</span></span>

* <span data-ttu-id="5550f-3911">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="5550f-3911">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5550f-3912">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="5550f-3912">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5550f-3913">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3913">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5550f-3914">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="5550f-3914">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5550f-3915">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="5550f-3915">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5550f-3916">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="5550f-3916">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5550f-3917">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="5550f-3917">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5550f-3918">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="5550f-3918">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5550f-3919">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-3919">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5550f-3920">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3920">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5550f-3921">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5550f-3921">Batch</span></span>

* <span data-ttu-id="5550f-3922">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="5550f-3922">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5550f-3923">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3923">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5550f-3924">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3924">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5550f-3925">CDN</span><span class="sxs-lookup"><span data-stu-id="5550f-3925">CDN</span></span>

* <span data-ttu-id="5550f-3926">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-3926">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5550f-3927">Cloud</span><span class="sxs-lookup"><span data-stu-id="5550f-3927">Cloud</span></span>

* <span data-ttu-id="5550f-3928">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5550f-3928">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5550f-3929">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="5550f-3929">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5550f-3930">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="5550f-3930">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5550f-3931">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5550f-3931">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5550f-3932">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3932">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-3933">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-3933">CosmosDB</span></span>

* <span data-ttu-id="5550f-3934">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="5550f-3934">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5550f-3935">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="5550f-3935">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5550f-3936">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5550f-3936">Data Lake Analytics</span></span>

* <span data-ttu-id="5550f-3937">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3937">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5550f-3938">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3938">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5550f-3939">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3939">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5550f-3940">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5550f-3940">Data Lake Store</span></span>

* <span data-ttu-id="5550f-3941">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3941">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5550f-3942">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="5550f-3942">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5550f-3943">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3943">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5550f-3944">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5550f-3944">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5550f-3945">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="5550f-3945">Interactive</span></span>

* <span data-ttu-id="5550f-3946">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="5550f-3946">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5550f-3947">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="5550f-3947">Increased test coverage</span></span>
* <span data-ttu-id="5550f-3948">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="5550f-3948">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5550f-3949">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="5550f-3949">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5550f-3950">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="5550f-3950">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5550f-3951">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="5550f-3951">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5550f-3952">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5550f-3952">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5550f-3953">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3953">Added `--progress` flag</span></span>
* <span data-ttu-id="5550f-3954">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3954">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5550f-3955">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="5550f-3955">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5550f-3956">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5550f-3956">IoT</span></span>

* <span data-ttu-id="5550f-3957">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="5550f-3957">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5550f-3958">(3934).</span><span class="sxs-lookup"><span data-stu-id="5550f-3958">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5550f-3959">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-3959">Key vault</span></span>

* <span data-ttu-id="5550f-3960">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="5550f-3960">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5550f-3961">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3961">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5550f-3962">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="5550f-3962">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5550f-3963">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3963">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5550f-3964">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3964">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5550f-3965">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="5550f-3965">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5550f-3966">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="5550f-3966">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5550f-3967">(3307).</span><span class="sxs-lookup"><span data-stu-id="5550f-3967">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-3968">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-3968">Lab</span></span>

* <span data-ttu-id="5550f-3969">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3969">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5550f-3970">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3970">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-3971">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-3971">Monitor</span></span>

* <span data-ttu-id="5550f-3972">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="5550f-3972">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5550f-3973">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="5550f-3973">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5550f-3974">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="5550f-3974">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5550f-3975">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="5550f-3975">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5550f-3976">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="5550f-3976">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5550f-3977">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="5550f-3977">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5550f-3978">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="5550f-3978">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5550f-3979">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="5550f-3979">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5550f-3980">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5550f-3980">`location` no longer required</span></span>
  * <span data-ttu-id="5550f-3981">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="5550f-3981">Add name and ID support for target</span></span>
  * <span data-ttu-id="5550f-3982">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="5550f-3982">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5550f-3983">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5550f-3983">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5550f-3984">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="5550f-3984">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5550f-3985">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="5550f-3985">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5550f-3986">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3986">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5550f-3987">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3987">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5550f-3988">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-3988">Network</span></span>

* <span data-ttu-id="5550f-3989">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3989">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5550f-3990">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3990">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5550f-3991">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5550f-3991">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5550f-3992">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3992">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5550f-3993">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3993">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5550f-3994">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3994">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5550f-3995">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3995">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5550f-3996">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3996">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5550f-3997">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3997">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5550f-3998">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3998">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5550f-3999">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-3999">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5550f-4000">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4000">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5550f-4001">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4001">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5550f-4002">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4002">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5550f-4003">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4003">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5550f-4004">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4004">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5550f-4005">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="5550f-4005">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5550f-4006">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4006">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5550f-4007">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4007">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5550f-4008">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4008">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5550f-4009">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4009">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5550f-4010">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4010">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5550f-4011">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4011">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5550f-4012">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-4012">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5550f-4013">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-4013">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5550f-4014">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5550f-4014">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5550f-4015">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-4015">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-4016">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-4016">Profile</span></span>

* <span data-ttu-id="5550f-4017">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5550f-4017">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5550f-4018">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5550f-4018">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5550f-4019">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5550f-4019">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5550f-4020">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="5550f-4020">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5550f-4021">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="5550f-4021">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5550f-4022">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5550f-4022">RDBMS</span></span>

* <span data-ttu-id="5550f-4023">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="5550f-4023">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5550f-4024">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="5550f-4024">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5550f-4025">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="5550f-4025">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5550f-4026">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="5550f-4026">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-4027">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-4027">Resource</span></span>

* <span data-ttu-id="5550f-4028">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4028">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5550f-4029">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4029">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5550f-4030">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4030">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5550f-4031">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4031">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5550f-4032">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="5550f-4032">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5550f-4033">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4033">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5550f-4034">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="5550f-4034">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5550f-4035">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4035">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5550f-4036">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-4036">Role</span></span>

* <span data-ttu-id="5550f-4037">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5550f-4037">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5550f-4038">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="5550f-4038">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5550f-4039">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="5550f-4039">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5550f-4040">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5550f-4040">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5550f-4041">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4041">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5550f-4042">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5550f-4042">Service Fabric</span></span>
* <span data-ttu-id="5550f-4043">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="5550f-4043">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5550f-4044">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="5550f-4044">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5550f-4045">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="5550f-4045">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-4046">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-4046">SQL</span></span>

* <span data-ttu-id="5550f-4047">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4047">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5550f-4048">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4048">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5550f-4049">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4049">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-4050">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-4050">Storage</span></span>

* <span data-ttu-id="5550f-4051">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="5550f-4051">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5550f-4052">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5550f-4052">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5550f-4053">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="5550f-4053">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5550f-4054">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="5550f-4054">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5550f-4055">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="5550f-4055">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5550f-4056">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="5550f-4056">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-4057">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-4057">VM</span></span>

* <span data-ttu-id="5550f-4058">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="5550f-4058">Support configuring nsg</span></span>
* <span data-ttu-id="5550f-4059">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="5550f-4059">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5550f-4060">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-4060">Support managed service identities</span></span>
* <span data-ttu-id="5550f-4061">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4061">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5550f-4062">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="5550f-4062">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5550f-4063">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-4063">May 10, 2017</span></span>

<span data-ttu-id="5550f-4064">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5550f-4064">Version 2.0.6</span></span>

* <span data-ttu-id="5550f-4065">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5550f-4065">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5550f-4066">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="5550f-4066">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5550f-4067">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-4067">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5550f-4068">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5550f-4068">Include Cognitive Services module</span></span>
* <span data-ttu-id="5550f-4069">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="5550f-4069">Include Service Fabric module</span></span>
* <span data-ttu-id="5550f-4070">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="5550f-4070">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5550f-4071">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="5550f-4071">Add support for CDN commands</span></span>
* <span data-ttu-id="5550f-4072">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="5550f-4072">Remove Container module</span></span>
* <span data-ttu-id="5550f-4073">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4073">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5550f-4074">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4074">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5550f-4075">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-4075">Core</span></span>

* <span data-ttu-id="5550f-4076">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="5550f-4076">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5550f-4077">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4077">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5550f-4078">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4078">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5550f-4079">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4079">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5550f-4080">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4080">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5550f-4081">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4081">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5550f-4082">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4082">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5550f-4083">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4083">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5550f-4084">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4084">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5550f-4085">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="5550f-4085">core: Improved performance</span></span>
* <span data-ttu-id="5550f-4086">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="5550f-4086">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5550f-4087">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="5550f-4087">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-4088">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-4088">ACS</span></span>

* <span data-ttu-id="5550f-4089">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="5550f-4089">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5550f-4090">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="5550f-4090">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5550f-4091">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="5550f-4091">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5550f-4092">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4092">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-4093">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-4093">AppService</span></span>

* <span data-ttu-id="5550f-4094">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="5550f-4094">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5550f-4095">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-4095">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5550f-4096">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="5550f-4096">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5550f-4097">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5550f-4097">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5550f-4098">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="5550f-4098">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5550f-4099">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4099">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5550f-4100">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="5550f-4100">support slot swap with preview</span></span>
* <span data-ttu-id="5550f-4101">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4101">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5550f-4102">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4102">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5550f-4103">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5550f-4103">CosmosDB</span></span>

* <span data-ttu-id="5550f-4104">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5550f-4104">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5550f-4105">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="5550f-4105">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5550f-4106">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="5550f-4106">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5550f-4107">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="5550f-4107">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5550f-4108">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5550f-4108">Data Lake Analytics</span></span>

* <span data-ttu-id="5550f-4109">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="5550f-4109">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5550f-4110">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="5550f-4110">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5550f-4111">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4111">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5550f-4112">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="5550f-4112">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5550f-4113">Таблица</span><span class="sxs-lookup"><span data-stu-id="5550f-4113">Table</span></span>
  * <span data-ttu-id="5550f-4114">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="5550f-4114">Table valued function</span></span>
  * <span data-ttu-id="5550f-4115">Представление</span><span class="sxs-lookup"><span data-stu-id="5550f-4115">View</span></span>
  * <span data-ttu-id="5550f-4116">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="5550f-4116">Table Statistics.</span></span> <span data-ttu-id="5550f-4117">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="5550f-4117">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5550f-4118">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="5550f-4118">Data Lake Store</span></span>

* <span data-ttu-id="5550f-4119">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="5550f-4119">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5550f-4120">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4120">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5550f-4121">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="5550f-4121">missed help for access show.</span></span> <span data-ttu-id="5550f-4122">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="5550f-4122">adding it.</span></span> <span data-ttu-id="5550f-4123">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5550f-4123">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5550f-4124">Поиск</span><span class="sxs-lookup"><span data-stu-id="5550f-4124">Find</span></span>

* <span data-ttu-id="5550f-4125">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="5550f-4125">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5550f-4126">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5550f-4126">KeyVault</span></span>

* <span data-ttu-id="5550f-4127">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="5550f-4127">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5550f-4128">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="5550f-4128">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5550f-4129">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="5550f-4129">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5550f-4130">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="5550f-4130">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5550f-4131">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4131">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5550f-4132">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5550f-4132">Lab</span></span>

* <span data-ttu-id="5550f-4133">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-4133">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5550f-4134">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-4134">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5550f-4135">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-4135">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5550f-4136">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-4136">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5550f-4137">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5550f-4137">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5550f-4138">Монитор</span><span class="sxs-lookup"><span data-stu-id="5550f-4138">Monitor</span></span>

* <span data-ttu-id="5550f-4139">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4139">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5550f-4140">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4140">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5550f-4141">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-4141">Network</span></span>

* <span data-ttu-id="5550f-4142">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4142">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5550f-4143">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4143">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5550f-4144">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-4144">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5550f-4145">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5550f-4145">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5550f-4146">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5550f-4146">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5550f-4147">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="5550f-4147">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5550f-4148">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5550f-4148">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5550f-4149">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5550f-4149">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5550f-4150">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4150">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5550f-4151">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="5550f-4151">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5550f-4152">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4152">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5550f-4153">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4153">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5550f-4154">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="5550f-4154">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5550f-4155">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="5550f-4155">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5550f-4156">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="5550f-4156">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5550f-4157">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="5550f-4157">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5550f-4158">Профиль</span><span class="sxs-lookup"><span data-stu-id="5550f-4158">Profile</span></span>

* <span data-ttu-id="5550f-4159">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4159">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5550f-4160">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4160">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5550f-4161">Redis</span><span class="sxs-lookup"><span data-stu-id="5550f-4161">Redis</span></span>

* <span data-ttu-id="5550f-4162">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="5550f-4162">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5550f-4163">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="5550f-4163">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5550f-4164">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5550f-4164">Resource</span></span>

* <span data-ttu-id="5550f-4165">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4165">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5550f-4166">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4166">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5550f-4167">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4167">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5550f-4168">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="5550f-4168">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5550f-4169">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5550f-4169">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5550f-4170">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="5550f-4170">Add docs for az lock update.</span></span> <span data-ttu-id="5550f-4171">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5550f-4171">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5550f-4172">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="5550f-4172">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5550f-4173">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5550f-4173">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5550f-4174">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5550f-4174">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5550f-4175">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5550f-4175">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5550f-4176">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4176">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5550f-4177">Роль</span><span class="sxs-lookup"><span data-stu-id="5550f-4177">Role</span></span>

* <span data-ttu-id="5550f-4178">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4178">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5550f-4179">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4179">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5550f-4180">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4180">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5550f-4181">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="5550f-4181">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5550f-4182">SQL</span><span class="sxs-lookup"><span data-stu-id="5550f-4182">SQL</span></span>

* <span data-ttu-id="5550f-4183">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="5550f-4183">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5550f-4184">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4184">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5550f-4185">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-4185">Storage</span></span>

* <span data-ttu-id="5550f-4186">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4186">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5550f-4187">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-4187">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5550f-4188">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5550f-4188">Add support for large block blob upload</span></span>
* <span data-ttu-id="5550f-4189">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5550f-4189">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-4190">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-4190">VM</span></span>

* <span data-ttu-id="5550f-4191">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="5550f-4191">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5550f-4192">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="5550f-4192">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5550f-4193">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5550f-4193">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5550f-4194">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5550f-4194">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5550f-4195">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="5550f-4195">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5550f-4196">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="5550f-4196">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5550f-4197">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4197">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5550f-4198">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-4198">April 3, 2017</span></span>

<span data-ttu-id="5550f-4199">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5550f-4199">Version 2.0.2</span></span>

<span data-ttu-id="5550f-4200">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="5550f-4200">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5550f-4201">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="5550f-4201">Core</span></span>

* <span data-ttu-id="5550f-4202">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-4202">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5550f-4203">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4203">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5550f-4204">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4204">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5550f-4205">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4205">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5550f-4206">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4206">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5550f-4207">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="5550f-4207">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5550f-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4208">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5550f-4209">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5550f-4209">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5550f-4210">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="5550f-4210">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5550f-4211">ACS</span><span class="sxs-lookup"><span data-stu-id="5550f-4211">ACS</span></span>

* <span data-ttu-id="5550f-4212">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4212">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5550f-4213">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="5550f-4213">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5550f-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4214">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5550f-4215">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="5550f-4215">Add support for windows clusters.</span></span> <span data-ttu-id="5550f-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4216">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5550f-4217">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="5550f-4217">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5550f-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4218">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5550f-4219">AppService</span><span class="sxs-lookup"><span data-stu-id="5550f-4219">AppService</span></span>

* <span data-ttu-id="5550f-4220">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4220">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5550f-4221">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4221">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5550f-4222">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4222">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5550f-4223">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4223">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5550f-4224">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5550f-4224">DataLake</span></span>

* <span data-ttu-id="5550f-4225">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5550f-4225">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5550f-4226">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5550f-4226">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5550f-4227">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="5550f-4227">DocuemntDB</span></span>

* <span data-ttu-id="5550f-4228">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4228">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5550f-4229">ВМ</span><span class="sxs-lookup"><span data-stu-id="5550f-4229">VM</span></span>

* <span data-ttu-id="5550f-4230">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4230">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5550f-4231">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4231">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5550f-4232">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4232">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5550f-4233">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4233">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5550f-4234">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4234">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5550f-4235">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4235">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="5550f-4236">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="5550f-4236">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5550f-4237">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5550f-4237">February 27, 2017</span></span>

<span data-ttu-id="5550f-4238">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5550f-4238">Version 2.0.0</span></span>

<span data-ttu-id="5550f-4239">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="5550f-4239">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5550f-4240">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="5550f-4240">Container Service (acs)</span></span>
- <span data-ttu-id="5550f-4241">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="5550f-4241">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5550f-4242">Сеть</span><span class="sxs-lookup"><span data-stu-id="5550f-4242">Networking</span></span>
- <span data-ttu-id="5550f-4243">Память</span><span class="sxs-lookup"><span data-stu-id="5550f-4243">Storage</span></span>

<span data-ttu-id="5550f-4244">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4244">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5550f-4245">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="5550f-4245">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5550f-4246">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="5550f-4246">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5550f-4247">Некоторые командные модули имеют постфикс b *n* или rc *n* . Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="5550f-4247">Some of the command modules have a "b *n* " or "rc *n* " postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5550f-4248">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5550f-4248">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5550f-4249">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="5550f-4249">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5550f-4250">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="5550f-4250">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5550f-4251">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="5550f-4251">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5550f-4252">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5550f-4252">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="5550f-4253">Заметки о выпуске бета-версии</span><span class="sxs-lookup"><span data-stu-id="5550f-4253">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="5550f-4254">Бета-версия Azure CLI позволяет перейти с метода аутентификации платформы AAD (версия 1.0) на [платформу удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="5550f-4254">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="5550f-4255">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="5550f-4255">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="5550f-4256">Сведения о новой бета-версии Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5550f-4256">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="5550f-4257">Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию.</span><span class="sxs-lookup"><span data-stu-id="5550f-4257">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="5550f-4258">После установки бета-версии требуется выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="5550f-4258">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="5550f-4259">Бета-версия поддерживает только платформу Windows.</span><span class="sxs-lookup"><span data-stu-id="5550f-4259">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="5550f-4260">Azure Stack не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5550f-4260">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="5550f-4261">Параметр `--use-cert-sn-issuer` не поддерживается, если для проверки подлинности используется ключ субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5550f-4261">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="5550f-4262">Пропуск проверки SSL с использованием `ADAL_PYTHON_SSL_NO_VERIFY` среды не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5550f-4262">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="5550f-4263">Если у вас возникли проблемы с использованием бета-версии, вы можете обратиться к группе разработчиков Azure CLI на [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="5550f-4263">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
