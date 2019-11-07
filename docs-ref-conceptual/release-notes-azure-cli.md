---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/04/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3061d4b5519cfafbde92df68ecdee4d88d0bddff
ms.sourcegitcommit: b854f9b6acfdb814ba1d6ba87aac03e2d547d998
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "73536789"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="29801-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="29801-103">Azure CLI release notes</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="29801-104">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-104">November 4, 2019</span></span>

<span data-ttu-id="29801-105">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="29801-105">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="29801-106">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-106">ACR</span></span>

* <span data-ttu-id="29801-107">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="29801-107">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="29801-108">Поддерживается включение аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="29801-108">Supported enabling auditing on creating a registry</span></span>
* <span data-ttu-id="29801-109">Поддерживается функция RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="29801-109">Supported Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="29801-110">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-110">AKS</span></span>

* <span data-ttu-id="29801-111">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="29801-111">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="29801-112">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="29801-112">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="29801-113">AppConfig</span><span class="sxs-lookup"><span data-stu-id="29801-113">AppConfig</span></span>

* <span data-ttu-id="29801-114">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-114">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="29801-115">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="29801-115">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="29801-116">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="29801-116">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-117">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-117">AppService</span></span>

* <span data-ttu-id="29801-118">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="29801-118">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="29801-119">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-119">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="29801-120">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="29801-120">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="29801-121">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="29801-121">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="29801-122">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="29801-122">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="29801-123">ARM</span><span class="sxs-lookup"><span data-stu-id="29801-123">ARM</span></span>

* <span data-ttu-id="29801-124">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="29801-124">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="29801-125">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="29801-125">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="29801-126">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-126">Backup</span></span>

* <span data-ttu-id="29801-127">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="29801-127">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="29801-128">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="29801-128">Compute</span></span>

* <span data-ttu-id="29801-129">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="29801-129">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="29801-130">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="29801-130">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="29801-131">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="29801-131">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="29801-132">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="29801-132">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="29801-133">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="29801-133">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="29801-134">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set` Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-134">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="29801-135">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="29801-135">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="29801-136">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="29801-136">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-137">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-137">CosmosDB</span></span>

* <span data-ttu-id="29801-138">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create` `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="29801-138">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="29801-139">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create` `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="29801-139">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="29801-140">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-140">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="29801-141">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-141">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="29801-142">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-142">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="29801-143">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-143">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="29801-144">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="29801-144">Fixed typo in help message</span></span>
* <span data-ttu-id="29801-145">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="29801-145">database: Added deprecation infomation</span></span>
* <span data-ttu-id="29801-146">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="29801-146">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="29801-147">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-147">IoT</span></span>

* <span data-ttu-id="29801-148">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="29801-148">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="29801-149">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="29801-149">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-150">Key Vault</span><span class="sxs-lookup"><span data-stu-id="29801-150">Key Vault</span></span>

* <span data-ttu-id="29801-151">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="29801-151">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="29801-152">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="29801-152">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="29801-153">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="29801-153">NetAppFiles</span></span>

* <span data-ttu-id="29801-154">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="29801-154">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="29801-155">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="29801-155">This new API version includes:</span></span>

    - <span data-ttu-id="29801-156">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="29801-156">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="29801-157">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="29801-157">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="29801-158">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="29801-158">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="29801-159">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="29801-159">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="29801-160">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-160">Network</span></span>

* <span data-ttu-id="29801-161">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="29801-161">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="29801-162">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="29801-162">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="29801-163">`az network public-ip prefix create`: Добавлена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="29801-163">`az network public-ip prefix create`: Supported to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="29801-164">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="29801-164">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="29801-165">`az network vrouter`: Добавлена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="29801-165">`az network vrouter`: Supported new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="29801-166">`az network express-route gateway connection`: Добавлена поддержка `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="29801-166">`az network express-route gateway connection`: Supported `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-167">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-167">Profile</span></span>

* <span data-ttu-id="29801-168">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="29801-168">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="29801-169">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="29801-169">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-170">RBAC</span><span class="sxs-lookup"><span data-stu-id="29801-170">RBAC</span></span>

* <span data-ttu-id="29801-171">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="29801-171">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="29801-172">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-172">ServiceFabric</span></span>

* <span data-ttu-id="29801-173">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="29801-173">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="29801-174">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-174">SQL</span></span>

* <span data-ttu-id="29801-175">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="29801-175">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="29801-176">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-176">Storage</span></span>

* <span data-ttu-id="29801-177">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-177">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="29801-178">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-178">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="29801-179">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-179">October 15, 2019</span></span>

<span data-ttu-id="29801-180">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="29801-180">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="29801-181">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-181">AKS</span></span>

* <span data-ttu-id="29801-182">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-182">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="29801-183">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-183">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="29801-184">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-184">AMS</span></span>

* <span data-ttu-id="29801-185">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="29801-185">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="29801-186">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="29801-186">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-187">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-187">AppService</span></span>

* <span data-ttu-id="29801-188">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="29801-188">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="29801-189">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="29801-189">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="29801-190">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="29801-190">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="29801-191">ARM</span><span class="sxs-lookup"><span data-stu-id="29801-191">ARM</span></span>

* <span data-ttu-id="29801-192">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-192">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="29801-193">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="29801-193">Compute</span></span>

* <span data-ttu-id="29801-194">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-194">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="29801-195">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="29801-195">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="29801-196">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="29801-196">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="29801-197">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="29801-197">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="29801-198">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="29801-198">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="29801-199">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="29801-199">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="29801-200">Core</span><span class="sxs-lookup"><span data-stu-id="29801-200">Core</span></span>

* <span data-ttu-id="29801-201">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="29801-201">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="29801-202">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-202">IoT</span></span>

* <span data-ttu-id="29801-203">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="29801-203">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-204">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-204">Monitor</span></span>

* <span data-ttu-id="29801-205">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="29801-205">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="29801-206">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-206">Network</span></span>

* <span data-ttu-id="29801-207">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="29801-207">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="29801-208">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-208">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="29801-209">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-209">SQL</span></span>

* <span data-ttu-id="29801-210">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="29801-210">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="29801-211">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-211">Storage</span></span>

* <span data-ttu-id="29801-212">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="29801-212">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="29801-213">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-213">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="29801-214">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-214">September 24, 2019</span></span>

<span data-ttu-id="29801-215">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="29801-215">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="29801-216">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-216">ACR</span></span>

* <span data-ttu-id="29801-217">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="29801-217">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="29801-218">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="29801-218">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="29801-219">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-219">AKS</span></span>

* <span data-ttu-id="29801-220">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="29801-220">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="29801-221">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="29801-221">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="29801-222">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-222">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="29801-223">ARM</span><span class="sxs-lookup"><span data-stu-id="29801-223">ARM</span></span>

* <span data-ttu-id="29801-224">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-224">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="29801-225">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="29801-225">Compute</span></span>

* <span data-ttu-id="29801-226">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="29801-226">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="29801-227">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="29801-227">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="29801-228">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="29801-228">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="29801-229">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="29801-229">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="29801-230">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="29801-230">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="29801-231">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-231">Cosmos DB</span></span>

* <span data-ttu-id="29801-232">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="29801-232">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="29801-233">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="29801-233">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="29801-234">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="29801-234">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="29801-235">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="29801-235">EventGrid</span></span>

* <span data-ttu-id="29801-236">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="29801-236">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-237">Key Vault</span><span class="sxs-lookup"><span data-stu-id="29801-237">Key Vault</span></span>

* <span data-ttu-id="29801-238">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="29801-238">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-239">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-239">Monitor</span></span>

* <span data-ttu-id="29801-240">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="29801-240">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="29801-241">Политика</span><span class="sxs-lookup"><span data-stu-id="29801-241">Policy</span></span>

* <span data-ttu-id="29801-242">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="29801-242">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="29801-243">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="29801-243">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="29801-244">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-244">Storage</span></span>

* <span data-ttu-id="29801-245">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="29801-245">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="29801-246">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-246">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="29801-247">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-247">ACR</span></span>

* <span data-ttu-id="29801-248">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-248">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="29801-249">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-249">AKS</span></span>

* <span data-ttu-id="29801-250">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="29801-250">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="29801-251">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-251">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="29801-252">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-252">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="29801-253">ARM</span><span class="sxs-lookup"><span data-stu-id="29801-253">ARM</span></span>

* <span data-ttu-id="29801-254">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="29801-254">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="29801-255">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-255">Batch</span></span>

* <span data-ttu-id="29801-256">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="29801-256">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="29801-257">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="29801-257">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="29801-258">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="29801-258">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="29801-259">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="29801-259">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="29801-260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="29801-260">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="29801-261">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="29801-261">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="29801-262">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="29801-262">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-263">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-263">HDInsight</span></span>

* <span data-ttu-id="29801-264">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="29801-264">GA release</span></span>
* <span data-ttu-id="29801-265">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="29801-265">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-266">Key Vault</span><span class="sxs-lookup"><span data-stu-id="29801-266">Key Vault</span></span>

* <span data-ttu-id="29801-267">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="29801-267">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="29801-268">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="29801-268">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="29801-269">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-269">Network</span></span>

* <span data-ttu-id="29801-270">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="29801-270">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="29801-271">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="29801-271">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="29801-272">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="29801-272">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="29801-273">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="29801-273">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="29801-274">Политика</span><span class="sxs-lookup"><span data-stu-id="29801-274">Policy</span></span>

* <span data-ttu-id="29801-275">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="29801-275">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="29801-276">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-276">August 27, 2019</span></span>

<span data-ttu-id="29801-277">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="29801-277">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="29801-278">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-278">ACR</span></span>

* <span data-ttu-id="29801-279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="29801-279">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="29801-280">Управление API</span><span class="sxs-lookup"><span data-stu-id="29801-280">API Management</span></span>

* <span data-ttu-id="29801-281">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="29801-281">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-282">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-282">AppService</span></span>

* <span data-ttu-id="29801-283">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="29801-283">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="29801-284">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="29801-284">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-285">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-285">Keyvault</span></span>

* <span data-ttu-id="29801-286">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="29801-286">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="29801-287">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-287">Network</span></span>

* <span data-ttu-id="29801-288">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="29801-288">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="29801-289">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="29801-289">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="29801-290">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="29801-290">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="29801-291">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="29801-291">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-292">RBAC</span><span class="sxs-lookup"><span data-stu-id="29801-292">RBAC</span></span>

* <span data-ttu-id="29801-293">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="29801-293">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="29801-294">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-294">ServiceFabric</span></span>

* <span data-ttu-id="29801-295">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="29801-295">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="29801-296">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="29801-296">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="29801-297">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="29801-297">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="29801-298">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="29801-298">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="29801-299">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="29801-299">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="29801-300">SignalR</span><span class="sxs-lookup"><span data-stu-id="29801-300">SignalR</span></span>

* <span data-ttu-id="29801-301">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="29801-301">Added new commands:</span></span>
  * <span data-ttu-id="29801-302">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="29801-302">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="29801-303">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="29801-303">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="29801-304">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="29801-304">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="29801-305">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="29801-305">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-306">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-306">Storage</span></span>

* <span data-ttu-id="29801-307">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="29801-307">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="29801-308">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-308">August 13, 2019</span></span>

<span data-ttu-id="29801-309">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="29801-309">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-310">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-310">AppService</span></span>

* <span data-ttu-id="29801-311">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="29801-311">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-312">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-312">BotService</span></span>

* <span data-ttu-id="29801-313">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="29801-313">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="29801-314">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="29801-314">CognitiveServices</span></span>

* <span data-ttu-id="29801-315">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-315">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="29801-316">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-316">Cosmos DB</span></span>

* <span data-ttu-id="29801-317">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="29801-317">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="29801-318">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-318">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-319">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-319">HDInsight</span></span>

<span data-ttu-id="29801-320">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="29801-320">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="29801-321">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="29801-321">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="29801-322">Команда `--storage-default-container` переименована в `--storage-container`.</span><span class="sxs-lookup"><span data-stu-id="29801-322">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="29801-323">Команда `--storage-default-filesystem` переименована в `--storage-filesystem`.</span><span class="sxs-lookup"><span data-stu-id="29801-323">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="29801-324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="29801-324">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="29801-325">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="29801-325">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="29801-326">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="29801-326">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="29801-327">Команда `--application-type` переименована в `--type`.</span><span class="sxs-lookup"><span data-stu-id="29801-327">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="29801-328">Команда `--marketplace-identifier` переименована в `--marketplace-id`.</span><span class="sxs-lookup"><span data-stu-id="29801-328">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="29801-329">Команда `--https-endpoint-access-mode` переименована в `--access-mode`.</span><span class="sxs-lookup"><span data-stu-id="29801-329">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="29801-330">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="29801-330">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="29801-331">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="29801-331">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="29801-332">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="29801-332">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="29801-333">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="29801-333">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="29801-334">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="29801-334">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="29801-335">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="29801-335">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="29801-336">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="29801-336">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="29801-337">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="29801-337">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="29801-338">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="29801-338">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="29801-339">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-339">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="29801-340">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="29801-340">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="29801-341">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="29801-341">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="29801-342">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="29801-342">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="29801-343">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="29801-343">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-344">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-344">Interactive</span></span>

* <span data-ttu-id="29801-345">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="29801-345">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="29801-346">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="29801-346">Kubernetes</span></span>

* <span data-ttu-id="29801-347">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="29801-347">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="29801-348">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-348">Network</span></span>

* <span data-ttu-id="29801-349">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="29801-349">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-350">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-350">Profile</span></span>

* <span data-ttu-id="29801-351">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="29801-351">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="29801-352">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-352">ServiceFabric</span></span>

* <span data-ttu-id="29801-353">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="29801-353">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="29801-354">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="29801-354">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="29801-355">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-355">Storage</span></span>

* <span data-ttu-id="29801-356">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="29801-356">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="29801-357">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-357">July 30, 2019</span></span>

<span data-ttu-id="29801-358">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="29801-358">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="29801-359">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-359">ACR</span></span>

* <span data-ttu-id="29801-360">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="29801-360">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="29801-361">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="29801-361">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-362">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-362">Appservice</span></span>

* <span data-ttu-id="29801-363">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="29801-363">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="29801-364">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="29801-364">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="29801-365">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="29801-365">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="29801-366">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-366">Network</span></span>

* <span data-ttu-id="29801-367">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="29801-367">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="29801-368">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="29801-368">Fixes #9604.</span></span> <span data-ttu-id="29801-369">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-369">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="29801-370">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="29801-370">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-371">RBAC</span><span class="sxs-lookup"><span data-stu-id="29801-371">RBAC</span></span>

* <span data-ttu-id="29801-372">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="29801-372">Added `user update` command</span></span>
* <span data-ttu-id="29801-373">[УСТАРЕЛО] `--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="29801-373">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="29801-374">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="29801-374">Use replacement argument `--id`</span></span>
* <span data-ttu-id="29801-375">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="29801-375">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="29801-376">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-376">SQL</span></span>

* <span data-ttu-id="29801-377">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="29801-377">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="29801-378">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-378">Storage</span></span>

* <span data-ttu-id="29801-379">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="29801-379">Added `storage remove` command</span></span>
* <span data-ttu-id="29801-380">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="29801-380">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-381">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-381">VM</span></span>

* <span data-ttu-id="29801-382">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="29801-382">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="29801-383">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="29801-383">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="29801-384">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-384">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="29801-385">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="29801-385">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="29801-386">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="29801-386">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="29801-387">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-387">July 16, 2019</span></span>

<span data-ttu-id="29801-388">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="29801-388">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-389">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-389">Appservice</span></span>

* <span data-ttu-id="29801-390">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="29801-390">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="29801-391">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="29801-391">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="29801-392">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="29801-392">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="29801-393">Core</span><span class="sxs-lookup"><span data-stu-id="29801-393">Core</span></span>

* <span data-ttu-id="29801-394">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="29801-394">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="29801-395">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-395">Batch</span></span>

* <span data-ttu-id="29801-396">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="29801-396">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="29801-397">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="29801-397">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="29801-398">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="29801-398">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="29801-399">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-399">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="29801-400">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="29801-400">Eventhubs</span></span>

* <span data-ttu-id="29801-401">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="29801-401">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-402">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-402">RDBMS</span></span>

* <span data-ttu-id="29801-403">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="29801-403">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="29801-404">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="29801-404">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="29801-405">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="29801-405">Relay</span></span>

* <span data-ttu-id="29801-406">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="29801-406">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="29801-407">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="29801-407">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="29801-408">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-408">Servicebus</span></span>

* <span data-ttu-id="29801-409">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="29801-409">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="29801-410">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-410">Storage</span></span>

* <span data-ttu-id="29801-411">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="29801-411">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="29801-412">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="29801-412">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="29801-413">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-413">July 2, 2019</span></span>

<span data-ttu-id="29801-414">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="29801-414">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="29801-415">Core</span><span class="sxs-lookup"><span data-stu-id="29801-415">Core</span></span>

* <span data-ttu-id="29801-416">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="29801-416">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="29801-417">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="29801-417">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="29801-418">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="29801-418">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="29801-419">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-419">ACR</span></span>

* <span data-ttu-id="29801-420">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="29801-420">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-421">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-421">Appservice</span></span>

* <span data-ttu-id="29801-422">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-422">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="29801-423">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="29801-423">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="29801-424">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="29801-424">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="29801-425">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-425">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="29801-426">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-426">Cosmos DB</span></span>

* <span data-ttu-id="29801-427">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="29801-427">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="29801-428">DLS</span><span class="sxs-lookup"><span data-stu-id="29801-428">DLS</span></span>

* <span data-ttu-id="29801-429">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="29801-429">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="29801-430">Отзыв</span><span class="sxs-lookup"><span data-stu-id="29801-430">Feedback</span></span>

* <span data-ttu-id="29801-431">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="29801-431">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-432">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-432">HDInsight</span></span>

* <span data-ttu-id="29801-433">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="29801-433">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="29801-434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="29801-434">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="29801-435">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="29801-435">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="29801-436">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="29801-436">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="29801-437">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="29801-437">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="29801-438">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-438">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="29801-439">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-439">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="29801-440">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="29801-440">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="29801-441">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="29801-441">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="29801-442">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="29801-442">Managed Services</span></span>

* <span data-ttu-id="29801-443">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="29801-443">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="29801-444">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-444">Profile</span></span>
* <span data-ttu-id="29801-445">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="29801-445">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-446">RBAC</span><span class="sxs-lookup"><span data-stu-id="29801-446">RBAC</span></span>

* <span data-ttu-id="29801-447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="29801-447">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="29801-448">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="29801-448">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="29801-449">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-449">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="29801-450">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="29801-450">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-451">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-451">RDBMS</span></span>

* <span data-ttu-id="29801-452">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="29801-452">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="29801-453">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-453">SQL</span></span>

* <span data-ttu-id="29801-454">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-454">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-455">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-455">Storage</span></span>

* <span data-ttu-id="29801-456">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="29801-456">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="29801-457">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="29801-457">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="29801-458">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-458">VM</span></span>

* <span data-ttu-id="29801-459">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-459">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="29801-460">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="29801-460">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="29801-461">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="29801-461">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="29801-462">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="29801-462">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="29801-463">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-463">June 18, 2019</span></span>

<span data-ttu-id="29801-464">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="29801-464">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="29801-465">Core</span><span class="sxs-lookup"><span data-stu-id="29801-465">Core</span></span>

<span data-ttu-id="29801-466">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="29801-466">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="29801-467">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="29801-467">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="29801-468">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="29801-468">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="29801-469">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="29801-469">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="29801-470">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="29801-470">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="29801-471">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="29801-471">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="29801-472">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="29801-472">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="29801-473">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-473">ACR</span></span>
* <span data-ttu-id="29801-474">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="29801-474">Added 'acr check-health' command</span></span>
* <span data-ttu-id="29801-475">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="29801-475">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="29801-476">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-476">ACS</span></span>
* <span data-ttu-id="29801-477">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="29801-477">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="29801-478">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-478">AMS</span></span>
* <span data-ttu-id="29801-479">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="29801-479">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-480">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-480">AppService</span></span>
* <span data-ttu-id="29801-481">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="29801-481">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="29801-482">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="29801-482">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="29801-483">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="29801-483">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="29801-484">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-484">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="29801-485">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="29801-485">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="29801-486">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="29801-486">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="29801-487">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-487">Batch</span></span>
* <span data-ttu-id="29801-488">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="29801-488">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-489">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-489">BatchAI</span></span>
* <span data-ttu-id="29801-490">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="29801-490">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-491">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-491">BotService</span></span>
* <span data-ttu-id="29801-492">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="29801-492">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-493">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-493">CosmosDB</span></span>
* <span data-ttu-id="29801-494">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="29801-494">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="29801-495">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="29801-495">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="29801-496">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="29801-496">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="29801-497">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="29801-497">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="29801-498">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="29801-498">EventGrid</span></span>
* <span data-ttu-id="29801-499">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="29801-499">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="29801-500">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="29801-500">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="29801-501">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="29801-501">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="29801-502">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="29801-502">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="29801-503">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-503">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-504">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-504">HDInsight</span></span>
* <span data-ttu-id="29801-505">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="29801-505">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="29801-506">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-506">IoT</span></span>
* <span data-ttu-id="29801-507">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="29801-507">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="29801-508">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="29801-508">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="29801-509">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-509">Network</span></span>
* <span data-ttu-id="29801-510">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="29801-510">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="29801-511">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="29801-511">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="29801-512">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="29801-512">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="29801-513">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="29801-513">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="29801-514">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-514">Resource</span></span>
* <span data-ttu-id="29801-515">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="29801-515">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="29801-516">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="29801-516">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="29801-517">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-517">ServiceBus</span></span>
* <span data-ttu-id="29801-518">Исправлена ошибка [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="29801-518">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="29801-519">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-519">SQL</span></span>
* <span data-ttu-id="29801-520">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-520">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="29801-521">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="29801-521">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="29801-522">SQLVm</span><span class="sxs-lookup"><span data-stu-id="29801-522">SQLVm</span></span>
* <span data-ttu-id="29801-523">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="29801-523">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="29801-524">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="29801-524">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="29801-525">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-525">Storage</span></span>
* <span data-ttu-id="29801-526">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="29801-526">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="29801-527">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-527">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="29801-528">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-528">VM</span></span>
* <span data-ttu-id="29801-529">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="29801-529">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="29801-530">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-530">June 4, 2019</span></span>

<span data-ttu-id="29801-531">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="29801-531">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="29801-532">Core</span><span class="sxs-lookup"><span data-stu-id="29801-532">Core</span></span>
* <span data-ttu-id="29801-533">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="29801-533">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="29801-534">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-534">ACR</span></span>
* <span data-ttu-id="29801-535">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="29801-535">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="29801-536">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-536">ACS</span></span>
* <span data-ttu-id="29801-537">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-537">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="29801-538">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="29801-538">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="29801-539">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-539">Batch</span></span>
* <span data-ttu-id="29801-540">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="29801-540">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="29801-541">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-541">IoT</span></span>
* <span data-ttu-id="29801-542">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="29801-542">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="29801-543">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-543">Network</span></span>
* <span data-ttu-id="29801-544">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="29801-544">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="29801-545">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-545">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="29801-546">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-546">Resource</span></span>
* <span data-ttu-id="29801-547">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="29801-547">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="29801-548">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-548">Role</span></span>
* <span data-ttu-id="29801-549">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="29801-549">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="29801-550">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="29801-550">Compute</span></span>
* <span data-ttu-id="29801-551">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="29801-551">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="29801-552">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-552">May 21, 2019</span></span>

<span data-ttu-id="29801-553">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="29801-553">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="29801-554">Core</span><span class="sxs-lookup"><span data-stu-id="29801-554">Core</span></span>
* <span data-ttu-id="29801-555">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="29801-555">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="29801-556">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="29801-556">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="29801-557">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="29801-557">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="29801-558">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-558">ACR</span></span>
* <span data-ttu-id="29801-559">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="29801-559">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="29801-560">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-560">ACS</span></span>
* <span data-ttu-id="29801-561">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="29801-561">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-562">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-562">AppService</span></span>
* <span data-ttu-id="29801-563">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="29801-563">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="29801-564">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="29801-564">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="29801-565">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="29801-565">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="29801-566">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="29801-566">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="29801-567">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="29801-567">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="29801-568">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="29801-568">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="29801-569">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="29801-569">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-570">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-570">BotService</span></span>
* <span data-ttu-id="29801-571">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="29801-571">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="29801-572">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="29801-572">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-573">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-573">Consumption</span></span>
* <span data-ttu-id="29801-574">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-574">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="29801-575">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-575">IoT</span></span>
* <span data-ttu-id="29801-576">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="29801-576">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="29801-577">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-577">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="29801-579">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="29801-579">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="29801-580">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="29801-580">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-581">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-581">RDBMS</span></span>
* <span data-ttu-id="29801-582">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="29801-582">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-583">RBAC</span><span class="sxs-lookup"><span data-stu-id="29801-583">RBAC</span></span>
* <span data-ttu-id="29801-584">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="29801-584">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-585">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-585">Storage</span></span>
* <span data-ttu-id="29801-586">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-586">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="29801-587">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="29801-587">Compute</span></span>
* <span data-ttu-id="29801-588">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="29801-588">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="29801-589">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="29801-589">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="29801-590">__Примечание__. Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="29801-590">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="29801-591">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="29801-591">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="29801-592">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-592">May 6, 2019</span></span>

<span data-ttu-id="29801-593">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="29801-593">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="29801-594">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-594">ACS</span></span>
* <span data-ttu-id="29801-595">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="29801-595">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="29801-596">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="29801-596">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="29801-597">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="29801-597">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="29801-598">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-598">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-599">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-599">Appservice</span></span>
* <span data-ttu-id="29801-600">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="29801-600">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="29801-601">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="29801-601">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="29801-602">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="29801-602">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="29801-603">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-603">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="29801-604">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="29801-604">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="29801-605">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="29801-605">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="29801-606">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-606">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="29801-607">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="29801-607">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="29801-608">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-608">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="29801-609">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="29801-609">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="29801-610">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-610">Batch</span></span>
* <span data-ttu-id="29801-611">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="29801-611">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-612">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-612">Botservice</span></span>
* <span data-ttu-id="29801-613">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="29801-613">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="29801-614">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="29801-614">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="29801-615">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="29801-615">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="29801-616">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-616">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="29801-617">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-617">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="29801-618">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="29801-618">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="29801-619">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="29801-619">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="29801-620">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="29801-620">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="29801-621">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="29801-621">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="29801-622">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="29801-622">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="29801-623">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="29801-623">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="29801-624">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="29801-624">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="29801-625">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="29801-625">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="29801-626">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="29801-626">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="29801-627">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-627">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="29801-628">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="29801-628">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="29801-629">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="29801-629">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="29801-630">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="29801-630">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="29801-631">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="29801-631">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="29801-632">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="29801-632">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="29801-633">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="29801-633">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="29801-634">Настройка</span><span class="sxs-lookup"><span data-stu-id="29801-634">Configure</span></span>
* <span data-ttu-id="29801-635">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="29801-635">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="29801-636">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="29801-636">Eventhubs</span></span>
* <span data-ttu-id="29801-637">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-637">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="29801-638">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-638">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="29801-639">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-639">Network</span></span>
* <span data-ttu-id="29801-640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-640">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="29801-641">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="29801-641">Policy Insights</span></span>
* <span data-ttu-id="29801-642">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-642">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="29801-643">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-643">Role</span></span>
* <span data-ttu-id="29801-644">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="29801-644">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="29801-645">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-645">Service Bus</span></span>
* <span data-ttu-id="29801-646">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-646">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="29801-647">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-647">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="29801-648">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="29801-648">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="29801-649">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-649">SQL</span></span>
* <span data-ttu-id="29801-650">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="29801-650">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="29801-651">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-651">VM</span></span>
* <span data-ttu-id="29801-652">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="29801-652">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="29801-653">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="29801-653">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="29801-654">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-654">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="29801-655">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="29801-655">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="29801-656">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="29801-656">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="29801-657">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="29801-657">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="29801-658">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-658">April 23, 2019</span></span>

<span data-ttu-id="29801-659">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="29801-659">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="29801-660">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-660">ACS</span></span>
* <span data-ttu-id="29801-661">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="29801-661">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="29801-662">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="29801-662">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="29801-663">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-663">AMS</span></span>
* <span data-ttu-id="29801-664">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="29801-664">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-665">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-665">AppService</span></span>
* <span data-ttu-id="29801-666">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="29801-666">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="29801-667">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="29801-667">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="29801-668">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="29801-668">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="29801-669">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="29801-669">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="29801-670">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-670">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="29801-671">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="29801-671">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="29801-672">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="29801-672">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="29801-673">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="29801-673">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="29801-674">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="29801-674">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="29801-675">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="29801-675">Deployment Manager</span></span>
* <span data-ttu-id="29801-676">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="29801-676">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="29801-677">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="29801-677">Lab</span></span>
* <span data-ttu-id="29801-678">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="29801-678">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="29801-679">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-679">Network</span></span>
* <span data-ttu-id="29801-680">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="29801-680">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="29801-681">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-681">Resource</span></span>
* <span data-ttu-id="29801-682">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="29801-682">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="29801-683">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="29801-683">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="29801-684">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="29801-684">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="29801-685">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="29801-685">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="29801-686">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-686">SQL</span></span>
* <span data-ttu-id="29801-687">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="29801-687">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="29801-688">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="29801-688">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="29801-689">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-689">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="29801-690">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-690">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-691">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-691">Storage</span></span>
* <span data-ttu-id="29801-692">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="29801-692">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-693">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-693">VM</span></span>
* <span data-ttu-id="29801-694">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="29801-694">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="29801-695">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="29801-695">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="29801-696">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="29801-696">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="29801-697">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-697">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="29801-698">Core</span><span class="sxs-lookup"><span data-stu-id="29801-698">Core</span></span>
* <span data-ttu-id="29801-699">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="29801-699">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="29801-700">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-700">ACR</span></span>
* <span data-ttu-id="29801-701">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="29801-701">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="29801-702">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-702">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="29801-705">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="29801-705">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="29801-706">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="29801-706">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-707">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-707">AppService</span></span>
* <span data-ttu-id="29801-708">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="29801-708">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="29801-709">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="29801-709">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="29801-710">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="29801-710">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="29801-711">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-711">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="29801-712">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-712">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="29801-713">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="29801-713">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="29801-714">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-714">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-715">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-715">CDN</span></span>
* <span data-ttu-id="29801-716">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="29801-716">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="29801-717">Отзыв</span><span class="sxs-lookup"><span data-stu-id="29801-717">Feedback</span></span>
* <span data-ttu-id="29801-718">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="29801-718">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="29801-719">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="29801-719">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="29801-720">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="29801-720">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-721">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-721">Monitor</span></span>
* <span data-ttu-id="29801-722">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-722">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="29801-723">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-723">Network</span></span>
* <span data-ttu-id="29801-724">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="29801-724">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="29801-725">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-725">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="29801-726">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="29801-726">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="29801-727">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="29801-727">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="29801-728">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="29801-728">PrivateDNS</span></span>
* <span data-ttu-id="29801-729">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="29801-729">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="29801-730">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-730">Resource</span></span>
* <span data-ttu-id="29801-731">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="29801-731">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="29801-732">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-732">Role</span></span>
* <span data-ttu-id="29801-733">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="29801-733">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="29801-734">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="29801-734">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="29801-735">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-735">SQL</span></span>
* <span data-ttu-id="29801-736">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="29801-736">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="29801-737">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-737">Storage</span></span>
* <span data-ttu-id="29801-738">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="29801-738">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="29801-739">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="29801-739">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="29801-740">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="29801-740">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="29801-741">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="29801-741">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="29801-742">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-742">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="29801-743">Core</span><span class="sxs-lookup"><span data-stu-id="29801-743">Core</span></span>
* <span data-ttu-id="29801-744">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="29801-744">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="29801-745">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="29801-745">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="29801-746">Облако</span><span class="sxs-lookup"><span data-stu-id="29801-746">Cloud</span></span>
* <span data-ttu-id="29801-747">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="29801-747">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="29801-748">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-748">ACR</span></span>
* <span data-ttu-id="29801-749">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="29801-749">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="29801-750">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="29801-750">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="29801-751">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="29801-751">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="29801-752">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="29801-752">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-753">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-753">AppService</span></span>
* <span data-ttu-id="29801-754">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="29801-754">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="29801-755">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="29801-755">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="29801-756">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-756">BOT Service</span></span>
* <span data-ttu-id="29801-757">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="29801-757">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="29801-758">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="29801-758">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="29801-759">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="29801-759">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="29801-760">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="29801-760">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-761">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-761">CDN</span></span>
* <span data-ttu-id="29801-762">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="29801-762">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="29801-763">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-763">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="29801-764">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-764">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="29801-765">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="29801-765">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-766">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-766">Cosmosdb</span></span>
* <span data-ttu-id="29801-767">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="29801-767">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="29801-768">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="29801-768">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-769">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-769">Interactive</span></span>
* <span data-ttu-id="29801-770">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="29801-770">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-771">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-771">Monitor</span></span>
* <span data-ttu-id="29801-772">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-772">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="29801-773">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-773">Network</span></span>
* <span data-ttu-id="29801-774">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="29801-774">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-775">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-775">Profile</span></span>
* <span data-ttu-id="29801-776">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="29801-776">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="29801-777">Postgres</span><span class="sxs-lookup"><span data-stu-id="29801-777">Postgres</span></span> 
* <span data-ttu-id="29801-778">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="29801-778">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="29801-779">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-779">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="29801-780">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-780">Resource</span></span>
* <span data-ttu-id="29801-781">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-781">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="29801-782">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="29801-782">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="29801-783">График</span><span class="sxs-lookup"><span data-stu-id="29801-783">Graph</span></span>
* <span data-ttu-id="29801-784">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="29801-784">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="29801-785">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="29801-785">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="29801-786">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="29801-786">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="29801-787">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="29801-787">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="29801-788">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="29801-788">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="29801-789">storage</span><span class="sxs-lookup"><span data-stu-id="29801-789">storage</span></span>
* <span data-ttu-id="29801-790">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-790">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="29801-791">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="29801-791">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="29801-792">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="29801-792">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="29801-793">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="29801-793">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="29801-794">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-794">VM</span></span>
* <span data-ttu-id="29801-795">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="29801-795">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="29801-796">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-796">March 12, 2019</span></span>

<span data-ttu-id="29801-797">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="29801-797">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="29801-798">Core</span><span class="sxs-lookup"><span data-stu-id="29801-798">Core</span></span>

* <span data-ttu-id="29801-799">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="29801-799">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="29801-800">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-800">ACR</span></span>

* <span data-ttu-id="29801-801">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="29801-801">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="29801-802">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-802">ACS</span></span>

* <span data-ttu-id="29801-803">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="29801-803">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="29801-804">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-804">AppService</span></span>

* <span data-ttu-id="29801-805">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="29801-805">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="29801-806">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="29801-806">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="29801-807">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-807">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="29801-808">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="29801-808">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-809">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-809">Botservice</span></span>

* <span data-ttu-id="29801-810">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="29801-810">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="29801-811">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="29801-811">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="29801-812">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="29801-812">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="29801-813">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="29801-813">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="29801-814">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-814">Container</span></span>

* <span data-ttu-id="29801-815">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="29801-815">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="29801-816">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="29801-816">EventHub</span></span>

* <span data-ttu-id="29801-817">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="29801-817">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="29801-818">Поиск</span><span class="sxs-lookup"><span data-stu-id="29801-818">Find</span></span>

* <span data-ttu-id="29801-819">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="29801-819">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-820">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-820">HDInsight</span></span>

* <span data-ttu-id="29801-821">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="29801-821">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="29801-822">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-822">Network</span></span>

* <span data-ttu-id="29801-823">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="29801-823">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-824">Rdbms</span><span class="sxs-lookup"><span data-stu-id="29801-824">Rdbms</span></span>

* <span data-ttu-id="29801-825">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-825">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="29801-826">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-826">Role</span></span>

* <span data-ttu-id="29801-827">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="29801-827">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="29801-828">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="29801-828">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="29801-829">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-829">Service Fabric</span></span>

* <span data-ttu-id="29801-830">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="29801-830">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="29801-831">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-831">February 26, 2019</span></span>

<span data-ttu-id="29801-832">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="29801-832">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="29801-833">Core</span><span class="sxs-lookup"><span data-stu-id="29801-833">Core</span></span>

* <span data-ttu-id="29801-834">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="29801-834">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="29801-835">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-835">ACR</span></span>

* <span data-ttu-id="29801-836">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="29801-836">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="29801-837">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-837">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="29801-838">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-838">ACS</span></span>

* <span data-ttu-id="29801-839">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="29801-839">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-840">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-840">AppService</span></span>

* <span data-ttu-id="29801-841">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="29801-841">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="29801-842">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-842">Batch</span></span>
* <span data-ttu-id="29801-843">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="29801-843">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="29801-844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="29801-844">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="29801-845">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="29801-845">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="29801-846">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="29801-846">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="29801-847">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="29801-847">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="29801-848">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29801-848">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-849">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-849">CosmosDB</span></span>

* <span data-ttu-id="29801-850">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="29801-850">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="29801-851">Kusto</span><span class="sxs-lookup"><span data-stu-id="29801-851">Kusto</span></span>

* <span data-ttu-id="29801-852">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="29801-852">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="29801-853">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-853">Network</span></span>

* <span data-ttu-id="29801-854">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-854">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="29801-855">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="29801-855">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="29801-856">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="29801-856">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="29801-857">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-857">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="29801-858">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-858">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="29801-859">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-859">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="29801-860">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="29801-860">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="29801-861">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-861">Resource</span></span>

* <span data-ttu-id="29801-862">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="29801-862">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="29801-863">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="29801-863">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="29801-864">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="29801-864">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="29801-865">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="29801-865">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="29801-866">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-866">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="29801-867">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-867">Role</span></span>

* <span data-ttu-id="29801-868">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-868">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-869">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-869">VM</span></span>

* <span data-ttu-id="29801-870">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="29801-870">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="29801-871">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-871">February 12, 2019</span></span>

<span data-ttu-id="29801-872">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="29801-872">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="29801-873">Core</span><span class="sxs-lookup"><span data-stu-id="29801-873">Core</span></span>

* <span data-ttu-id="29801-874">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="29801-874">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="29801-875">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-875">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="29801-876">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-876">ACR</span></span>
* <span data-ttu-id="29801-877">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="29801-877">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="29801-878">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="29801-878">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="29801-879">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-879">ACS</span></span>
* <span data-ttu-id="29801-880">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="29801-880">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="29801-881">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="29801-881">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="29801-882">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="29801-882">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="29801-883">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-883">AMS</span></span>
* <span data-ttu-id="29801-884">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-884">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="29801-885">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-885">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-886">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-886">Appservice</span></span>
* <span data-ttu-id="29801-887">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-887">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="29801-888">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-888">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="29801-889">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="29801-889">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="29801-890">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="29801-890">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="29801-891">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-891">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-892">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-892">Botservice</span></span>
* <span data-ttu-id="29801-893">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="29801-893">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="29801-894">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="29801-894">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="29801-895">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="29801-895">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="29801-896">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="29801-896">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="29801-897">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="29801-897">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="29801-898">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="29801-898">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="29801-899">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-899">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="29801-900">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-900">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="29801-901">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="29801-901">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="29801-902">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="29801-902">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-903">Key Vault</span><span class="sxs-lookup"><span data-stu-id="29801-903">Key Vault</span></span>
* <span data-ttu-id="29801-904">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="29801-904">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-905">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-905">Monitor</span></span>
* <span data-ttu-id="29801-906">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="29801-906">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="29801-907">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-907">Network</span></span>
* <span data-ttu-id="29801-908">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="29801-908">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="29801-909">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-909">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="29801-910">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="29801-910">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="29801-911">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="29801-911">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="29801-912">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="29801-912">Policy Insights</span></span>
* <span data-ttu-id="29801-913">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-913">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-914">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-914">RDBMS</span></span>
* <span data-ttu-id="29801-915">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="29801-915">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="29801-916">Redis</span><span class="sxs-lookup"><span data-stu-id="29801-916">Redis</span></span>
* <span data-ttu-id="29801-917">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="29801-917">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="29801-918">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="29801-918">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="29801-919">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="29801-919">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="29801-920">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="29801-920">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="29801-921">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="29801-921">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="29801-922">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="29801-922">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="29801-923">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29801-923">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="29801-924">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-924">Role</span></span>
* <span data-ttu-id="29801-925">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="29801-925">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="29801-926">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="29801-926">SQL VM</span></span>
* <span data-ttu-id="29801-927">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="29801-927">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="29801-928">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-928">VM</span></span>
* <span data-ttu-id="29801-929">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="29801-929">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="29801-930">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-930">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="29801-931">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="29801-931">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="29801-932">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="29801-932">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="29801-933">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-933">January 31, 2019</span></span>

<span data-ttu-id="29801-934">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="29801-934">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="29801-935">Core</span><span class="sxs-lookup"><span data-stu-id="29801-935">Core</span></span>

* <span data-ttu-id="29801-936">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="29801-936">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="29801-937">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-937">January 28, 2019</span></span>

<span data-ttu-id="29801-938">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="29801-938">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="29801-939">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-939">ACR</span></span>
* <span data-ttu-id="29801-940">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="29801-940">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="29801-941">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-941">ACS</span></span>
* <span data-ttu-id="29801-942">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="29801-942">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="29801-943">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="29801-943">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="29801-944">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="29801-944">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="29801-945">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-945">AMS</span></span>
* <span data-ttu-id="29801-946">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="29801-946">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="29801-947">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="29801-947">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-948">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-948">Appservice</span></span>
* <span data-ttu-id="29801-949">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="29801-949">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="29801-950">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="29801-950">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="29801-951">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="29801-951">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="29801-952">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-952">Container</span></span>
* <span data-ttu-id="29801-953">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="29801-953">Added `container start` command</span></span>
* <span data-ttu-id="29801-954">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-954">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="29801-955">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="29801-955">EventGrid</span></span>
* <span data-ttu-id="29801-956">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-956">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="29801-957">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="29801-957">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="29801-958">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="29801-958">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="29801-959">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="29801-959">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="29801-960">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="29801-960">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-961">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-961">HDInsight</span></span>
* <span data-ttu-id="29801-962">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-962">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="29801-963">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-963">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="29801-964">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="29801-964">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="29801-965">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="29801-965">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="29801-966">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="29801-966">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="29801-967">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="29801-967">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="29801-968">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-968">IoT</span></span>
* <span data-ttu-id="29801-969">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="29801-969">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="29801-970">Kusto</span><span class="sxs-lookup"><span data-stu-id="29801-970">Kusto</span></span>
* <span data-ttu-id="29801-971">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="29801-971">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-972">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-972">Monitor</span></span>
* <span data-ttu-id="29801-973">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="29801-973">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="29801-974">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-974">Profile</span></span>
* <span data-ttu-id="29801-975">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="29801-975">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="29801-976">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-976">Network</span></span>
* <span data-ttu-id="29801-977">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="29801-977">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="29801-978">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="29801-978">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="29801-979">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-979">Resource</span></span>
* <span data-ttu-id="29801-980">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="29801-980">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="29801-981">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-981">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="29801-982">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="29801-982">SQL Virtual Machine</span></span>
* <span data-ttu-id="29801-983">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="29801-983">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="29801-984">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-984">Storage</span></span>
* <span data-ttu-id="29801-985">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="29801-985">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="29801-986">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="29801-986">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="29801-987">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-987">VM</span></span>
* <span data-ttu-id="29801-988">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="29801-988">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="29801-989">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="29801-989">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="29801-990">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="29801-990">January 15, 2019</span></span>

<span data-ttu-id="29801-991">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="29801-991">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="29801-992">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-992">ACR</span></span>
* <span data-ttu-id="29801-993">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="29801-993">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="29801-994">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="29801-994">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="29801-995">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="29801-995">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="29801-996">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-996">ACS</span></span>
* <span data-ttu-id="29801-997">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="29801-997">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-998">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-998">Appservice</span></span>
* <span data-ttu-id="29801-999">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="29801-999">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="29801-1000">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-1000">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="29801-1001">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="29801-1001">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="29801-1002">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="29801-1002">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-1003">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-1003">Botservice</span></span>
* <span data-ttu-id="29801-1004">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1004">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="29801-1005">Настройка</span><span class="sxs-lookup"><span data-stu-id="29801-1005">Configure</span></span>
* <span data-ttu-id="29801-1006">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="29801-1006">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-1007">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-1007">CosmosDB</span></span>
* <span data-ttu-id="29801-1008">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="29801-1008">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-1009">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-1009">HDInsight</span></span>
* <span data-ttu-id="29801-1010">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="29801-1010">Added commands for managing applications</span></span>
* <span data-ttu-id="29801-1011">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="29801-1011">Added commands for managing script actions</span></span>
* <span data-ttu-id="29801-1012">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="29801-1012">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="29801-1013">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="29801-1013">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="29801-1014">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1014">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="29801-1015">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1015">Network</span></span>
* <span data-ttu-id="29801-1016">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-1016">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="29801-1017">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="29801-1017">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="29801-1018">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-1018">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="29801-1019">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1019">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="29801-1020">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1020">Role</span></span>
* <span data-ttu-id="29801-1021">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29801-1021">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="29801-1022">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="29801-1022">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="29801-1023">Безопасность</span><span class="sxs-lookup"><span data-stu-id="29801-1023">Security</span></span>
* <span data-ttu-id="29801-1024">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-1024">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1025">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1025">Storage</span></span>
* <span data-ttu-id="29801-1026">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="29801-1026">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="29801-1027">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="29801-1027">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="29801-1028">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1028">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="29801-1029">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1029">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="29801-1030">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="29801-1030">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1031">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1031">VM</span></span>
* <span data-ttu-id="29801-1032">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="29801-1032">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="29801-1033">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1033">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="29801-1034">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="29801-1034">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="29801-1035">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="29801-1035">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="29801-1036">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1036">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="29801-1037">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-1037">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="29801-1038">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1038">December 20, 2018</span></span>

<span data-ttu-id="29801-1039">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="29801-1039">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="29801-1040">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1040">Appservice</span></span>
* <span data-ttu-id="29801-1041">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="29801-1041">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="29801-1042">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="29801-1042">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="29801-1043">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-1043">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="29801-1044">IoT Central</span><span class="sxs-lookup"><span data-stu-id="29801-1044">IoTCentral</span></span>
* <span data-ttu-id="29801-1045">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="29801-1045">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="29801-1046">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1046">Role</span></span>
* <span data-ttu-id="29801-1047">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-1047">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1048">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1048">SQL</span></span>
* <span data-ttu-id="29801-1049">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="29801-1049">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1050">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1050">VM</span></span>
* <span data-ttu-id="29801-1051">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1051">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="29801-1052">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1052">December 18, 2018</span></span>

<span data-ttu-id="29801-1053">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="29801-1053">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="29801-1054">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1054">ACR</span></span>
* <span data-ttu-id="29801-1055">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1055">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="29801-1056">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="29801-1056">Condensed the table layout for task list</span></span>
* <span data-ttu-id="29801-1057">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="29801-1057">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1058">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1058">ACS</span></span>
* <span data-ttu-id="29801-1059">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="29801-1059">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="29801-1060">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="29801-1060">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="29801-1061">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="29801-1061">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="29801-1062">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1062">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="29801-1063">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-1063">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="29801-1064">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="29801-1064">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1065">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1065">Appservice</span></span>
* <span data-ttu-id="29801-1066">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="29801-1066">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="29801-1067">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-1067">Botservice</span></span>
* <span data-ttu-id="29801-1068">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1068">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="29801-1069">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="29801-1069">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="29801-1070">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="29801-1070">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="29801-1071">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="29801-1071">Reduced Kudu network calls</span></span>
* <span data-ttu-id="29801-1072">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1072">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-1073">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-1073">Consumption</span></span>
* <span data-ttu-id="29801-1074">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="29801-1074">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-1075">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-1075">CosmosDB</span></span>
* <span data-ttu-id="29801-1076">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="29801-1076">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="29801-1077">Maps</span><span class="sxs-lookup"><span data-stu-id="29801-1077">Maps</span></span>
* <span data-ttu-id="29801-1078">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="29801-1078">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="29801-1079">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1079">Network</span></span>
* <span data-ttu-id="29801-1080">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="29801-1080">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="29801-1081">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="29801-1081">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1082">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1082">Resource</span></span>
* <span data-ttu-id="29801-1083">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1083">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="29801-1084">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1084">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1085">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1085">Storage</span></span>
*  <span data-ttu-id="29801-1086">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="29801-1086">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1087">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1087">VM</span></span>
* <span data-ttu-id="29801-1088">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1088">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="29801-1089">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1089">December 4, 2018</span></span>

<span data-ttu-id="29801-1090">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="29801-1090">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="29801-1091">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1091">Core</span></span>
* <span data-ttu-id="29801-1092">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1092">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="29801-1093">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="29801-1093">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1094">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1094">Appservice</span></span>
* <span data-ttu-id="29801-1095">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="29801-1095">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="29801-1096">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="29801-1096">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="29801-1097">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1097">Network</span></span>
* <span data-ttu-id="29801-1098">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="29801-1098">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="29801-1099">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1099">Role</span></span>
* <span data-ttu-id="29801-1100">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="29801-1100">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="29801-1101">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1101">VM</span></span>
* <span data-ttu-id="29801-1102">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29801-1102">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="29801-1103">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="29801-1103">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="29801-1104">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="29801-1104">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="29801-1105">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="29801-1105">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="29801-1106">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1106">November 20, 2018</span></span>

<span data-ttu-id="29801-1107">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="29801-1107">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="29801-1108">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1108">Core</span></span>
* <span data-ttu-id="29801-1109">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="29801-1109">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1110">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1110">ACR</span></span>
* <span data-ttu-id="29801-1111">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="29801-1111">Added context token to task step</span></span>
* <span data-ttu-id="29801-1112">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-1112">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="29801-1113">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="29801-1113">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1114">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1114">Appservice</span></span>
* <span data-ttu-id="29801-1115">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="29801-1115">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="29801-1116">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1116">Updated the default `node_version`.</span></span> <span data-ttu-id="29801-1117">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="29801-1117">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="29801-1118">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="29801-1118">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="29801-1119">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="29801-1119">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="29801-1120">IotCentral</span><span class="sxs-lookup"><span data-stu-id="29801-1120">IotCentral</span></span>
* <span data-ttu-id="29801-1121">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="29801-1121">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-1122">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-1122">KeyVault</span></span>
* <span data-ttu-id="29801-1123">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="29801-1123">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="29801-1124">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1124">Network</span></span>
* <span data-ttu-id="29801-1125">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-1125">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="29801-1126">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="29801-1126">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="29801-1127">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="29801-1127">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="29801-1128">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="29801-1128">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1129">Rdbms</span><span class="sxs-lookup"><span data-stu-id="29801-1129">Rdbms</span></span>
* <span data-ttu-id="29801-1130">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="29801-1130">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="29801-1131">RBAC:</span><span class="sxs-lookup"><span data-stu-id="29801-1131">Rbac</span></span>
* <span data-ttu-id="29801-1132">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1132">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="29801-1133">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="29801-1133">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="29801-1134">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1134">Storage</span></span>
* <span data-ttu-id="29801-1135">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="29801-1135">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="29801-1136">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-1136">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="29801-1137">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="29801-1137">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="29801-1138">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="29801-1138">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1139">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1139">VM</span></span>
* <span data-ttu-id="29801-1140">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="29801-1140">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="29801-1141">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="29801-1141">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="29801-1142">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="29801-1142">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="29801-1143">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="29801-1143">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="29801-1144">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1144">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="29801-1145">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1145">Added `snapshot wait` command</span></span>
* <span data-ttu-id="29801-1146">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-1146">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="29801-1147">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1147">November 6, 2018</span></span>

<span data-ttu-id="29801-1148">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="29801-1148">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="29801-1149">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1149">Core</span></span>
* <span data-ttu-id="29801-1150">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="29801-1150">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1151">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1151">ACR</span></span>
* <span data-ttu-id="29801-1152">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="29801-1152">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="29801-1153">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="29801-1153">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1154">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1154">ACS</span></span>
* <span data-ttu-id="29801-1155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1155">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="29801-1156">Помощник</span><span class="sxs-lookup"><span data-stu-id="29801-1156">Advisor</span></span>
* <span data-ttu-id="29801-1157">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="29801-1157">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="29801-1158">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-1158">AMS</span></span>
* <span data-ttu-id="29801-1159">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="29801-1159">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="29801-1160">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="29801-1160">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="29801-1161">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1161">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="29801-1162">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="29801-1162">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="29801-1163">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="29801-1163">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="29801-1164">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="29801-1164">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="29801-1165">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="29801-1165">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="29801-1166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="29801-1166">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="29801-1167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="29801-1167">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="29801-1168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-1168">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="29801-1169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-1169">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="29801-1170">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="29801-1170">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="29801-1171">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="29801-1171">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="29801-1172">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="29801-1172">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="29801-1173">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="29801-1173">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="29801-1174">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="29801-1174">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="29801-1175">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="29801-1175">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1176">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1176">AppService</span></span>
* <span data-ttu-id="29801-1177">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="29801-1177">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="29801-1178">Настройка</span><span class="sxs-lookup"><span data-stu-id="29801-1178">Configure</span></span>
* <span data-ttu-id="29801-1179">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="29801-1179">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="29801-1180">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1180">Container</span></span>
* <span data-ttu-id="29801-1181">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="29801-1181">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="29801-1182">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="29801-1182">EventHub</span></span>
* <span data-ttu-id="29801-1183">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1183">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1184">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1184">Interactive</span></span>
* <span data-ttu-id="29801-1185">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="29801-1185">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-1186">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-1186">Monitor</span></span>
* <span data-ttu-id="29801-1187">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1187">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="29801-1188">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1188">Network</span></span>
* <span data-ttu-id="29801-1189">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="29801-1189">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="29801-1190">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="29801-1190">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="29801-1191">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1191">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="29801-1192">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-1192">Profile</span></span>
* <span data-ttu-id="29801-1193">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-1193">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1194">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-1194">RDBMS</span></span>
* <span data-ttu-id="29801-1195">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="29801-1195">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1196">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1196">Resource</span></span>
* <span data-ttu-id="29801-1197">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="29801-1197">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="29801-1198">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1198">Role</span></span>
* <span data-ttu-id="29801-1199">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-1199">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="29801-1200">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1200">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="29801-1201">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="29801-1201">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1202">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1202">Storage</span></span>
* <span data-ttu-id="29801-1203">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="29801-1203">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1204">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1204">VM</span></span>
* <span data-ttu-id="29801-1205">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="29801-1205">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="29801-1206">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="29801-1206">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="29801-1207">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="29801-1207">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="29801-1208">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="29801-1208">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="29801-1209">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="29801-1209">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="29801-1210">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="29801-1210">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="29801-1211">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1211">October 23, 2018</span></span>

<span data-ttu-id="29801-1212">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="29801-1212">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="29801-1213">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1213">Core</span></span>
* <span data-ttu-id="29801-1214">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-1214">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="29801-1215">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-1215">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1216">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1216">ACR</span></span>
* <span data-ttu-id="29801-1217">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="29801-1217">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-1218">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-1218">CDN</span></span>
* <span data-ttu-id="29801-1219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1219">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="29801-1220">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="29801-1220">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="29801-1221">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1221">Container</span></span>
* <span data-ttu-id="29801-1222">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="29801-1222">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="29801-1223">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="29801-1223">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="29801-1224">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-1224">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="29801-1225">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1225">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="29801-1226">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="29801-1226">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="29801-1227">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="29801-1227">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="29801-1228">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1228">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-1229">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-1229">CosmosDB</span></span>
* <span data-ttu-id="29801-1230">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="29801-1230">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1231">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1231">Interactive</span></span>
* <span data-ttu-id="29801-1232">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="29801-1232">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="29801-1233">IoT Central</span><span class="sxs-lookup"><span data-stu-id="29801-1233">IoT Central</span></span>
* <span data-ttu-id="29801-1234">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="29801-1234">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="29801-1235">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="29801-1235">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-1236">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-1236">Monitor</span></span>
* <span data-ttu-id="29801-1237">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="29801-1237">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="29801-1238">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-1238">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="29801-1239">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="29801-1239">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="29801-1240">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="29801-1240">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="29801-1241">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="29801-1241">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="29801-1242">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="29801-1242">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="29801-1243">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="29801-1243">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="29801-1244">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="29801-1244">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="29801-1245">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="29801-1245">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="29801-1246">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1246">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="29801-1247">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1247">Network</span></span>
* <span data-ttu-id="29801-1248">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="29801-1248">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="29801-1249">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="29801-1249">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="29801-1250">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-1250">ServiceBus</span></span>
* <span data-ttu-id="29801-1251">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="29801-1251">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1252">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1252">SQL</span></span>
* <span data-ttu-id="29801-1253">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="29801-1253">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1254">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1254">Storage</span></span>
* <span data-ttu-id="29801-1255">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1255">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="29801-1256">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="29801-1256">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1257">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1257">VM</span></span>
* <span data-ttu-id="29801-1258">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="29801-1258">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="29801-1259">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="29801-1259">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="29801-1260">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="29801-1260">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="29801-1261">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1261">October 16, 2018</span></span>

<span data-ttu-id="29801-1262">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="29801-1262">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1263">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1263">VM</span></span>
* <span data-ttu-id="29801-1264">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="29801-1264">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="29801-1265">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1265">October 9, 2018</span></span>

<span data-ttu-id="29801-1266">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="29801-1266">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="29801-1267">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1267">Core</span></span>
* <span data-ttu-id="29801-1268">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="29801-1268">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1269">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1269">ACR</span></span>
* <span data-ttu-id="29801-1270">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="29801-1270">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1271">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1271">ACS</span></span>
* <span data-ttu-id="29801-1272">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="29801-1272">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="29801-1273">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="29801-1273">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="29801-1274">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="29801-1274">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="29801-1275">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="29801-1275">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="29801-1276">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1276">Container</span></span>
* <span data-ttu-id="29801-1277">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="29801-1277">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="29801-1278">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-1278">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="29801-1279">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="29801-1279">Event Hub</span></span>
* <span data-ttu-id="29801-1280">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1280">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="29801-1281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="29801-1281">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="29801-1282">расширения.</span><span class="sxs-lookup"><span data-stu-id="29801-1282">Extensions</span></span>
* <span data-ttu-id="29801-1283">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="29801-1283">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="29801-1284">HDInsight</span><span class="sxs-lookup"><span data-stu-id="29801-1284">HDInsight</span></span>
* <span data-ttu-id="29801-1285">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-1285">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="29801-1286">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-1286">IoT</span></span>
* <span data-ttu-id="29801-1287">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="29801-1287">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-1288">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-1288">KeyVault</span></span>
* <span data-ttu-id="29801-1289">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="29801-1289">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="29801-1290">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1290">Network</span></span>
* <span data-ttu-id="29801-1291">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1291">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="29801-1292">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="29801-1292">See #6052</span></span>
* <span data-ttu-id="29801-1293">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1293">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="29801-1294">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="29801-1294">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="29801-1295">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="29801-1295">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="29801-1296">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="29801-1296">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="29801-1297">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="29801-1297">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="29801-1298">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1298">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="29801-1299">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1299">Role</span></span>
* <span data-ttu-id="29801-1300">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="29801-1300">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="29801-1301">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="29801-1301">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="29801-1302">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="29801-1302">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="29801-1303">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="29801-1303">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="29801-1304">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-1304">Service Bus</span></span>
* <span data-ttu-id="29801-1305">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="29801-1305">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1306">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1306">VM</span></span>
* <span data-ttu-id="29801-1307">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="29801-1307">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="29801-1308">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="29801-1308">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="29801-1309">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="29801-1309">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="29801-1310">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="29801-1310">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="29801-1311">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="29801-1311">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="29801-1312">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="29801-1312">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="29801-1313">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1313">September 21, 2018</span></span>

<span data-ttu-id="29801-1314">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="29801-1314">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1315">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1315">ACR</span></span>
* <span data-ttu-id="29801-1316">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-1316">Added ACR Task commands</span></span>
* <span data-ttu-id="29801-1317">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="29801-1317">Added quick run command</span></span>
* <span data-ttu-id="29801-1318">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="29801-1318">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="29801-1319">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-1319">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="29801-1320">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="29801-1320">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="29801-1321">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="29801-1321">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1322">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1322">ACS</span></span>
* <span data-ttu-id="29801-1323">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-1323">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="29801-1324">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="29801-1324">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1325">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1325">AppService</span></span>

* <span data-ttu-id="29801-1326">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="29801-1326">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="29801-1327">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="29801-1327">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="29801-1328">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-1328">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="29801-1329">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="29801-1329">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="29801-1330">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-1330">Batch</span></span>
* <span data-ttu-id="29801-1331">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="29801-1331">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="29801-1332">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="29801-1332">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="29801-1333">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1333">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="29801-1334">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="29801-1334">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="29801-1335">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1335">Batch AI</span></span> 
* <span data-ttu-id="29801-1336">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1336">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="29801-1337">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="29801-1337">Cognitive Services</span></span>
* <span data-ttu-id="29801-1338">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="29801-1338">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="29801-1339">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="29801-1339">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="29801-1340">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="29801-1340">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="29801-1341">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1341">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="29801-1342">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="29801-1342">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="29801-1343">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="29801-1343">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="29801-1344">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1344">Container</span></span>
* <span data-ttu-id="29801-1345">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1345">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="29801-1346">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="29801-1346">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="29801-1347">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="29801-1347">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="29801-1348">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1348">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="29801-1349">Data Lake</span><span class="sxs-lookup"><span data-stu-id="29801-1349">Datalake</span></span>
* <span data-ttu-id="29801-1350">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="29801-1350">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="29801-1351">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="29801-1351">Interactive Shell</span></span>
* <span data-ttu-id="29801-1352">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1352">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="29801-1353">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-1353">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="29801-1354">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-1354">IoT</span></span>
* <span data-ttu-id="29801-1355">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="29801-1355">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-1356">Key Vault</span><span class="sxs-lookup"><span data-stu-id="29801-1356">Key Vault</span></span>
* <span data-ttu-id="29801-1357">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="29801-1357">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="29801-1358">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1358">Network</span></span>
* <span data-ttu-id="29801-1359">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="29801-1359">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="29801-1360">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1360">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="29801-1361">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="29801-1361">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="29801-1362">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="29801-1362">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="29801-1363">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1363">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="29801-1364">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1364">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="29801-1365">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="29801-1365">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="29801-1366">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="29801-1366">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="29801-1367">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="29801-1367">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="29801-1368">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="29801-1368">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="29801-1369">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="29801-1369">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="29801-1370">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="29801-1370">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="29801-1371">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="29801-1371">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="29801-1372">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="29801-1372">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="29801-1373">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="29801-1373">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="29801-1374">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="29801-1374">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="29801-1375">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="29801-1375">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="29801-1376">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="29801-1376">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1377">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-1377">RDBMS</span></span>
* <span data-ttu-id="29801-1378">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="29801-1378">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="29801-1379">резервирование.</span><span class="sxs-lookup"><span data-stu-id="29801-1379">Reservation</span></span>
* <span data-ttu-id="29801-1380">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-1380">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="29801-1381">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="29801-1381">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="29801-1382">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="29801-1382">Manage App</span></span>
* <span data-ttu-id="29801-1383">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="29801-1383">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="29801-1384">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="29801-1384">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="29801-1385">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1385">Role</span></span>
* <span data-ttu-id="29801-1386">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="29801-1386">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="29801-1387">SignalR</span><span class="sxs-lookup"><span data-stu-id="29801-1387">SignalR</span></span>
* <span data-ttu-id="29801-1388">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-1388">First release</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1389">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1389">Storage</span></span>
* <span data-ttu-id="29801-1390">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="29801-1390">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="29801-1391">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="29801-1391">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1392">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1392">VM</span></span>
* <span data-ttu-id="29801-1393">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="29801-1393">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="29801-1394">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="29801-1394">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="29801-1395">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1395">August 28, 2018</span></span>

<span data-ttu-id="29801-1396">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="29801-1396">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="29801-1397">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1397">Core</span></span>

* <span data-ttu-id="29801-1398">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="29801-1398">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="29801-1399">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="29801-1399">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1400">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1400">ACR</span></span>

* <span data-ttu-id="29801-1401">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="29801-1401">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="29801-1402">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="29801-1402">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1403">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1403">ACS</span></span>

* <span data-ttu-id="29801-1404">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="29801-1404">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="29801-1405">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="29801-1405">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1406">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1406">AppService</span></span>

* <span data-ttu-id="29801-1407">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="29801-1407">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="29801-1408">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="29801-1408">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="29801-1409">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1409">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="29801-1410">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-1410">Backup</span></span>

* <span data-ttu-id="29801-1411">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1411">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="29801-1412">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="29801-1412">Bot Service</span></span>

* <span data-ttu-id="29801-1413">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="29801-1413">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="29801-1414">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="29801-1414">Cognitive Services</span></span>

* <span data-ttu-id="29801-1415">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="29801-1415">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="29801-1416">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-1416">IoT</span></span>

* <span data-ttu-id="29801-1417">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="29801-1417">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-1418">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-1418">Monitor</span></span>

* <span data-ttu-id="29801-1419">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="29801-1419">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="29801-1420">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="29801-1420">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="29801-1421">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1421">Network</span></span>

* <span data-ttu-id="29801-1422">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1422">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1423">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1423">Resource</span></span>

* <span data-ttu-id="29801-1424">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1424">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1425">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1425">Storage</span></span>

* <span data-ttu-id="29801-1426">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1426">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1427">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1427">VM</span></span>

* <span data-ttu-id="29801-1428">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29801-1428">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="29801-1429">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1429">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="29801-1430">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1430">Auguest 14, 2018</span></span>

<span data-ttu-id="29801-1431">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="29801-1431">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="29801-1432">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1432">Core</span></span>

* <span data-ttu-id="29801-1433">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="29801-1433">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="29801-1434">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="29801-1434">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="29801-1435">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="29801-1435">Telemetry</span></span>

* <span data-ttu-id="29801-1436">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="29801-1436">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1437">ACR</span></span>

* <span data-ttu-id="29801-1438">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-1438">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="29801-1439">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="29801-1439">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1440">ACS</span></span>

* <span data-ttu-id="29801-1441">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-1441">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="29801-1442">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="29801-1442">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="29801-1443">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="29801-1443">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="29801-1444">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="29801-1444">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="29801-1445">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="29801-1445">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="29801-1446">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1446">AppService</span></span>

* <span data-ttu-id="29801-1447">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-1447">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="29801-1448">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="29801-1448">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-1449">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1449">BatchAI</span></span>

* <span data-ttu-id="29801-1450">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="29801-1450">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="29801-1451">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1451">Container</span></span>

* <span data-ttu-id="29801-1452">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="29801-1452">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="29801-1453">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-1453">IoT</span></span>

* <span data-ttu-id="29801-1454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="29801-1454">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="29801-1455">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="29801-1455">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="29801-1456">IoT Central</span><span class="sxs-lookup"><span data-stu-id="29801-1456">Iot Central</span></span>

* <span data-ttu-id="29801-1457">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="29801-1457">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-1458">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-1458">KeyVault</span></span>


* <span data-ttu-id="29801-1459">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="29801-1459">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="29801-1460">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="29801-1460">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="29801-1461">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="29801-1461">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="29801-1462">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="29801-1462">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="29801-1463">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="29801-1463">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="29801-1464">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="29801-1464">Relay</span></span>

* <span data-ttu-id="29801-1465">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-1465">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1466">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1466">Sql</span></span>

* <span data-ttu-id="29801-1467">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="29801-1467">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1468">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1468">Storage</span></span>

* <span data-ttu-id="29801-1469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="29801-1469">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="29801-1470">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="29801-1470">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="29801-1471">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="29801-1471">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="29801-1472">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="29801-1472">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="29801-1473">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="29801-1473">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1474">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1474">VM</span></span>

* <span data-ttu-id="29801-1475">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="29801-1475">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="29801-1476">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1476">July 31, 2018</span></span>

<span data-ttu-id="29801-1477">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="29801-1477">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1478">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1478">ACR</span></span>

* <span data-ttu-id="29801-1479">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="29801-1479">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="29801-1480">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="29801-1480">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1481">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1481">ACS</span></span>

* <span data-ttu-id="29801-1482">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="29801-1482">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="29801-1483">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-1483">Batch</span></span>

* <span data-ttu-id="29801-1484">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="29801-1484">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="29801-1485">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1485">Container</span></span>

* <span data-ttu-id="29801-1486">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-1486">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="29801-1487">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1487">Network</span></span>

* <span data-ttu-id="29801-1488">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="29801-1488">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="29801-1489">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1489">Resource</span></span>

* <span data-ttu-id="29801-1490">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="29801-1490">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="29801-1491">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="29801-1491">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="29801-1492">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1492">Role</span></span>

* <span data-ttu-id="29801-1493">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="29801-1493">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="29801-1494">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="29801-1494">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="29801-1495">Поиск</span><span class="sxs-lookup"><span data-stu-id="29801-1495">Search</span></span>

* <span data-ttu-id="29801-1496">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="29801-1496">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="29801-1497">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-1497">Service Bus</span></span>

* <span data-ttu-id="29801-1498">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="29801-1498">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="29801-1499">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="29801-1499">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="29801-1500">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="29801-1500">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="29801-1501">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="29801-1501">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1502">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1502">Storage</span></span>

* <span data-ttu-id="29801-1503">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="29801-1503">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="29801-1504">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="29801-1504">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1505">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1505">VM</span></span>

* <span data-ttu-id="29801-1506">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="29801-1506">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="29801-1507">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="29801-1507">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="29801-1508">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="29801-1508">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="29801-1509">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="29801-1509">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="29801-1510">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1510">July 18, 2018</span></span>

<span data-ttu-id="29801-1511">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="29801-1511">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="29801-1512">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1512">Core</span></span>

* <span data-ttu-id="29801-1513">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="29801-1513">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="29801-1514">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="29801-1514">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="29801-1515">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="29801-1515">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1516">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1516">ACR</span></span>

* <span data-ttu-id="29801-1517">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="29801-1517">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="29801-1518">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1518">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="29801-1519">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="29801-1519">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="29801-1520">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="29801-1520">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1521">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1521">ACS</span></span>

* <span data-ttu-id="29801-1522">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="29801-1522">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1523">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1523">AppService</span></span>

* <span data-ttu-id="29801-1524">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="29801-1524">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="29801-1525">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-1525">Batch</span></span>

* <span data-ttu-id="29801-1526">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="29801-1526">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="29801-1527">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="29801-1527">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="29801-1528">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1528">Batch AI</span></span>

* <span data-ttu-id="29801-1529">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="29801-1529">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="29801-1530">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1530">Container</span></span>

* <span data-ttu-id="29801-1531">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="29801-1531">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="29801-1532">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="29801-1532">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="29801-1533">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1533">Network</span></span>

* <span data-ttu-id="29801-1534">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1534">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="29801-1535">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1535">Added `network nic wait`</span></span>
* <span data-ttu-id="29801-1536">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="29801-1536">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="29801-1537">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="29801-1537">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="29801-1538">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1538">Resource</span></span>

* <span data-ttu-id="29801-1539">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1539">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="29801-1540">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1540">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="29801-1541">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1541">Added `deployment wait` command</span></span>
* <span data-ttu-id="29801-1542">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="29801-1542">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1543">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1543">SQL</span></span>

* <span data-ttu-id="29801-1544">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1544">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="29801-1545">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="29801-1545">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="29801-1546">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="29801-1546">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1547">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1547">Storage</span></span>

* <span data-ttu-id="29801-1548">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-1548">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1549">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1549">VM</span></span>

* <span data-ttu-id="29801-1550">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1550">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="29801-1551">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1551">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="29801-1552">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-1552">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="29801-1553">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1553">July 3, 2018</span></span>

<span data-ttu-id="29801-1554">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="29801-1554">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="29801-1555">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-1555">AKS</span></span>

* <span data-ttu-id="29801-1556">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-1556">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="29801-1557">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1557">July 3, 2018</span></span>

<span data-ttu-id="29801-1558">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="29801-1558">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="29801-1559">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1559">Core</span></span>

* <span data-ttu-id="29801-1560">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="29801-1560">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1561">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1561">ACR</span></span>

* <span data-ttu-id="29801-1562">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="29801-1562">Added polling build status</span></span>
* <span data-ttu-id="29801-1563">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="29801-1563">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="29801-1564">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="29801-1564">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1565">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1565">ACS</span></span>

* <span data-ttu-id="29801-1566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1566">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="29801-1567">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1567">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="29801-1568">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="29801-1568">Updated options for `aks browse` command.</span></span> <span data-ttu-id="29801-1569">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="29801-1569">Added `--listen-port` support</span></span>
* <span data-ttu-id="29801-1570">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-1570">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="29801-1571">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="29801-1571">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="29801-1572">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="29801-1572">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1573">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1573">AppService</span></span>

* <span data-ttu-id="29801-1574">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="29801-1574">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="29801-1575">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="29801-1575">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="29801-1576">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-1576">Backup</span></span>

* <span data-ttu-id="29801-1577">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="29801-1577">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-1578">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1578">BatchAI</span></span>

* <span data-ttu-id="29801-1579">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1579">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="29801-1580">Облако</span><span class="sxs-lookup"><span data-stu-id="29801-1580">Cloud</span></span>

* <span data-ttu-id="29801-1581">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="29801-1581">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="29801-1582">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1582">Container</span></span>

* <span data-ttu-id="29801-1583">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="29801-1583">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="29801-1584">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="29801-1584">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="29801-1585">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="29801-1585">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="29801-1586">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-1586">Extension</span></span>

* <span data-ttu-id="29801-1587">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="29801-1587">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="29801-1588">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1588">Network</span></span>

* <span data-ttu-id="29801-1589">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="29801-1589">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1590">Rdbms</span><span class="sxs-lookup"><span data-stu-id="29801-1590">Rdbms</span></span>

* <span data-ttu-id="29801-1591">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-1591">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1592">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1592">Resource</span></span>

* <span data-ttu-id="29801-1593">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="29801-1593">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1594">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1594">VM</span></span>

* <span data-ttu-id="29801-1595">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="29801-1595">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="29801-1596">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1596">June 25, 2018</span></span>

<span data-ttu-id="29801-1597">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="29801-1597">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="29801-1598">CLI</span><span class="sxs-lookup"><span data-stu-id="29801-1598">CLI</span></span>

* <span data-ttu-id="29801-1599">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="29801-1599">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="29801-1600">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1600">June 19, 2018</span></span>

<span data-ttu-id="29801-1601">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="29801-1601">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="29801-1602">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1602">Core</span></span>

* <span data-ttu-id="29801-1603">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1603">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1604">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1604">ACR</span></span>

* <span data-ttu-id="29801-1605">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="29801-1605">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="29801-1606">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="29801-1606">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1607">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1607">ACS</span></span>

* <span data-ttu-id="29801-1608">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="29801-1608">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="29801-1609">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1609">Added `--update` support</span></span>
* <span data-ttu-id="29801-1610">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="29801-1610">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="29801-1611">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="29801-1611">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="29801-1612">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="29801-1612">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="29801-1613">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-1613">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="29801-1614">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-1614">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="29801-1615">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-1615">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1616">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1616">AppService</span></span>

* <span data-ttu-id="29801-1617">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="29801-1617">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="29801-1618">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-1618">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="29801-1619">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-1619">Batch</span></span>

* <span data-ttu-id="29801-1620">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="29801-1620">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="29801-1621">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1621">Batch AI</span></span>

* <span data-ttu-id="29801-1622">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="29801-1622">Added support for workspaces.</span></span> <span data-ttu-id="29801-1623">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-1623">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="29801-1624">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="29801-1624">Added support for experiments.</span></span> <span data-ttu-id="29801-1625">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="29801-1625">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="29801-1626">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="29801-1626">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="29801-1627">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="29801-1627">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="29801-1628">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="29801-1628">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="29801-1629">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="29801-1629">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="29801-1630">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="29801-1630">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="29801-1631">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="29801-1631">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="29801-1632">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1632">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="29801-1633">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="29801-1633">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="29801-1634">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1634">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="29801-1635">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="29801-1635">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="29801-1636">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="29801-1636">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="29801-1637">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="29801-1637">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="29801-1638">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1638">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="29801-1639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="29801-1639">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="29801-1640">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="29801-1640">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="29801-1641">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="29801-1641">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="29801-1642">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="29801-1642">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="29801-1643">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="29801-1643">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="29801-1644">Maps</span><span class="sxs-lookup"><span data-stu-id="29801-1644">Maps</span></span>

* <span data-ttu-id="29801-1645">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="29801-1645">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="29801-1646">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1646">Network</span></span>

* <span data-ttu-id="29801-1647">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="29801-1647">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="29801-1648">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="29801-1648">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="29801-1649">#6502</span><span class="sxs-lookup"><span data-stu-id="29801-1649">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="29801-1650">Резервирование</span><span class="sxs-lookup"><span data-stu-id="29801-1650">Reservations</span></span>

* <span data-ttu-id="29801-1651">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1651">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="29801-1652">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1652">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="29801-1653">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="29801-1653">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="29801-1654">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="29801-1654">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="29801-1655">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="29801-1655">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="29801-1656">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1656">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="29801-1657">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1657">Role</span></span>

* <span data-ttu-id="29801-1658">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="29801-1658">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1659">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1659">SQL</span></span>

* <span data-ttu-id="29801-1660">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-1660">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1661">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1661">Storage</span></span>

* <span data-ttu-id="29801-1662">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="29801-1662">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1663">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1663">VM</span></span>

* <span data-ttu-id="29801-1664">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1664">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="29801-1665">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="29801-1665">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="29801-1666">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="29801-1666">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="29801-1667">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1667">June 13, 2018</span></span>

<span data-ttu-id="29801-1668">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="29801-1668">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="29801-1669">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1669">Core</span></span>

* <span data-ttu-id="29801-1670">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="29801-1670">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="29801-1671">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1671">June 13, 2018</span></span>

<span data-ttu-id="29801-1672">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="29801-1672">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="29801-1673">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-1673">AKS</span></span>

* <span data-ttu-id="29801-1674">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="29801-1674">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="29801-1675">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="29801-1675">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="29801-1676">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="29801-1676">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="29801-1677">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="29801-1677">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="29801-1678">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="29801-1678">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1679">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1679">AppService</span></span>

* <span data-ttu-id="29801-1680">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="29801-1680">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="29801-1681">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1681">June 5, 2018</span></span>

<span data-ttu-id="29801-1682">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="29801-1682">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1683">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1683">Interactive</span></span>

* <span data-ttu-id="29801-1684">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="29801-1684">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="29801-1685">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1685">June 5, 2018</span></span>

<span data-ttu-id="29801-1686">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="29801-1686">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="29801-1687">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1687">Core</span></span>

* <span data-ttu-id="29801-1688">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="29801-1688">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="29801-1689">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="29801-1689">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1690">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1690">ACR</span></span>

* <span data-ttu-id="29801-1691">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="29801-1691">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="29801-1692">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="29801-1692">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="29801-1693">AKS</span><span class="sxs-lookup"><span data-stu-id="29801-1693">AKS</span></span>

* <span data-ttu-id="29801-1694">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="29801-1694">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="29801-1695">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-1695">Batch</span></span>

* <span data-ttu-id="29801-1696">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="29801-1696">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="29801-1697">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-1697">IOT</span></span>

* <span data-ttu-id="29801-1698">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="29801-1698">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="29801-1699">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1699">Network</span></span>

* <span data-ttu-id="29801-1700">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="29801-1700">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="29801-1701">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="29801-1701">Policy Insights</span></span>

* <span data-ttu-id="29801-1702">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-1702">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="29801-1703">ARM</span><span class="sxs-lookup"><span data-stu-id="29801-1703">ARM</span></span>

* <span data-ttu-id="29801-1704">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="29801-1704">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1705">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1705">SQL</span></span>

* <span data-ttu-id="29801-1706">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="29801-1706">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="29801-1707">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="29801-1707">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="29801-1708">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1708">Storage</span></span>

* <span data-ttu-id="29801-1709">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="29801-1709">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1710">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1710">VM</span></span>

* <span data-ttu-id="29801-1711">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="29801-1711">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="29801-1712">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1712">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="29801-1713">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1713">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="29801-1714">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1714">May 22, 2018</span></span>

<span data-ttu-id="29801-1715">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="29801-1715">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="29801-1716">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1716">Core</span></span>

* <span data-ttu-id="29801-1717">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="29801-1717">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1718">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1718">ACS</span></span>

* <span data-ttu-id="29801-1719">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="29801-1719">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="29801-1720">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="29801-1720">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1721">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-1721">AppService</span></span>

* <span data-ttu-id="29801-1722">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="29801-1722">Improved generic update commands</span></span>
* <span data-ttu-id="29801-1723">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="29801-1723">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="29801-1724">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1724">Container</span></span>

* <span data-ttu-id="29801-1725">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="29801-1725">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="29801-1726">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1726">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="29801-1727">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-1727">Extension</span></span>

* <span data-ttu-id="29801-1728">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="29801-1728">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1729">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1729">Interactive</span></span>

* <span data-ttu-id="29801-1730">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="29801-1730">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="29801-1731">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="29801-1731">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-1732">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-1732">KeyVault</span></span>

* <span data-ttu-id="29801-1733">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="29801-1733">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="29801-1734">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1734">Network</span></span>

* <span data-ttu-id="29801-1735">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="29801-1735">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="29801-1736">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="29801-1736">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1737">SQL</span></span>

* <span data-ttu-id="29801-1738">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="29801-1738">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="29801-1739">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="29801-1739">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="29801-1740">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="29801-1740">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="29801-1741">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="29801-1741">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="29801-1742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="29801-1742">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="29801-1743">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="29801-1743">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="29801-1744">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="29801-1744">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="29801-1745">`edition`.</span><span class="sxs-lookup"><span data-stu-id="29801-1745">`edition`.</span></span> <span data-ttu-id="29801-1746">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="29801-1746">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="29801-1747">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="29801-1747">`elasticPoolName`.</span></span> <span data-ttu-id="29801-1748">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="29801-1748">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="29801-1749">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="29801-1749">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="29801-1750">`edition`.</span><span class="sxs-lookup"><span data-stu-id="29801-1750">`edition`.</span></span> <span data-ttu-id="29801-1751">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="29801-1751">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="29801-1752">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="29801-1752">`dtu`.</span></span> <span data-ttu-id="29801-1753">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="29801-1753">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="29801-1754">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="29801-1754">`databaseDtuMin`.</span></span> <span data-ttu-id="29801-1755">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="29801-1755">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="29801-1756">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="29801-1756">`databaseDtuMax`.</span></span> <span data-ttu-id="29801-1757">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="29801-1757">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="29801-1758">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="29801-1758">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="29801-1759">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="29801-1759">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1760">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1760">Storage</span></span>

* <span data-ttu-id="29801-1761">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-1761">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="29801-1762">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="29801-1762">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1763">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1763">VM</span></span>

* <span data-ttu-id="29801-1764">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1764">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="29801-1765">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="29801-1765">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="29801-1766">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="29801-1766">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="29801-1767">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="29801-1767">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="29801-1768">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1768">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="29801-1769">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1769">May 7, 2018</span></span>

<span data-ttu-id="29801-1770">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="29801-1770">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="29801-1771">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1771">Core</span></span>

* <span data-ttu-id="29801-1772">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="29801-1772">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="29801-1773">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="29801-1773">Added limited support for positional arguments</span></span>
* <span data-ttu-id="29801-1774">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-1774">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="29801-1775">#5591</span><span class="sxs-lookup"><span data-stu-id="29801-1775">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="29801-1776">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-1776">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="29801-1777">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="29801-1777">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="29801-1778">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="29801-1778">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="29801-1779">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="29801-1779">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="29801-1780">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="29801-1780">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1781">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1781">ACR</span></span>

* <span data-ttu-id="29801-1782">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-1782">Added ACR Build commands</span></span>
* <span data-ttu-id="29801-1783">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="29801-1783">Improved resource not found error messages</span></span>
* <span data-ttu-id="29801-1784">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="29801-1784">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="29801-1785">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="29801-1785">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="29801-1786">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="29801-1786">Improved repository commands error messages</span></span>
* <span data-ttu-id="29801-1787">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="29801-1787">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1788">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1788">ACS</span></span>

* <span data-ttu-id="29801-1789">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="29801-1789">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="29801-1790">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="29801-1790">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="29801-1791">AMS</span><span class="sxs-lookup"><span data-stu-id="29801-1791">AMS</span></span>

* <span data-ttu-id="29801-1792">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-1792">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1793">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1793">Appservice</span></span>

* <span data-ttu-id="29801-1794">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="29801-1794">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="29801-1795">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1795">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="29801-1796">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="29801-1796">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="29801-1797">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1797">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="29801-1798">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1798">Batch AI</span></span>

* <span data-ttu-id="29801-1799">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="29801-1799">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="29801-1800">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="29801-1800">Cognitive Services</span></span>

* <span data-ttu-id="29801-1801">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="29801-1801">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-1802">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-1802">Consumption</span></span>

* <span data-ttu-id="29801-1803">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="29801-1803">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="29801-1804">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1804">Container</span></span>

* <span data-ttu-id="29801-1805">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="29801-1805">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="29801-1806">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-1806">Cosmos DB</span></span>

* <span data-ttu-id="29801-1807">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-1807">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="29801-1808">DMS</span><span class="sxs-lookup"><span data-stu-id="29801-1808">DMS</span></span>

* <span data-ttu-id="29801-1809">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="29801-1809">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="29801-1810">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-1810">Extension</span></span>

* <span data-ttu-id="29801-1811">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="29801-1811">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1812">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1812">Interactive</span></span>

* <span data-ttu-id="29801-1813">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="29801-1813">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="29801-1814">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="29801-1814">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="29801-1815">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="29801-1815">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="29801-1816">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1816">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="29801-1817">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="29801-1817">Lab</span></span>

* <span data-ttu-id="29801-1818">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="29801-1818">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="29801-1819">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1819">Network</span></span>

* <span data-ttu-id="29801-1820">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="29801-1820">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="29801-1821">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-1821">Profile</span></span>

* <span data-ttu-id="29801-1822">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1822">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="29801-1823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="29801-1823">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="29801-1824">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="29801-1824">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="29801-1825">Redis</span><span class="sxs-lookup"><span data-stu-id="29801-1825">Redis</span></span>

* <span data-ttu-id="29801-1826">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1826">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="29801-1827">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="29801-1827">Deprecated `redis list-all`.</span></span> <span data-ttu-id="29801-1828">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1828">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="29801-1829">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="29801-1829">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="29801-1830">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1830">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="29801-1831">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1831">Role</span></span>

* <span data-ttu-id="29801-1832">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="29801-1832">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1833">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1833">Storage</span></span>

* <span data-ttu-id="29801-1834">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="29801-1834">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="29801-1835">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="29801-1835">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="29801-1836">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="29801-1836">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="29801-1837">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="29801-1837">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="29801-1838">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="29801-1838">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1839">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1839">VM</span></span>

* <span data-ttu-id="29801-1840">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="29801-1840">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="29801-1841">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="29801-1841">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="29801-1842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="29801-1842">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="29801-1843">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="29801-1843">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="29801-1844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="29801-1844">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="29801-1845">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="29801-1845">Added write accelerator support</span></span>
* <span data-ttu-id="29801-1846">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="29801-1846">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="29801-1847">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="29801-1847">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="29801-1848">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="29801-1848">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="29801-1849">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1849">April 10, 2018</span></span>

<span data-ttu-id="29801-1850">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="29801-1850">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1851">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1851">ACR</span></span>

* <span data-ttu-id="29801-1852">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="29801-1852">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1853">ACS</span></span>

* <span data-ttu-id="29801-1854">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="29801-1854">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1855">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1855">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="29801-1857">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-1857">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-1858">Batch AI</span><span class="sxs-lookup"><span data-stu-id="29801-1858">BatchAI</span></span>

* <span data-ttu-id="29801-1859">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="29801-1859">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="29801-1860">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="29801-1860">Job level mounting</span></span>
  - <span data-ttu-id="29801-1861">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="29801-1861">Environment variables with secret values</span></span>
  - <span data-ttu-id="29801-1862">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="29801-1862">Performance counters settings</span></span>
  - <span data-ttu-id="29801-1863">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="29801-1863">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="29801-1864">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="29801-1864">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="29801-1865">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="29801-1865">Usage and limits reporting</span></span>
  - <span data-ttu-id="29801-1866">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="29801-1866">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="29801-1867">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="29801-1867">Support for custom images</span></span>
  - <span data-ttu-id="29801-1868">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="29801-1868">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="29801-1869">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="29801-1869">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="29801-1870">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="29801-1870">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="29801-1871">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="29801-1871">National clouds are supported</span></span>
* <span data-ttu-id="29801-1872">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="29801-1872">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="29801-1873">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="29801-1873">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="29801-1874">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="29801-1874">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="29801-1875">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="29801-1875">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="29801-1876">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="29801-1876">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="29801-1877">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="29801-1877">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="29801-1878">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1878">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="29801-1879">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="29801-1879">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="29801-1880">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="29801-1880">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="29801-1881">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1881">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="29801-1882">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="29801-1882">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="29801-1883">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="29801-1883">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="29801-1884">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1884">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="29801-1885">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="29801-1885">Billing</span></span>

* <span data-ttu-id="29801-1886">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="29801-1886">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-1887">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-1887">Consumption</span></span>

* <span data-ttu-id="29801-1888">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="29801-1888">Added `marketplace` commands</span></span>
* <span data-ttu-id="29801-1889">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="29801-1889">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="29801-1890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="29801-1890">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="29801-1891">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="29801-1891">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="29801-1892">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="29801-1892">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="29801-1893">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="29801-1893">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="29801-1894">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1894">Container</span></span>

* <span data-ttu-id="29801-1895">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="29801-1895">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="29801-1896">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="29801-1896">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="29801-1897">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-1897">Extension</span></span>

* <span data-ttu-id="29801-1898">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="29801-1898">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1899">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1899">Interactive</span></span>

* <span data-ttu-id="29801-1900">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="29801-1900">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="29801-1901">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1901">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="29801-1902">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="29801-1902">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="29801-1903">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1903">Network</span></span>

* <span data-ttu-id="29801-1904">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1904">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="29801-1905">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1905">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="29801-1906">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="29801-1906">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="29801-1907">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="29801-1907">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="29801-1908">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="29801-1908">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="29801-1909">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1909">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="29801-1910">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1910">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="29801-1911">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="29801-1911">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-1912">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-1912">Profile</span></span>

* <span data-ttu-id="29801-1913">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1913">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="29801-1914">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="29801-1914">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1915">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-1915">RDBMS</span></span>

* <span data-ttu-id="29801-1916">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="29801-1916">Added `georestore` command</span></span>
* <span data-ttu-id="29801-1917">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="29801-1917">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1918">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1918">Resource</span></span>

* <span data-ttu-id="29801-1919">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1919">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="29801-1920">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1920">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="29801-1921">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-1921">SQL</span></span>

* <span data-ttu-id="29801-1922">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="29801-1922">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1923">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1923">Storage</span></span>

* <span data-ttu-id="29801-1924">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="29801-1924">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1925">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1925">VM</span></span>

* <span data-ttu-id="29801-1926">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="29801-1926">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="29801-1927">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="29801-1927">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="29801-1929">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1929">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="29801-1930">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="29801-1930">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="29801-1931">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="29801-1931">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="29801-1932">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="29801-1932">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="29801-1933">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1933">March 27, 2018</span></span>

<span data-ttu-id="29801-1934">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="29801-1934">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="29801-1935">Core</span><span class="sxs-lookup"><span data-stu-id="29801-1935">Core</span></span>

* <span data-ttu-id="29801-1936">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="29801-1936">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1937">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1937">ACS</span></span>

* <span data-ttu-id="29801-1938">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="29801-1938">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-1939">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-1939">Appservice</span></span>

* <span data-ttu-id="29801-1940">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1940">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="29801-1941">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1941">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="29801-1942">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-1942">Backup</span></span>

* <span data-ttu-id="29801-1943">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="29801-1943">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="29801-1944">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="29801-1944">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="29801-1945">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="29801-1945">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="29801-1946">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="29801-1946">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="29801-1947">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-1947">Container</span></span>

* <span data-ttu-id="29801-1948">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="29801-1948">Added `container exec` command.</span></span> <span data-ttu-id="29801-1949">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1949">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="29801-1950">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-1950">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="29801-1951">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-1951">Extension</span></span>

* <span data-ttu-id="29801-1952">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="29801-1952">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="29801-1953">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="29801-1953">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="29801-1954">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-1954">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-1955">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-1955">Interactive</span></span>

* <span data-ttu-id="29801-1956">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1956">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="29801-1957">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="29801-1957">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="29801-1958">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="29801-1958">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="29801-1959">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="29801-1959">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="29801-1960">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="29801-1960">Lab</span></span>

* <span data-ttu-id="29801-1961">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="29801-1961">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-1962">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-1962">Monitor</span></span>

* <span data-ttu-id="29801-1963">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="29801-1963">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="29801-1964">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="29801-1964">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="29801-1965">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="29801-1965">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="29801-1966">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-1966">Network</span></span>

* <span data-ttu-id="29801-1967">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="29801-1967">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="29801-1968">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-1968">Profile</span></span>

* <span data-ttu-id="29801-1969">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="29801-1969">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-1970">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-1970">RDBMS</span></span>

* <span data-ttu-id="29801-1971">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="29801-1971">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="29801-1972">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-1972">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="29801-1974">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-1974">Role</span></span>

* <span data-ttu-id="29801-1975">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="29801-1975">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="29801-1976">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="29801-1976">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="29801-1977">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="29801-1977">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="29801-1978">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1978">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="29801-1979">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="29801-1979">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-1980">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-1980">Storage</span></span>

* <span data-ttu-id="29801-1981">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="29801-1981">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="29801-1982">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="29801-1982">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="29801-1983">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-1983">VM</span></span>

* <span data-ttu-id="29801-1984">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="29801-1984">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="29801-1985">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="29801-1985">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="29801-1986">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="29801-1986">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="29801-1987">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="29801-1987">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="29801-1988">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-1988">March 13, 2018</span></span>

<span data-ttu-id="29801-1989">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="29801-1989">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="29801-1990">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-1990">ACR</span></span>

* <span data-ttu-id="29801-1991">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="29801-1991">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="29801-1992">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="29801-1992">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="29801-1993">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="29801-1993">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="29801-1994">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-1994">ACS</span></span>

* <span data-ttu-id="29801-1995">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="29801-1995">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="29801-1996">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="29801-1996">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="29801-1997">Помощник</span><span class="sxs-lookup"><span data-stu-id="29801-1997">Advisor</span></span>

* <span data-ttu-id="29801-1998">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="29801-1998">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="29801-1999">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="29801-1999">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="29801-2000">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="29801-2000">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="29801-2001">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="29801-2001">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="29801-2002">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2002">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2003">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2003">Appservice</span></span>

* <span data-ttu-id="29801-2004">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="29801-2004">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="29801-2005">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2005">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="29801-2006">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="29801-2006">Eventhubs</span></span>

* <span data-ttu-id="29801-2007">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-2007">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="29801-2008">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-2008">Extension</span></span>

* <span data-ttu-id="29801-2009">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="29801-2009">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-2010">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-2010">Interactive</span></span>

* <span data-ttu-id="29801-2011">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="29801-2011">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="29801-2012">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="29801-2012">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="29801-2013">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="29801-2013">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="29801-2014">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="29801-2014">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2015">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2015">Monitor</span></span>

* <span data-ttu-id="29801-2016">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="29801-2016">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="29801-2017">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="29801-2017">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="29801-2018">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="29801-2018">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="29801-2019">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-2019">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="29801-2020">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2020">Network</span></span>

* <span data-ttu-id="29801-2021">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2021">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="29801-2022">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="29801-2022">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="29801-2023">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="29801-2023">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="29801-2024">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="29801-2024">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2025">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2025">Profile</span></span>

* <span data-ttu-id="29801-2026">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="29801-2026">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="29801-2027">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="29801-2027">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-2028">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-2028">RDBMS</span></span>

* <span data-ttu-id="29801-2029">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="29801-2029">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="29801-2030">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="29801-2030">Service Bus</span></span>

* <span data-ttu-id="29801-2031">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-2031">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2032">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2032">Storage</span></span>

* <span data-ttu-id="29801-2033">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="29801-2033">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="29801-2034">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="29801-2034">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2035">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2035">VM</span></span>

* <span data-ttu-id="29801-2036">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="29801-2036">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="29801-2037">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="29801-2037">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="29801-2038">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2038">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="29801-2039">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="29801-2039">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="29801-2040">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="29801-2040">February 27, 2018</span></span>

<span data-ttu-id="29801-2041">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="29801-2041">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="29801-2042">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2042">Core</span></span>

* <span data-ttu-id="29801-2043">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="29801-2043">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="29801-2044">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="29801-2044">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="29801-2045">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="29801-2045">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2046">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2046">ACS</span></span>

* <span data-ttu-id="29801-2047">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2047">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="29801-2048">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="29801-2048">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="29801-2049">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-2049">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="29801-2050">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="29801-2050">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2051">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2051">Appservice</span></span>

* <span data-ttu-id="29801-2052">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="29801-2052">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="29801-2053">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="29801-2053">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="29801-2054">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="29801-2054">Cognitive Services</span></span>

* <span data-ttu-id="29801-2055">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="29801-2055">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-2056">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-2056">Consumption</span></span>

* <span data-ttu-id="29801-2057">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="29801-2057">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="29801-2058">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="29801-2058">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="29801-2059">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2059">Container</span></span>

* <span data-ttu-id="29801-2060">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="29801-2060">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="29801-2061">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2061">Network</span></span>

* <span data-ttu-id="29801-2062">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="29801-2062">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2063">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2063">Resource</span></span>

* <span data-ttu-id="29801-2064">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="29801-2064">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="29801-2065">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2065">Role</span></span>

* <span data-ttu-id="29801-2066">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="29801-2066">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2067">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2067">SQL</span></span>

* <span data-ttu-id="29801-2068">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="29801-2068">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2069">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2069">Storage</span></span>

* <span data-ttu-id="29801-2070">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2070">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2071">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2071">VM</span></span>

* <span data-ttu-id="29801-2072">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="29801-2072">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="29801-2073">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2073">February 13, 2018</span></span>

<span data-ttu-id="29801-2074">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="29801-2074">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="29801-2075">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2075">Core</span></span>

* <span data-ttu-id="29801-2076">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="29801-2076">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2077">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2077">ACS</span></span>

* <span data-ttu-id="29801-2078">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="29801-2078">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="29801-2079">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2079">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="29801-2080">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="29801-2080">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="29801-2081">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="29801-2081">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="29801-2082">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="29801-2082">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="29801-2083">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="29801-2083">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="29801-2084">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="29801-2084">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="29801-2085">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="29801-2085">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2086">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2086">Appservice</span></span>

* <span data-ttu-id="29801-2087">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="29801-2087">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="29801-2088">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="29801-2088">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-2089">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-2089">CDN</span></span>

* <span data-ttu-id="29801-2090">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2090">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="29801-2091">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2091">Container</span></span>

* <span data-ttu-id="29801-2092">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="29801-2092">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="29801-2093">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-2093">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-2094">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-2094">CosmosDB</span></span>

* <span data-ttu-id="29801-2095">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="29801-2095">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="29801-2096">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-2096">Extension</span></span>

* <span data-ttu-id="29801-2097">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2097">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="29801-2098">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2098">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="29801-2099">Отзыв</span><span class="sxs-lookup"><span data-stu-id="29801-2099">Feedback</span></span>

* <span data-ttu-id="29801-2100">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="29801-2100">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-2101">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-2101">Interactive</span></span>

* <span data-ttu-id="29801-2102">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="29801-2102">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="29801-2103">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="29801-2103">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="29801-2104">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-2104">IoT</span></span>

* <span data-ttu-id="29801-2105">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="29801-2105">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="29801-2106">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="29801-2106">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="29801-2107">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2107">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="29801-2108">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="29801-2108">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2109">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2109">Monitor</span></span>

* <span data-ttu-id="29801-2110">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2110">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="29801-2111">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2111">Network</span></span>

* <span data-ttu-id="29801-2112">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="29801-2112">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="29801-2113">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2113">Profile</span></span>

* <span data-ttu-id="29801-2114">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="29801-2114">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2115">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2115">Resource</span></span>

* <span data-ttu-id="29801-2116">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2116">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="29801-2117">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2117">Role</span></span>

* <span data-ttu-id="29801-2118">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="29801-2118">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2119">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2119">SQL</span></span>

* <span data-ttu-id="29801-2120">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="29801-2120">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="29801-2121">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="29801-2121">Added `sql db rename`</span></span>
* <span data-ttu-id="29801-2122">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="29801-2122">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2123">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2123">Storage</span></span>

* <span data-ttu-id="29801-2124">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="29801-2124">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2125">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2125">VM</span></span>

* <span data-ttu-id="29801-2126">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="29801-2126">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="29801-2127">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="29801-2127">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="29801-2128">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="29801-2128">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="29801-2129">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2129">January 31, 2018</span></span>

<span data-ttu-id="29801-2130">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="29801-2130">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="29801-2131">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2131">Core</span></span>

* <span data-ttu-id="29801-2132">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="29801-2132">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="29801-2133">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-2133">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="29801-2134">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="29801-2134">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="29801-2135">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="29801-2135">Use `--verbose` to see</span></span>
* <span data-ttu-id="29801-2136">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="29801-2136">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2137">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2137">ACS</span></span>

* <span data-ttu-id="29801-2138">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="29801-2138">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="29801-2139">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="29801-2139">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2140">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2140">Appservice</span></span>

* <span data-ttu-id="29801-2141">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="29801-2141">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="29801-2142">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="29801-2142">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-2143">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-2143">CDN</span></span>

* <span data-ttu-id="29801-2144">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2144">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-2145">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-2145">CosmosDB</span></span>

* <span data-ttu-id="29801-2146">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="29801-2146">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-2147">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-2147">Interactive</span></span>

* <span data-ttu-id="29801-2148">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="29801-2148">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="29801-2149">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2149">Network</span></span>

* <span data-ttu-id="29801-2150">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2150">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="29801-2151">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2151">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="29801-2152">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2152">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="29801-2153">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2153">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="29801-2154">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="29801-2154">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="29801-2155">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="29801-2155">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="29801-2156">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="29801-2156">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="29801-2157">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="29801-2157">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="29801-2158">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="29801-2158">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="29801-2159">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="29801-2159">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2160">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2160">Profile</span></span>

* <span data-ttu-id="29801-2161">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="29801-2161">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2162">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2162">Resource</span></span>

* <span data-ttu-id="29801-2163">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="29801-2163">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2164">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2164">Storage</span></span>

* <span data-ttu-id="29801-2165">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="29801-2165">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="29801-2166">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="29801-2166">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="29801-2167">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-2167">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="29801-2168">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2168">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="29801-2169">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="29801-2169">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2170">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2170">VM</span></span>

* <span data-ttu-id="29801-2171">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="29801-2171">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="29801-2172">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-2172">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="29801-2173">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="29801-2173">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="29801-2174">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2174">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="29801-2175">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2175">January 17, 2018</span></span>

<span data-ttu-id="29801-2176">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="29801-2176">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="29801-2177">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-2177">ACR</span></span>

* <span data-ttu-id="29801-2178">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-2178">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="29801-2179">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="29801-2179">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2180">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2180">ACS</span></span>

* <span data-ttu-id="29801-2181">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="29801-2181">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="29801-2182">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="29801-2182">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2183">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2183">Appservice</span></span>

* <span data-ttu-id="29801-2184">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="29801-2184">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="29801-2185">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="29801-2185">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="29801-2186">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="29801-2186">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="29801-2187">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-2187">Backup</span></span>

* <span data-ttu-id="29801-2188">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="29801-2188">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="29801-2189">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="29801-2189">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="29801-2190">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="29801-2190">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="29801-2191">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="29801-2191">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="29801-2192">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="29801-2192">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="29801-2193">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2193">Batch</span></span>

* <span data-ttu-id="29801-2194">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="29801-2194">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="29801-2195">Облако</span><span class="sxs-lookup"><span data-stu-id="29801-2195">Cloud</span></span>

* <span data-ttu-id="29801-2196">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="29801-2196">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-2197">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-2197">Consumption</span></span>

* <span data-ttu-id="29801-2198">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="29801-2198">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="29801-2199">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2199">Event Grid</span></span>

* <span data-ttu-id="29801-2200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="29801-2200">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="29801-2201">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="29801-2201">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="29801-2202">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="29801-2202">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="29801-2203">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="29801-2203">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="29801-2204">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2204">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="29801-2205">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2205">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="29801-2206">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="29801-2206">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="29801-2207">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="29801-2207">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-2208">Interactive</span><span class="sxs-lookup"><span data-stu-id="29801-2208">Interactive</span></span>

* <span data-ttu-id="29801-2209">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="29801-2209">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="29801-2210">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="29801-2210">Fixed errors on startup</span></span>
* <span data-ttu-id="29801-2211">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="29801-2211">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="29801-2212">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-2212">IoT</span></span>

* <span data-ttu-id="29801-2213">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="29801-2213">Added support for device provisioning service</span></span>
* <span data-ttu-id="29801-2214">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="29801-2214">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="29801-2215">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="29801-2215">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2216">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2216">Monitor</span></span>

* <span data-ttu-id="29801-2217">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="29801-2217">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="29801-2218">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2218">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="29801-2219">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="29801-2219">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="29801-2220">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2220">Network</span></span>

* <span data-ttu-id="29801-2221">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="29801-2221">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="29801-2222">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="29801-2222">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2223">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2223">Profile</span></span>

* <span data-ttu-id="29801-2224">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29801-2224">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="29801-2225">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2225">Role</span></span>

* <span data-ttu-id="29801-2226">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="29801-2226">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="29801-2227">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-2227">Service Fabric</span></span>

* <span data-ttu-id="29801-2228">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="29801-2228">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="29801-2229">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="29801-2229">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2230">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2230">VM</span></span>

* <span data-ttu-id="29801-2231">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="29801-2231">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="29801-2232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="29801-2232">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="29801-2233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="29801-2233">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="29801-2234">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="29801-2234">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="29801-2235">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="29801-2235">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="29801-2236">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="29801-2236">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="29801-2237">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2237">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="29801-2238">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="29801-2238">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="29801-2239">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2239">December 19, 2017</span></span>

<span data-ttu-id="29801-2240">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="29801-2240">Version 2.0.23</span></span>

* <span data-ttu-id="29801-2241">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="29801-2241">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="29801-2242">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2242">Container</span></span>

* <span data-ttu-id="29801-2243">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-2243">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="29801-2244">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2244">Network</span></span>

* <span data-ttu-id="29801-2245">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2245">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="29801-2246">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2246">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2247">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2247">Storage</span></span>

* <span data-ttu-id="29801-2248">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="29801-2248">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2249">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2249">VM</span></span>

* <span data-ttu-id="29801-2250">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="29801-2250">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="29801-2251">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2251">December 5, 2017</span></span>

<span data-ttu-id="29801-2252">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="29801-2252">Version 2.0.22</span></span>

* <span data-ttu-id="29801-2253">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="29801-2253">Removed `az component` commands.</span></span> <span data-ttu-id="29801-2254">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="29801-2254">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="29801-2255">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2255">Core</span></span>
* <span data-ttu-id="29801-2256">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="29801-2256">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="29801-2257">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="29801-2257">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2258">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2258">ACS</span></span>

* <span data-ttu-id="29801-2259">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="29801-2259">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="29801-2260">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2260">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="29801-2261">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="29801-2261">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="29801-2262">Помощник</span><span class="sxs-lookup"><span data-stu-id="29801-2262">Advisor</span></span>

* <span data-ttu-id="29801-2263">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-2263">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2264">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2264">Appservice</span></span>

* <span data-ttu-id="29801-2265">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="29801-2265">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="29801-2266">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-2266">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="29801-2267">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="29801-2267">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="29801-2268">Потребление</span><span class="sxs-lookup"><span data-stu-id="29801-2268">Consumption</span></span>

* <span data-ttu-id="29801-2269">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="29801-2269">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="29801-2270">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2270">Container</span></span>

* <span data-ttu-id="29801-2271">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="29801-2271">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2272">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2272">Monitor</span></span>

* <span data-ttu-id="29801-2273">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="29801-2273">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2274">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2274">Resource</span></span>

* <span data-ttu-id="29801-2275">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="29801-2275">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="29801-2276">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2276">Role</span></span>

* <span data-ttu-id="29801-2277">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="29801-2277">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="29801-2278">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="29801-2278">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="29801-2279">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="29801-2279">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2280">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2280">SQL</span></span>

* <span data-ttu-id="29801-2281">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="29801-2281">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="29801-2282">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2282">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2283">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2283">VM</span></span>

* <span data-ttu-id="29801-2284">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="29801-2284">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="29801-2285">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2285">November 14, 2017</span></span>

<span data-ttu-id="29801-2286">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="29801-2286">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="29801-2287">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-2287">ACR</span></span>

* <span data-ttu-id="29801-2288">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="29801-2288">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="29801-2289">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2289">ACS</span></span>

* <span data-ttu-id="29801-2290">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="29801-2290">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="29801-2291">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="29801-2291">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="29801-2292">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="29801-2292">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="29801-2293">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-2293">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="29801-2294">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-2294">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2295">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2295">Appservice</span></span>

* <span data-ttu-id="29801-2296">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="29801-2296">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="29801-2297">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="29801-2297">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="29801-2298">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="29801-2298">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="29801-2299">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="29801-2299">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="29801-2300">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="29801-2300">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="29801-2301">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="29801-2301">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="29801-2302">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2302">Batch</span></span>

* <span data-ttu-id="29801-2303">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="29801-2303">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-2304">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="29801-2304">Batchai</span></span>

* <span data-ttu-id="29801-2305">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2305">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="29801-2306">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2306">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="29801-2307">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="29801-2307">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="29801-2308">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2308">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="29801-2309">Облако</span><span class="sxs-lookup"><span data-stu-id="29801-2309">Cloud</span></span>

* <span data-ttu-id="29801-2310">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="29801-2310">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="29801-2311">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2311">Container</span></span>

* <span data-ttu-id="29801-2312">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="29801-2312">Added support to open multiple ports</span></span>
* <span data-ttu-id="29801-2313">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-2313">Added container group restart policy</span></span>
* <span data-ttu-id="29801-2314">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="29801-2314">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="29801-2315">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="29801-2315">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="29801-2316">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="29801-2316">Data Lake Analytics</span></span>

* <span data-ttu-id="29801-2317">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="29801-2317">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="29801-2318">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="29801-2318">Data Lake Store</span></span>

* <span data-ttu-id="29801-2319">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="29801-2319">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="29801-2320">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-2320">Extension</span></span>

* <span data-ttu-id="29801-2321">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="29801-2321">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="29801-2322">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="29801-2322">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="29801-2323">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-2323">IoT</span></span>

* <span data-ttu-id="29801-2324">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-2324">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2325">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2325">Monitor</span></span>

* <span data-ttu-id="29801-2326">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="29801-2326">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="29801-2327">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2327">Network</span></span>

* <span data-ttu-id="29801-2328">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="29801-2328">Added support for CAA DNS records</span></span>
* <span data-ttu-id="29801-2329">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2329">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="29801-2330">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="29801-2330">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="29801-2331">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="29801-2331">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="29801-2332">Резервирование</span><span class="sxs-lookup"><span data-stu-id="29801-2332">Reservations</span></span>

* <span data-ttu-id="29801-2333">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="29801-2333">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2334">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2334">Resource</span></span>

* <span data-ttu-id="29801-2335">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="29801-2335">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2336">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2336">SQL</span></span>

* <span data-ttu-id="29801-2337">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2337">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2338">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2338">Storage</span></span>

* <span data-ttu-id="29801-2339">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2339">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="29801-2340">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="29801-2340">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="29801-2341">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="29801-2341">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="29801-2342">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="29801-2342">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="29801-2343">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2343">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="29801-2344">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="29801-2344">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="29801-2345">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2345">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2346">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2346">VM</span></span>

* <span data-ttu-id="29801-2347">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="29801-2347">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="29801-2348">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="29801-2348">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="29801-2349">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="29801-2349">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="29801-2350">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="29801-2350">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="29801-2351">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="29801-2351">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="29801-2352">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2352">October 24, 2017</span></span>

<span data-ttu-id="29801-2353">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="29801-2353">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="29801-2354">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2354">Core</span></span>

* <span data-ttu-id="29801-2355">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="29801-2355">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="29801-2356">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-2356">ACR</span></span>

* <span data-ttu-id="29801-2357">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="29801-2357">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="29801-2358">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="29801-2358">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="29801-2359">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="29801-2359">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2360">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2360">ACS</span></span>

* <span data-ttu-id="29801-2361">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="29801-2361">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="29801-2362">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="29801-2362">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2363">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2363">Appservice</span></span>

* <span data-ttu-id="29801-2364">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="29801-2364">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="29801-2365">Компонент</span><span class="sxs-lookup"><span data-stu-id="29801-2365">Component</span></span>

* <span data-ttu-id="29801-2366">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="29801-2366">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2367">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2367">Monitor</span></span>

* <span data-ttu-id="29801-2368">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="29801-2368">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2369">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2369">Resource</span></span>

* <span data-ttu-id="29801-2370">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="29801-2370">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="29801-2371">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="29801-2371">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2372">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2372">VM</span></span>

* <span data-ttu-id="29801-2373">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="29801-2373">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="29801-2374">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2374">October 9, 2017</span></span>

<span data-ttu-id="29801-2375">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="29801-2375">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="29801-2376">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2376">Core</span></span>

* <span data-ttu-id="29801-2377">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="29801-2377">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2378">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2378">Appservice</span></span>

* <span data-ttu-id="29801-2379">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2379">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="29801-2380">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2380">Batch</span></span>

* <span data-ttu-id="29801-2381">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="29801-2381">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="29801-2382">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="29801-2382">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="29801-2383">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="29801-2383">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="29801-2384">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="29801-2384">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="29801-2385">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="29801-2385">Batchai</span></span>

* <span data-ttu-id="29801-2386">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="29801-2386">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-2387">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2387">Keyvault</span></span>

* <span data-ttu-id="29801-2388">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="29801-2388">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="29801-2389">(#4448)</span><span class="sxs-lookup"><span data-stu-id="29801-2389">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="29801-2390">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2390">Network</span></span>

* <span data-ttu-id="29801-2391">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="29801-2391">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="29801-2392">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="29801-2392">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2393">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2393">Resource</span></span>

* <span data-ttu-id="29801-2394">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="29801-2394">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="29801-2395">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="29801-2395">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="29801-2396">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="29801-2396">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="29801-2397">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="29801-2397">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2398">Sql</span></span>

* <span data-ttu-id="29801-2399">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="29801-2399">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="29801-2400">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="29801-2400">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="29801-2401">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="29801-2401">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2402">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2402">Storage</span></span>

* <span data-ttu-id="29801-2403">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-2403">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2404">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="29801-2404">Vm</span></span>

* <span data-ttu-id="29801-2405">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="29801-2405">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="29801-2406">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2406">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="29801-2407">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="29801-2407">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="29801-2408">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2408">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="29801-2409">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="29801-2409">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="29801-2410">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2410">September 22, 2017</span></span>

<span data-ttu-id="29801-2411">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="29801-2411">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2412">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2412">Resource</span></span>

* <span data-ttu-id="29801-2413">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="29801-2413">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="29801-2414">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="29801-2414">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="29801-2415">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="29801-2415">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="29801-2416">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="29801-2416">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="29801-2417">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2417">Network</span></span>

* <span data-ttu-id="29801-2418">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="29801-2418">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="29801-2419">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="29801-2419">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="29801-2420">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="29801-2420">Added `asg` application security group commands</span></span>
* <span data-ttu-id="29801-2421">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2421">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="29801-2422">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2422">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="29801-2423">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2423">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="29801-2424">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2424">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2425">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2425">Storage</span></span>

* <span data-ttu-id="29801-2426">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="29801-2426">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="29801-2427">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="29801-2427">Eventgrid</span></span>

* <span data-ttu-id="29801-2428">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="29801-2428">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2429">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2429">SQL</span></span>

* <span data-ttu-id="29801-2430">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="29801-2430">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="29801-2431">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="29801-2431">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="29801-2432">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="29801-2432">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-2433">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2433">Keyvault</span></span>

* <span data-ttu-id="29801-2434">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="29801-2434">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2435">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2435">VM</span></span>

* <span data-ttu-id="29801-2436">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="29801-2436">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="29801-2437">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="29801-2437">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="29801-2438">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="29801-2438">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="29801-2439">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="29801-2439">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="29801-2440">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="29801-2440">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="29801-2441">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="29801-2441">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2442">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2442">ACS</span></span>

* <span data-ttu-id="29801-2443">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29801-2443">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2444">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2444">Appservice</span></span>

* <span data-ttu-id="29801-2445">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="29801-2445">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="29801-2446">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="29801-2446">Backup</span></span>

* <span data-ttu-id="29801-2447">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="29801-2447">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="29801-2448">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2448">September 11, 2017</span></span>

<span data-ttu-id="29801-2449">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="29801-2449">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="29801-2450">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2450">Core</span></span>

* <span data-ttu-id="29801-2451">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="29801-2451">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="29801-2452">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="29801-2452">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2453">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2453">Acs</span></span>

* <span data-ttu-id="29801-2454">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="29801-2454">Added `acs list-locations` command</span></span>
* <span data-ttu-id="29801-2455">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2455">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2456">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2456">Appservice</span></span>

* <span data-ttu-id="29801-2457">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="29801-2457">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-2458">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-2458">CDN</span></span>

* <span data-ttu-id="29801-2459">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2459">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="29801-2460">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="29801-2460">Extension</span></span>

* <span data-ttu-id="29801-2461">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-2461">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-2462">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2462">Keyvault</span></span>

* <span data-ttu-id="29801-2463">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-2463">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="29801-2464">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2464">Network</span></span>

* <span data-ttu-id="29801-2465">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="29801-2465">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="29801-2466">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2466">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="29801-2467">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2467">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="29801-2468">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2468">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="29801-2469">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2469">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2470">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2470">Resource</span></span>

* <span data-ttu-id="29801-2471">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2471">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="29801-2472">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2472">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="29801-2473">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="29801-2473">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="29801-2474">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="29801-2474">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2475">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2475">SQL</span></span>

* <span data-ttu-id="29801-2476">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-2476">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2477">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2477">VM</span></span>

* <span data-ttu-id="29801-2478">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="29801-2478">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="29801-2479">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="29801-2479">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="29801-2480">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2480">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="29801-2481">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="29801-2481">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="29801-2482">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="29801-2482">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="29801-2483">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2483">August 31, 2017</span></span>

<span data-ttu-id="29801-2484">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="29801-2484">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-2485">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2485">Keyvault</span></span>

* <span data-ttu-id="29801-2486">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="29801-2486">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="29801-2487">Sf</span><span class="sxs-lookup"><span data-stu-id="29801-2487">Sf</span></span>

* <span data-ttu-id="29801-2488">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="29801-2488">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2489">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2489">Storage</span></span>

* <span data-ttu-id="29801-2490">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="29801-2490">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="29801-2491">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="29801-2491">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="29801-2492">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2492">August 28, 2017</span></span>

<span data-ttu-id="29801-2493">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="29801-2493">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="29801-2494">CLI</span><span class="sxs-lookup"><span data-stu-id="29801-2494">CLI</span></span>

* <span data-ttu-id="29801-2495">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="29801-2495">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2496">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2496">ACS</span></span>

* <span data-ttu-id="29801-2497">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="29801-2497">Corrected preview regions</span></span>
* <span data-ttu-id="29801-2498">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="29801-2498">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="29801-2499">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="29801-2499">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2500">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2500">Appservice</span></span>

* <span data-ttu-id="29801-2501">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2501">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="29801-2502">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-2502">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="29801-2503">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2503">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="29801-2504">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="29801-2504">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="29801-2505">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="29801-2505">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="29801-2506">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-2506">IoT</span></span>

* <span data-ttu-id="29801-2507">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="29801-2507">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="29801-2508">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2508">Network</span></span>

* <span data-ttu-id="29801-2509">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="29801-2509">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="29801-2510">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2510">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="29801-2511">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="29801-2511">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="29801-2512">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2512">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="29801-2513">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2513">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2514">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2514">Profile</span></span>

* <span data-ttu-id="29801-2515">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="29801-2515">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="29801-2516">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-2516">Service Fabric</span></span>

* <span data-ttu-id="29801-2517">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="29801-2517">Preview release</span></span>
* <span data-ttu-id="29801-2518">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="29801-2518">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="29801-2519">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="29801-2519">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="29801-2520">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="29801-2520">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2521">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2521">Storage</span></span>

* <span data-ttu-id="29801-2522">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="29801-2522">Enabled setting blob tier</span></span>
* <span data-ttu-id="29801-2523">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="29801-2523">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="29801-2524">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="29801-2524">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="29801-2525">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="29801-2525">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="29801-2526">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2526">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="29801-2527">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="29801-2527">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2528">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2528">VM</span></span>

* <span data-ttu-id="29801-2529">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="29801-2529">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="29801-2530">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2530">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="29801-2531">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="29801-2531">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="29801-2532">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="29801-2532">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="29801-2533">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="29801-2533">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="29801-2534">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2534">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="29801-2535">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2535">August 15, 2017</span></span>

<span data-ttu-id="29801-2536">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="29801-2536">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2537">ACS</span></span>

* <span data-ttu-id="29801-2538">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="29801-2538">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2539">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2539">Appservice</span></span>

* <span data-ttu-id="29801-2540">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="29801-2540">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="29801-2541">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2541">Event Grid</span></span>

* <span data-ttu-id="29801-2542">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="29801-2542">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="29801-2543">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2543">August 11, 2017</span></span>

<span data-ttu-id="29801-2544">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="29801-2544">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2545">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2545">ACS</span></span>

* <span data-ttu-id="29801-2546">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="29801-2546">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="29801-2547">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2547">Batch</span></span>

* <span data-ttu-id="29801-2548">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="29801-2548">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="29801-2549">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="29801-2549">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="29801-2550">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-2550">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="29801-2551">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="29801-2551">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="29801-2552">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="29801-2552">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="29801-2553">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="29801-2553">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="29801-2554">Компонент</span><span class="sxs-lookup"><span data-stu-id="29801-2554">Component</span></span>

* <span data-ttu-id="29801-2555">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="29801-2555">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="29801-2556">Контейнер</span><span class="sxs-lookup"><span data-stu-id="29801-2556">Container</span></span>

* <span data-ttu-id="29801-2557">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="29801-2557">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="29801-2558">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="29801-2558">Data Lake Store</span></span>

* <span data-ttu-id="29801-2559">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="29801-2559">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="29801-2560">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2560">Event Grid</span></span>

* <span data-ttu-id="29801-2561">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="29801-2561">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="29801-2562">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2562">Network</span></span>

* <span data-ttu-id="29801-2563">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="29801-2563">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="29801-2564">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-2564">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="29801-2565">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="29801-2565">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="29801-2566">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="29801-2566">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2567">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2567">Profile</span></span>

* <span data-ttu-id="29801-2568">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="29801-2568">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2569">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2569">Storage</span></span>

* <span data-ttu-id="29801-2570">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="29801-2570">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2571">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2571">VM</span></span>

* <span data-ttu-id="29801-2572">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="29801-2572">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="29801-2573">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="29801-2573">Exposed `list-skus` command</span></span>
* <span data-ttu-id="29801-2574">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="29801-2574">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="29801-2575">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="29801-2575">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="29801-2576">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="29801-2576">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="29801-2577">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2577">July 28, 2017</span></span>

<span data-ttu-id="29801-2578">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="29801-2578">Version 2.0.12</span></span>

* <span data-ttu-id="29801-2579">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="29801-2579">Added container commands</span></span>
* <span data-ttu-id="29801-2580">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="29801-2580">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="29801-2581">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2581">Core</span></span>

* <span data-ttu-id="29801-2582">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="29801-2582">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="29801-2583">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="29801-2583">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="29801-2584">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="29801-2584">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="29801-2585">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="29801-2585">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="29801-2586">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="29801-2586">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="29801-2587">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="29801-2587">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="29801-2588">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="29801-2588">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="29801-2589">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="29801-2589">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="29801-2590">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="29801-2590">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="29801-2591">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="29801-2591">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="29801-2592">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="29801-2592">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="29801-2593">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="29801-2593">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="29801-2594">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="29801-2594">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="29801-2595">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="29801-2595">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="29801-2596">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="29801-2596">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="29801-2597">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="29801-2597">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="29801-2598">ACR</span><span class="sxs-lookup"><span data-stu-id="29801-2598">ACR</span></span>

* <span data-ttu-id="29801-2599">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="29801-2599">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="29801-2600">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="29801-2600">Support SKU update for managed registries</span></span>
* <span data-ttu-id="29801-2601">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="29801-2601">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="29801-2602">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="29801-2602">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="29801-2603">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="29801-2603">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="29801-2604">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="29801-2604">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2605">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2605">ACS</span></span>

* <span data-ttu-id="29801-2606">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="29801-2606">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2607">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="29801-2607">Appservice</span></span>

* <span data-ttu-id="29801-2608">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="29801-2608">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="29801-2609">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="29801-2609">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="29801-2610">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="29801-2610">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="29801-2611">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="29801-2611">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="29801-2612">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="29801-2612">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="29801-2613">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="29801-2613">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="29801-2614">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="29801-2614">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="29801-2615">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="29801-2615">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="29801-2616">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="29801-2616">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="29801-2617">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="29801-2617">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="29801-2618">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="29801-2618">Batch</span></span>

* <span data-ttu-id="29801-2619">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="29801-2619">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="29801-2620">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="29801-2620">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="29801-2621">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="29801-2621">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="29801-2622">CDN</span><span class="sxs-lookup"><span data-stu-id="29801-2622">CDN</span></span>

* <span data-ttu-id="29801-2623">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="29801-2623">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="29801-2624">Облако</span><span class="sxs-lookup"><span data-stu-id="29801-2624">Cloud</span></span>

* <span data-ttu-id="29801-2625">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="29801-2625">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="29801-2626">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="29801-2626">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="29801-2627">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="29801-2627">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="29801-2628">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="29801-2628">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="29801-2629">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="29801-2629">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-2630">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-2630">CosmosDB</span></span>

* <span data-ttu-id="29801-2631">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="29801-2631">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="29801-2632">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="29801-2632">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="29801-2633">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="29801-2633">Data Lake Analytics</span></span>

* <span data-ttu-id="29801-2634">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="29801-2634">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="29801-2635">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2635">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="29801-2636">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="29801-2636">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="29801-2637">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="29801-2637">Data Lake Store</span></span>

* <span data-ttu-id="29801-2638">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2638">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="29801-2639">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="29801-2639">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="29801-2640">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="29801-2640">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="29801-2641">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="29801-2641">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="29801-2642">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="29801-2642">Interactive</span></span>

* <span data-ttu-id="29801-2643">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="29801-2643">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="29801-2644">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="29801-2644">Increased test coverage</span></span>
* <span data-ttu-id="29801-2645">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="29801-2645">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="29801-2646">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="29801-2646">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="29801-2647">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="29801-2647">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="29801-2648">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="29801-2648">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="29801-2649">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="29801-2649">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="29801-2650">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="29801-2650">Added `--progress` flag</span></span>
* <span data-ttu-id="29801-2651">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="29801-2651">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="29801-2652">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="29801-2652">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="29801-2653">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="29801-2653">IoT</span></span>

* <span data-ttu-id="29801-2654">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="29801-2654">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="29801-2655">(3934).</span><span class="sxs-lookup"><span data-stu-id="29801-2655">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="29801-2656">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2656">Key vault</span></span>

* <span data-ttu-id="29801-2657">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="29801-2657">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="29801-2658">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="29801-2658">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="29801-2659">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="29801-2659">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="29801-2660">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="29801-2660">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="29801-2661">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="29801-2661">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="29801-2662">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="29801-2662">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="29801-2663">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="29801-2663">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="29801-2664">(3307).</span><span class="sxs-lookup"><span data-stu-id="29801-2664">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="29801-2665">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="29801-2665">Lab</span></span>

* <span data-ttu-id="29801-2666">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="29801-2666">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="29801-2667">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2667">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2668">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2668">Monitor</span></span>

* <span data-ttu-id="29801-2669">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="29801-2669">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="29801-2670">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="29801-2670">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="29801-2671">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="29801-2671">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="29801-2672">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="29801-2672">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="29801-2673">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="29801-2673">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="29801-2674">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="29801-2674">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="29801-2675">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="29801-2675">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="29801-2676">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="29801-2676">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="29801-2677">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="29801-2677">`location` no longer required</span></span>
  * <span data-ttu-id="29801-2678">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="29801-2678">Add name and ID support for target</span></span>
  * <span data-ttu-id="29801-2679">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="29801-2679">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="29801-2680">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="29801-2680">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="29801-2681">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="29801-2681">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="29801-2682">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="29801-2682">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="29801-2683">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="29801-2683">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="29801-2684">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2684">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="29801-2685">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2685">Network</span></span>

* <span data-ttu-id="29801-2686">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="29801-2686">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="29801-2687">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2687">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="29801-2688">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="29801-2688">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="29801-2689">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="29801-2689">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="29801-2690">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2690">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="29801-2691">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="29801-2691">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="29801-2692">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2692">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="29801-2693">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="29801-2693">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="29801-2694">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="29801-2694">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="29801-2695">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="29801-2695">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="29801-2696">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2696">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="29801-2697">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="29801-2697">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="29801-2698">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="29801-2698">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="29801-2699">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2699">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="29801-2700">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2700">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="29801-2701">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2701">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="29801-2702">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="29801-2702">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="29801-2703">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="29801-2703">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="29801-2704">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2704">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="29801-2705">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2705">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="29801-2706">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2706">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="29801-2707">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="29801-2707">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="29801-2708">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="29801-2708">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="29801-2709">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="29801-2709">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="29801-2710">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="29801-2710">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="29801-2711">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="29801-2711">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="29801-2712">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="29801-2712">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2713">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2713">Profile</span></span>

* <span data-ttu-id="29801-2714">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="29801-2714">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="29801-2715">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="29801-2715">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="29801-2716">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="29801-2716">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="29801-2717">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="29801-2717">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="29801-2718">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="29801-2718">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="29801-2719">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="29801-2719">RDBMS</span></span>

* <span data-ttu-id="29801-2720">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="29801-2720">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="29801-2721">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="29801-2721">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="29801-2722">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="29801-2722">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="29801-2723">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="29801-2723">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2724">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2724">Resource</span></span>

* <span data-ttu-id="29801-2725">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2725">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="29801-2726">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="29801-2726">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="29801-2727">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="29801-2727">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="29801-2728">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="29801-2728">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="29801-2729">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="29801-2729">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="29801-2730">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="29801-2730">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="29801-2731">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="29801-2731">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="29801-2732">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="29801-2732">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="29801-2733">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2733">Role</span></span>

* <span data-ttu-id="29801-2734">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="29801-2734">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="29801-2735">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="29801-2735">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="29801-2736">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="29801-2736">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="29801-2737">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="29801-2737">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="29801-2738">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="29801-2738">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="29801-2739">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="29801-2739">Service Fabric</span></span>
* <span data-ttu-id="29801-2740">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="29801-2740">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="29801-2741">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="29801-2741">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="29801-2742">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="29801-2742">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2743">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2743">SQL</span></span>

* <span data-ttu-id="29801-2744">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2744">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="29801-2745">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="29801-2745">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="29801-2746">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="29801-2746">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2747">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2747">Storage</span></span>

* <span data-ttu-id="29801-2748">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="29801-2748">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="29801-2749">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="29801-2749">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="29801-2750">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="29801-2750">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="29801-2751">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="29801-2751">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="29801-2752">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="29801-2752">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="29801-2753">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="29801-2753">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2754">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2754">VM</span></span>

* <span data-ttu-id="29801-2755">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="29801-2755">Support configuring nsg</span></span>
* <span data-ttu-id="29801-2756">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="29801-2756">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="29801-2757">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="29801-2757">Support managed service identities</span></span>
* <span data-ttu-id="29801-2758">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="29801-2758">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="29801-2759">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="29801-2759">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="29801-2760">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2760">May 10, 2017</span></span>

<span data-ttu-id="29801-2761">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="29801-2761">Version 2.0.6</span></span>

* <span data-ttu-id="29801-2762">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="29801-2762">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="29801-2763">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="29801-2763">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="29801-2764">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="29801-2764">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="29801-2765">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="29801-2765">Include Cognitive Services module</span></span>
* <span data-ttu-id="29801-2766">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="29801-2766">Include Service Fabric module</span></span>
* <span data-ttu-id="29801-2767">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="29801-2767">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="29801-2768">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="29801-2768">Add support for CDN commands</span></span>
* <span data-ttu-id="29801-2769">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="29801-2769">Remove Container module</span></span>
* <span data-ttu-id="29801-2770">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="29801-2770">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="29801-2771">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="29801-2771">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="29801-2772">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2772">Core</span></span>

* <span data-ttu-id="29801-2773">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="29801-2773">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="29801-2774">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="29801-2774">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="29801-2775">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="29801-2775">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="29801-2776">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="29801-2776">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="29801-2777">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="29801-2777">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="29801-2778">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="29801-2778">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="29801-2779">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="29801-2779">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="29801-2780">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="29801-2780">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="29801-2781">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="29801-2781">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="29801-2782">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="29801-2782">core: Improved performance</span></span>
* <span data-ttu-id="29801-2783">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="29801-2783">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="29801-2784">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="29801-2784">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2785">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2785">ACS</span></span>

* <span data-ttu-id="29801-2786">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="29801-2786">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="29801-2787">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="29801-2787">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="29801-2788">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="29801-2788">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="29801-2789">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="29801-2789">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2790">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-2790">AppService</span></span>

* <span data-ttu-id="29801-2791">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="29801-2791">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="29801-2792">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-2792">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="29801-2793">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="29801-2793">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="29801-2794">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="29801-2794">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="29801-2795">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="29801-2795">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="29801-2796">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="29801-2796">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="29801-2797">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="29801-2797">support slot swap with preview</span></span>
* <span data-ttu-id="29801-2798">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="29801-2798">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="29801-2799">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="29801-2799">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="29801-2800">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="29801-2800">CosmosDB</span></span>

* <span data-ttu-id="29801-2801">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="29801-2801">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="29801-2802">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="29801-2802">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="29801-2803">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="29801-2803">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="29801-2804">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="29801-2804">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="29801-2805">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="29801-2805">Data Lake Analytics</span></span>

* <span data-ttu-id="29801-2806">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="29801-2806">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="29801-2807">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="29801-2807">Add support for new catalog item type: package.</span></span> <span data-ttu-id="29801-2808">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="29801-2808">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="29801-2809">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="29801-2809">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="29801-2810">Таблица</span><span class="sxs-lookup"><span data-stu-id="29801-2810">Table</span></span>
  * <span data-ttu-id="29801-2811">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="29801-2811">Table valued function</span></span>
  * <span data-ttu-id="29801-2812">Просмотр</span><span class="sxs-lookup"><span data-stu-id="29801-2812">View</span></span>
  * <span data-ttu-id="29801-2813">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="29801-2813">Table Statistics.</span></span> <span data-ttu-id="29801-2814">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="29801-2814">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="29801-2815">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="29801-2815">Data Lake Store</span></span>

* <span data-ttu-id="29801-2816">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="29801-2816">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="29801-2817">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="29801-2817">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="29801-2818">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="29801-2818">missed help for access show.</span></span> <span data-ttu-id="29801-2819">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="29801-2819">adding it.</span></span> <span data-ttu-id="29801-2820">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="29801-2820">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="29801-2821">Поиск</span><span class="sxs-lookup"><span data-stu-id="29801-2821">Find</span></span>

* <span data-ttu-id="29801-2822">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="29801-2822">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="29801-2823">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="29801-2823">KeyVault</span></span>

* <span data-ttu-id="29801-2824">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="29801-2824">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="29801-2825">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="29801-2825">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="29801-2826">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="29801-2826">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="29801-2827">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="29801-2827">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="29801-2828">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="29801-2828">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="29801-2829">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="29801-2829">Lab</span></span>

* <span data-ttu-id="29801-2830">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="29801-2830">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="29801-2831">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="29801-2831">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="29801-2832">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="29801-2832">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="29801-2833">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="29801-2833">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="29801-2834">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="29801-2834">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="29801-2835">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="29801-2835">Monitor</span></span>

* <span data-ttu-id="29801-2836">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="29801-2836">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="29801-2837">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="29801-2837">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="29801-2838">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2838">Network</span></span>

* <span data-ttu-id="29801-2839">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="29801-2839">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="29801-2840">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2840">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="29801-2841">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-2841">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="29801-2842">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="29801-2842">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="29801-2843">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="29801-2843">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="29801-2844">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="29801-2844">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="29801-2845">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="29801-2845">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="29801-2846">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="29801-2846">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="29801-2847">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="29801-2847">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="29801-2848">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="29801-2848">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="29801-2849">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="29801-2849">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="29801-2850">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2850">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="29801-2851">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="29801-2851">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="29801-2852">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="29801-2852">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="29801-2853">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="29801-2853">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="29801-2854">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="29801-2854">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="29801-2855">Профиль</span><span class="sxs-lookup"><span data-stu-id="29801-2855">Profile</span></span>

* <span data-ttu-id="29801-2856">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="29801-2856">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="29801-2857">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="29801-2857">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="29801-2858">Redis</span><span class="sxs-lookup"><span data-stu-id="29801-2858">Redis</span></span>

* <span data-ttu-id="29801-2859">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="29801-2859">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="29801-2860">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="29801-2860">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="29801-2861">Ресурс</span><span class="sxs-lookup"><span data-stu-id="29801-2861">Resource</span></span>

* <span data-ttu-id="29801-2862">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="29801-2862">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="29801-2863">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="29801-2863">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="29801-2864">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="29801-2864">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="29801-2865">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="29801-2865">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="29801-2866">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="29801-2866">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="29801-2867">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="29801-2867">Add docs for az lock update.</span></span> <span data-ttu-id="29801-2868">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="29801-2868">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="29801-2869">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="29801-2869">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="29801-2870">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="29801-2870">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="29801-2871">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="29801-2871">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="29801-2872">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="29801-2872">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="29801-2873">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="29801-2873">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="29801-2874">Роль</span><span class="sxs-lookup"><span data-stu-id="29801-2874">Role</span></span>

* <span data-ttu-id="29801-2875">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="29801-2875">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="29801-2876">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="29801-2876">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="29801-2877">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="29801-2877">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="29801-2878">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="29801-2878">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="29801-2879">SQL</span><span class="sxs-lookup"><span data-stu-id="29801-2879">SQL</span></span>

* <span data-ttu-id="29801-2880">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="29801-2880">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="29801-2881">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="29801-2881">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="29801-2882">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2882">Storage</span></span>

* <span data-ttu-id="29801-2883">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="29801-2883">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="29801-2884">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-2884">Add support for incremental blob copy</span></span>
* <span data-ttu-id="29801-2885">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="29801-2885">Add support for large block blob upload</span></span>
* <span data-ttu-id="29801-2886">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="29801-2886">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2887">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2887">VM</span></span>

* <span data-ttu-id="29801-2888">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="29801-2888">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="29801-2889">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="29801-2889">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="29801-2890">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="29801-2890">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="29801-2891">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="29801-2891">az vm/vmss disk</span></span>
  3. <span data-ttu-id="29801-2892">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="29801-2892">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="29801-2893">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="29801-2893">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="29801-2894">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="29801-2894">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="29801-2895">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2895">April 3, 2017</span></span>

<span data-ttu-id="29801-2896">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="29801-2896">Version 2.0.2</span></span>

<span data-ttu-id="29801-2897">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="29801-2897">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="29801-2898">Core</span><span class="sxs-lookup"><span data-stu-id="29801-2898">Core</span></span>

* <span data-ttu-id="29801-2899">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2899">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="29801-2900">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="29801-2900">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="29801-2901">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="29801-2901">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="29801-2902">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="29801-2902">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="29801-2903">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="29801-2903">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="29801-2904">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="29801-2904">Add prompting for missing template parameters.</span></span> <span data-ttu-id="29801-2905">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="29801-2905">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="29801-2906">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29801-2906">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="29801-2907">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="29801-2907">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="29801-2908">ACS</span><span class="sxs-lookup"><span data-stu-id="29801-2908">ACS</span></span>

* <span data-ttu-id="29801-2909">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="29801-2909">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="29801-2910">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="29801-2910">Add support for ssh key password prompting.</span></span> <span data-ttu-id="29801-2911">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="29801-2911">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="29801-2912">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="29801-2912">Add support for windows clusters.</span></span> <span data-ttu-id="29801-2913">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="29801-2913">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="29801-2914">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="29801-2914">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="29801-2915">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="29801-2915">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="29801-2916">AppService</span><span class="sxs-lookup"><span data-stu-id="29801-2916">AppService</span></span>

* <span data-ttu-id="29801-2917">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="29801-2917">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="29801-2918">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="29801-2918">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="29801-2919">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="29801-2919">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="29801-2920">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="29801-2920">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="29801-2921">Data Lake</span><span class="sxs-lookup"><span data-stu-id="29801-2921">DataLake</span></span>

* <span data-ttu-id="29801-2922">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="29801-2922">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="29801-2923">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="29801-2923">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="29801-2924">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="29801-2924">DocuemntDB</span></span>

* <span data-ttu-id="29801-2925">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="29801-2925">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="29801-2926">ВМ</span><span class="sxs-lookup"><span data-stu-id="29801-2926">VM</span></span>

* <span data-ttu-id="29801-2927">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="29801-2927">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="29801-2928">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="29801-2928">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="29801-2929">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="29801-2929">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="29801-2930">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="29801-2930">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="29801-2931">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="29801-2931">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="29801-2932">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="29801-2932">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="29801-2933">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="29801-2933">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="29801-2934">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="29801-2934">February 27, 2017</span></span>

<span data-ttu-id="29801-2935">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="29801-2935">Version 2.0.0</span></span>

<span data-ttu-id="29801-2936">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="29801-2936">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="29801-2937">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="29801-2937">Container Service (acs)</span></span>
- <span data-ttu-id="29801-2938">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="29801-2938">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="29801-2939">Сеть</span><span class="sxs-lookup"><span data-stu-id="29801-2939">Networking</span></span>
- <span data-ttu-id="29801-2940">Хранилище</span><span class="sxs-lookup"><span data-stu-id="29801-2940">Storage</span></span>

<span data-ttu-id="29801-2941">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="29801-2941">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="29801-2942">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="29801-2942">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="29801-2943">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="29801-2943">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="29801-2944">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="29801-2944">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="29801-2945">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="29801-2945">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="29801-2946">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="29801-2946">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="29801-2947">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="29801-2947">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="29801-2948">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="29801-2948">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="29801-2949">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="29801-2949">Provide feedback from the command line with the `az feedback` command</span></span>

