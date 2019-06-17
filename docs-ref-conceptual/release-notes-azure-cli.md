---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/05/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: b79d76480c3e6619427d6a7e3960f53b691889cc
ms.sourcegitcommit: 6aca5a788b9731e6cbeeb497c83a9197ebb7d36e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2019
ms.locfileid: "66750231"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="5f191-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5f191-103">Azure CLI release notes</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="5f191-104">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-104">June 4, 2019</span></span>

<span data-ttu-id="5f191-105">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="5f191-105">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="5f191-106">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-106">Core</span></span>
* <span data-ttu-id="5f191-107">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="5f191-107">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-108">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-108">ACR</span></span>
* <span data-ttu-id="5f191-109">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="5f191-109">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-110">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-110">ACS</span></span>
* <span data-ttu-id="5f191-111">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="5f191-111">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="5f191-112">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="5f191-112">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-113">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-113">Batch</span></span>
* <span data-ttu-id="5f191-114">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="5f191-114">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-115">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-115">IoT</span></span>
* <span data-ttu-id="5f191-116">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5f191-116">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="5f191-117">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-117">Network</span></span>
* <span data-ttu-id="5f191-118">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="5f191-118">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="5f191-119">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-119">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="5f191-120">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-120">Resource</span></span>
* <span data-ttu-id="5f191-121">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="5f191-121">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="5f191-122">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-122">Role</span></span>
* <span data-ttu-id="5f191-123">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="5f191-123">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="5f191-124">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5f191-124">Compute</span></span>
* <span data-ttu-id="5f191-125">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="5f191-125">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="5f191-126">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-126">May 21, 2019</span></span>

<span data-ttu-id="5f191-127">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="5f191-127">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="5f191-128">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-128">Core</span></span>
* <span data-ttu-id="5f191-129">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5f191-129">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="5f191-130">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="5f191-130">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="5f191-131">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-131">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-132">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-132">ACR</span></span>
* <span data-ttu-id="5f191-133">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="5f191-133">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-134">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-134">ACS</span></span>
* <span data-ttu-id="5f191-135">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="5f191-135">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-136">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-136">AppService</span></span>
* <span data-ttu-id="5f191-137">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="5f191-137">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="5f191-138">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="5f191-138">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="5f191-139">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5f191-139">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="5f191-140">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="5f191-140">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="5f191-141">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5f191-141">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="5f191-142">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="5f191-142">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="5f191-143">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="5f191-143">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-144">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-144">BotService</span></span>
* <span data-ttu-id="5f191-145">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-145">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="5f191-146">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="5f191-146">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-147">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-147">Consumption</span></span>
* <span data-ttu-id="5f191-148">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-148">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-149">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-149">IoT</span></span>
* <span data-ttu-id="5f191-150">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="5f191-150">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="5f191-151">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-151">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="5f191-153">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="5f191-153">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="5f191-154">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="5f191-154">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-155">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-155">RDBMS</span></span>
* <span data-ttu-id="5f191-156">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="5f191-156">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="5f191-157">RBAC</span><span class="sxs-lookup"><span data-stu-id="5f191-157">RBAC</span></span>
* <span data-ttu-id="5f191-158">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="5f191-158">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-159">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-159">Storage</span></span>
* <span data-ttu-id="5f191-160">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-160">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="5f191-161">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="5f191-161">Compute</span></span>
* <span data-ttu-id="5f191-162">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5f191-162">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="5f191-163">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="5f191-163">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="5f191-164">__Примечание__. Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="5f191-164">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="5f191-165">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="5f191-165">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="5f191-166">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-166">May 6, 2019</span></span>

<span data-ttu-id="5f191-167">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="5f191-167">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-168">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-168">ACS</span></span>
* <span data-ttu-id="5f191-169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="5f191-169">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="5f191-170">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="5f191-170">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="5f191-171">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-171">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="5f191-172">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-172">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-173">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-173">Appservice</span></span>
* <span data-ttu-id="5f191-174">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5f191-174">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="5f191-175">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="5f191-175">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="5f191-176">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5f191-176">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="5f191-177">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-177">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="5f191-178">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="5f191-178">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="5f191-179">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5f191-179">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="5f191-180">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="5f191-180">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="5f191-181">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="5f191-181">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="5f191-182">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-182">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="5f191-183">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="5f191-183">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-184">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-184">Batch</span></span>
* <span data-ttu-id="5f191-185">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="5f191-185">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-186">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-186">Botservice</span></span>
* <span data-ttu-id="5f191-187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="5f191-187">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="5f191-188">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="5f191-188">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="5f191-189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="5f191-189">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="5f191-190">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-190">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="5f191-191">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-191">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="5f191-192">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5f191-192">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="5f191-193">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-193">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="5f191-194">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="5f191-194">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="5f191-195">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5f191-195">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="5f191-196">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5f191-196">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="5f191-197">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="5f191-197">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="5f191-198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="5f191-198">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="5f191-199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="5f191-199">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="5f191-200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="5f191-200">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="5f191-201">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-201">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="5f191-202">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="5f191-202">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="5f191-203">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="5f191-203">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5f191-204">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="5f191-204">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="5f191-205">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="5f191-205">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="5f191-206">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-206">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="5f191-207">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="5f191-207">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="5f191-208">Настройка</span><span class="sxs-lookup"><span data-stu-id="5f191-208">Configure</span></span>
* <span data-ttu-id="5f191-209">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="5f191-209">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5f191-210">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5f191-210">Eventhubs</span></span>
* <span data-ttu-id="5f191-211">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-211">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5f191-212">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-212">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-213">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-213">Network</span></span>
* <span data-ttu-id="5f191-214">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-214">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="5f191-215">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5f191-215">Policy Insights</span></span>
* <span data-ttu-id="5f191-216">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f191-216">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="5f191-217">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-217">Role</span></span>
* <span data-ttu-id="5f191-218">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="5f191-218">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f191-219">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-219">Service Bus</span></span>
* <span data-ttu-id="5f191-220">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-220">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="5f191-221">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-221">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="5f191-222">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5f191-222">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-223">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-223">SQL</span></span>
* <span data-ttu-id="5f191-224">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-224">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-225">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-225">VM</span></span>
* <span data-ttu-id="5f191-226">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5f191-226">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="5f191-227">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5f191-227">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="5f191-228">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-228">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="5f191-229">Добавлена новая группа команд `ppg` для управления группами размещения близкого расположения.</span><span class="sxs-lookup"><span data-stu-id="5f191-229">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="5f191-230">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="5f191-230">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="5f191-231">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-231">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="5f191-232">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-232">April 23, 2019</span></span>

<span data-ttu-id="5f191-233">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="5f191-233">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-234">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-234">ACS</span></span>
* <span data-ttu-id="5f191-235">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="5f191-235">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="5f191-236">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="5f191-236">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-237">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-237">AMS</span></span>
* <span data-ttu-id="5f191-238">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="5f191-238">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-239">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-239">AppService</span></span>
* <span data-ttu-id="5f191-240">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5f191-240">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="5f191-241">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5f191-241">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="5f191-242">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="5f191-242">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="5f191-243">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="5f191-243">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="5f191-244">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-244">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="5f191-245">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="5f191-245">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="5f191-246">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="5f191-246">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="5f191-247">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="5f191-247">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="5f191-248">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="5f191-248">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="5f191-249">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="5f191-249">Deployment Manager</span></span>
* <span data-ttu-id="5f191-250">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="5f191-250">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="5f191-251">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5f191-251">Lab</span></span>
* <span data-ttu-id="5f191-252">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="5f191-252">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="5f191-253">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-253">Network</span></span>
* <span data-ttu-id="5f191-254">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="5f191-254">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-255">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-255">Resource</span></span>
* <span data-ttu-id="5f191-256">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="5f191-256">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="5f191-257">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="5f191-257">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="5f191-258">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="5f191-258">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="5f191-259">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="5f191-259">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-260">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-260">SQL</span></span>
* <span data-ttu-id="5f191-261">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5f191-261">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="5f191-262">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-262">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="5f191-263">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-263">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="5f191-264">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-264">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-265">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-265">Storage</span></span>
* <span data-ttu-id="5f191-266">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="5f191-266">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-267">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-267">VM</span></span>
* <span data-ttu-id="5f191-268">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="5f191-268">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="5f191-269">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="5f191-269">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="5f191-270">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="5f191-270">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="5f191-271">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-271">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="5f191-272">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-272">Core</span></span>
* <span data-ttu-id="5f191-273">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="5f191-273">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-274">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-274">ACR</span></span>
* <span data-ttu-id="5f191-275">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="5f191-275">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-276">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-276">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="5f191-279">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-279">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="5f191-280">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-280">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-281">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-281">AppService</span></span>
* <span data-ttu-id="5f191-282">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="5f191-282">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="5f191-283">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="5f191-283">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="5f191-284">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-284">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="5f191-285">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-285">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="5f191-286">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="5f191-286">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="5f191-287">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="5f191-287">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="5f191-288">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-288">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-289">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-289">CDN</span></span>
* <span data-ttu-id="5f191-290">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="5f191-290">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="5f191-291">Отзыв</span><span class="sxs-lookup"><span data-stu-id="5f191-291">Feedback</span></span>
* <span data-ttu-id="5f191-292">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-292">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="5f191-293">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="5f191-293">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="5f191-294">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="5f191-294">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-295">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-295">Monitor</span></span>
* <span data-ttu-id="5f191-296">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-296">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="5f191-297">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-297">Network</span></span>
* <span data-ttu-id="5f191-298">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="5f191-298">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="5f191-299">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-299">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="5f191-300">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-300">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="5f191-301">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-301">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="5f191-302">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="5f191-302">PrivateDNS</span></span>
* <span data-ttu-id="5f191-303">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5f191-303">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-304">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-304">Resource</span></span>
* <span data-ttu-id="5f191-305">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="5f191-305">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="5f191-306">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-306">Role</span></span>
* <span data-ttu-id="5f191-307">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="5f191-307">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="5f191-308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="5f191-308">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-309">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-309">SQL</span></span>
* <span data-ttu-id="5f191-310">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="5f191-310">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-311">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-311">Storage</span></span>
* <span data-ttu-id="5f191-312">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="5f191-312">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="5f191-313">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="5f191-313">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="5f191-314">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="5f191-314">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="5f191-315">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5f191-315">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="5f191-316">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-316">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="5f191-317">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-317">Core</span></span>
* <span data-ttu-id="5f191-318">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="5f191-318">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="5f191-319">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="5f191-319">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="5f191-320">Облако</span><span class="sxs-lookup"><span data-stu-id="5f191-320">Cloud</span></span>
* <span data-ttu-id="5f191-321">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="5f191-321">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-322">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-322">ACR</span></span>
* <span data-ttu-id="5f191-323">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5f191-323">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="5f191-324">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-324">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="5f191-325">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="5f191-325">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="5f191-326">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="5f191-326">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-327">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-327">AppService</span></span>
* <span data-ttu-id="5f191-328">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="5f191-328">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="5f191-329">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="5f191-329">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="5f191-330">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-330">BOT Service</span></span>
* <span data-ttu-id="5f191-331">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="5f191-331">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="5f191-332">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="5f191-332">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="5f191-333">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="5f191-333">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="5f191-334">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5f191-334">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-335">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-335">CDN</span></span>
* <span data-ttu-id="5f191-336">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-336">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="5f191-337">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-337">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="5f191-338">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-338">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5f191-339">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5f191-339">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-340">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-340">Cosmosdb</span></span>
* <span data-ttu-id="5f191-341">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5f191-341">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="5f191-342">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5f191-342">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-343">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-343">Interactive</span></span>
* <span data-ttu-id="5f191-344">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="5f191-344">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-345">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-345">Monitor</span></span>
* <span data-ttu-id="5f191-346">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-346">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-347">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-347">Network</span></span>
* <span data-ttu-id="5f191-348">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5f191-348">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-349">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-349">Profile</span></span>
* <span data-ttu-id="5f191-350">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="5f191-350">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="5f191-351">Postgres</span><span class="sxs-lookup"><span data-stu-id="5f191-351">Postgres</span></span> 
* <span data-ttu-id="5f191-352">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="5f191-352">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="5f191-353">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5f191-353">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-354">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-354">Resource</span></span>
* <span data-ttu-id="5f191-355">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-355">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="5f191-356">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="5f191-356">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="5f191-357">График</span><span class="sxs-lookup"><span data-stu-id="5f191-357">Graph</span></span>
* <span data-ttu-id="5f191-358">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="5f191-358">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="5f191-359">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="5f191-359">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="5f191-360">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="5f191-360">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="5f191-361">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="5f191-361">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="5f191-362">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="5f191-362">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-363">storage</span><span class="sxs-lookup"><span data-stu-id="5f191-363">storage</span></span>
* <span data-ttu-id="5f191-364">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f191-364">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="5f191-365">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="5f191-365">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="5f191-366">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="5f191-366">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="5f191-367">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="5f191-367">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-368">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-368">VM</span></span>
* <span data-ttu-id="5f191-369">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-369">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="5f191-370">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-370">March 12, 2019</span></span>

<span data-ttu-id="5f191-371">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="5f191-371">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="5f191-372">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-372">Core</span></span>

* <span data-ttu-id="5f191-373">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="5f191-373">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-374">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-374">ACR</span></span>

* <span data-ttu-id="5f191-375">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="5f191-375">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-376">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-376">ACS</span></span>

* <span data-ttu-id="5f191-377">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="5f191-377">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="5f191-378">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-378">AppService</span></span>

* <span data-ttu-id="5f191-379">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-379">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="5f191-380">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-380">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="5f191-381">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="5f191-381">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="5f191-382">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="5f191-382">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-383">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-383">Botservice</span></span>

* <span data-ttu-id="5f191-384">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5f191-384">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5f191-385">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="5f191-385">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5f191-386">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-386">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="5f191-387">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="5f191-387">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="5f191-388">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-388">Container</span></span>

* <span data-ttu-id="5f191-389">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="5f191-389">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f191-390">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5f191-390">EventHub</span></span>

* <span data-ttu-id="5f191-391">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="5f191-391">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="5f191-392">Поиск</span><span class="sxs-lookup"><span data-stu-id="5f191-392">Find</span></span>

* <span data-ttu-id="5f191-393">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="5f191-393">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f191-394">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f191-394">HDInsight</span></span>

* <span data-ttu-id="5f191-395">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="5f191-395">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="5f191-396">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-396">Network</span></span>

* <span data-ttu-id="5f191-397">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5f191-397">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-398">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f191-398">Rdbms</span></span>

* <span data-ttu-id="5f191-399">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="5f191-399">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="5f191-400">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-400">Role</span></span>

* <span data-ttu-id="5f191-401">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="5f191-401">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="5f191-402">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-402">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f191-403">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f191-403">Service Fabric</span></span>

* <span data-ttu-id="5f191-404">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="5f191-404">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="5f191-405">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-405">February 26, 2019</span></span>

<span data-ttu-id="5f191-406">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="5f191-406">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="5f191-407">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-407">Core</span></span>

* <span data-ttu-id="5f191-408">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="5f191-408">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-409">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-409">ACR</span></span>

* <span data-ttu-id="5f191-410">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-410">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="5f191-411">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-411">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-412">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-412">ACS</span></span>

* <span data-ttu-id="5f191-413">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="5f191-413">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-414">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-414">AppService</span></span>

* <span data-ttu-id="5f191-415">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="5f191-415">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-416">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-416">Batch</span></span>
* <span data-ttu-id="5f191-417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="5f191-417">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="5f191-418">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="5f191-418">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="5f191-419">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="5f191-419">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="5f191-420">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="5f191-420">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="5f191-421">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="5f191-421">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="5f191-422">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5f191-422">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-423">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-423">CosmosDB</span></span>

* <span data-ttu-id="5f191-424">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="5f191-424">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="5f191-425">Kusto</span><span class="sxs-lookup"><span data-stu-id="5f191-425">Kusto</span></span>

* <span data-ttu-id="5f191-426">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="5f191-426">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="5f191-427">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-427">Network</span></span>

* <span data-ttu-id="5f191-428">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-428">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="5f191-429">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="5f191-429">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="5f191-430">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="5f191-430">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="5f191-431">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-431">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="5f191-432">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-432">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="5f191-433">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-433">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="5f191-434">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="5f191-434">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-435">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-435">Resource</span></span>

* <span data-ttu-id="5f191-436">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5f191-436">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="5f191-437">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-437">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="5f191-438">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-438">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="5f191-439">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-439">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="5f191-440">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-440">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="5f191-441">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-441">Role</span></span>

* <span data-ttu-id="5f191-442">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-442">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-443">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-443">VM</span></span>

* <span data-ttu-id="5f191-444">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="5f191-444">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="5f191-445">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-445">February 12, 2019</span></span>

<span data-ttu-id="5f191-446">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="5f191-446">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="5f191-447">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-447">Core</span></span>

* <span data-ttu-id="5f191-448">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="5f191-448">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="5f191-449">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="5f191-449">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-450">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-450">ACR</span></span>
* <span data-ttu-id="5f191-451">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="5f191-451">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="5f191-452">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="5f191-452">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-453">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-453">ACS</span></span>
* <span data-ttu-id="5f191-454">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5f191-454">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="5f191-455">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="5f191-455">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="5f191-456">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="5f191-456">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-457">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-457">AMS</span></span>
* <span data-ttu-id="5f191-458">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-458">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="5f191-459">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-459">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-460">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-460">Appservice</span></span>
* <span data-ttu-id="5f191-461">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-461">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="5f191-462">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="5f191-462">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="5f191-463">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-463">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="5f191-464">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5f191-464">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="5f191-465">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-465">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-466">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-466">Botservice</span></span>
* <span data-ttu-id="5f191-467">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5f191-467">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="5f191-468">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="5f191-468">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="5f191-469">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-469">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="5f191-470">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="5f191-470">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="5f191-471">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="5f191-471">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="5f191-472">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="5f191-472">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="5f191-473">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-473">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="5f191-474">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-474">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="5f191-475">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="5f191-475">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="5f191-476">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="5f191-476">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f191-477">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f191-477">Key Vault</span></span>
* <span data-ttu-id="5f191-478">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="5f191-478">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-479">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-479">Monitor</span></span>
* <span data-ttu-id="5f191-480">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="5f191-480">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-481">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-481">Network</span></span>
* <span data-ttu-id="5f191-482">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="5f191-482">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="5f191-483">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-483">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="5f191-484">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="5f191-484">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="5f191-485">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="5f191-485">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5f191-486">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5f191-486">Policy Insights</span></span>
* <span data-ttu-id="5f191-487">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-487">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-488">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-488">RDBMS</span></span>
* <span data-ttu-id="5f191-489">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="5f191-489">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="5f191-490">Redis</span><span class="sxs-lookup"><span data-stu-id="5f191-490">Redis</span></span>
* <span data-ttu-id="5f191-491">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5f191-491">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="5f191-492">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="5f191-492">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="5f191-493">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="5f191-493">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="5f191-494">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="5f191-494">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="5f191-495">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="5f191-495">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="5f191-496">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="5f191-496">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="5f191-497">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f191-497">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="5f191-498">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-498">Role</span></span>
* <span data-ttu-id="5f191-499">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="5f191-499">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5f191-500">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-500">SQL VM</span></span>
* <span data-ttu-id="5f191-501">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="5f191-501">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-502">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-502">VM</span></span>
* <span data-ttu-id="5f191-503">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="5f191-503">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="5f191-504">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-504">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="5f191-505">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="5f191-505">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="5f191-506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="5f191-506">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="5f191-507">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-507">January 31, 2019</span></span>

<span data-ttu-id="5f191-508">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="5f191-508">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="5f191-509">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-509">Core</span></span>

* <span data-ttu-id="5f191-510">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="5f191-510">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="5f191-511">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-511">January 28, 2019</span></span>

<span data-ttu-id="5f191-512">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="5f191-512">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-513">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-513">ACR</span></span>
* <span data-ttu-id="5f191-514">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5f191-514">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-515">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-515">ACS</span></span>
* <span data-ttu-id="5f191-516">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-516">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5f191-517">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="5f191-517">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="5f191-518">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="5f191-518">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-519">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-519">AMS</span></span>
* <span data-ttu-id="5f191-520">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="5f191-520">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="5f191-521">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="5f191-521">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-522">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-522">Appservice</span></span>
* <span data-ttu-id="5f191-523">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-523">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="5f191-524">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5f191-524">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="5f191-525">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5f191-525">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="5f191-526">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-526">Container</span></span>
* <span data-ttu-id="5f191-527">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="5f191-527">Added `container start` command</span></span>
* <span data-ttu-id="5f191-528">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-528">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f191-529">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5f191-529">EventGrid</span></span>
* <span data-ttu-id="5f191-530">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-530">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="5f191-531">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="5f191-531">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="5f191-532">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="5f191-532">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="5f191-533">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="5f191-533">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="5f191-534">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5f191-534">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f191-535">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f191-535">HDInsight</span></span>
* <span data-ttu-id="5f191-536">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-536">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="5f191-537">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-537">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="5f191-538">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-538">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="5f191-539">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="5f191-539">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="5f191-540">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="5f191-540">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="5f191-541">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-541">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-542">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-542">IoT</span></span>
* <span data-ttu-id="5f191-543">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="5f191-543">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="5f191-544">Kusto</span><span class="sxs-lookup"><span data-stu-id="5f191-544">Kusto</span></span>
* <span data-ttu-id="5f191-545">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5f191-545">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-546">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-546">Monitor</span></span>
* <span data-ttu-id="5f191-547">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5f191-547">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-548">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-548">Profile</span></span>
* <span data-ttu-id="5f191-549">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-549">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-550">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-550">Network</span></span>
* <span data-ttu-id="5f191-551">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="5f191-551">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="5f191-552">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="5f191-552">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-553">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-553">Resource</span></span>
* <span data-ttu-id="5f191-554">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-554">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="5f191-555">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-555">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="5f191-556">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-556">SQL Virtual Machine</span></span>
* <span data-ttu-id="5f191-557">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5f191-557">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-558">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-558">Storage</span></span>
* <span data-ttu-id="5f191-559">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="5f191-559">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="5f191-560">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="5f191-560">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-561">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-561">VM</span></span>
* <span data-ttu-id="5f191-562">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="5f191-562">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="5f191-563">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5f191-563">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="5f191-564">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-564">January 15, 2019</span></span>

<span data-ttu-id="5f191-565">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="5f191-565">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-566">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-566">ACR</span></span>
* <span data-ttu-id="5f191-567">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="5f191-567">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="5f191-568">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5f191-568">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="5f191-569">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="5f191-569">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="5f191-570">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-570">ACS</span></span>
* <span data-ttu-id="5f191-571">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="5f191-571">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-572">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-572">Appservice</span></span>
* <span data-ttu-id="5f191-573">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="5f191-573">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="5f191-574">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="5f191-574">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="5f191-575">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="5f191-575">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="5f191-576">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="5f191-576">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-577">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-577">Botservice</span></span>
* <span data-ttu-id="5f191-578">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-578">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="5f191-579">Настройка</span><span class="sxs-lookup"><span data-stu-id="5f191-579">Configure</span></span>
* <span data-ttu-id="5f191-580">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="5f191-580">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-581">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-581">CosmosDB</span></span>
* <span data-ttu-id="5f191-582">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="5f191-582">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f191-583">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f191-583">HDInsight</span></span>
* <span data-ttu-id="5f191-584">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="5f191-584">Added commands for managing applications</span></span>
* <span data-ttu-id="5f191-585">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="5f191-585">Added commands for managing script actions</span></span>
* <span data-ttu-id="5f191-586">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="5f191-586">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="5f191-587">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5f191-587">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="5f191-588">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-588">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-589">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-589">Network</span></span>
* <span data-ttu-id="5f191-590">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-590">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="5f191-591">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="5f191-591">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="5f191-592">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-592">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="5f191-593">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-593">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="5f191-594">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-594">Role</span></span>
* <span data-ttu-id="5f191-595">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f191-595">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="5f191-596">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="5f191-596">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="5f191-597">Безопасность</span><span class="sxs-lookup"><span data-stu-id="5f191-597">Security</span></span>
* <span data-ttu-id="5f191-598">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-598">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-599">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-599">Storage</span></span>
* <span data-ttu-id="5f191-600">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="5f191-600">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="5f191-601">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="5f191-601">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="5f191-602">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-602">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="5f191-603">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-603">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="5f191-604">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="5f191-604">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-605">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-605">VM</span></span>
* <span data-ttu-id="5f191-606">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="5f191-606">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="5f191-607">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-607">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f191-608">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="5f191-608">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="5f191-609">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="5f191-609">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="5f191-610">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-610">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="5f191-611">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f191-611">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="5f191-612">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-612">December 20, 2018</span></span>

<span data-ttu-id="5f191-613">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="5f191-613">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="5f191-614">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-614">Appservice</span></span>
* <span data-ttu-id="5f191-615">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="5f191-615">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="5f191-616">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5f191-616">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="5f191-617">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-617">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5f191-618">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f191-618">IoTCentral</span></span>
* <span data-ttu-id="5f191-619">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="5f191-619">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="5f191-620">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-620">Role</span></span>
* <span data-ttu-id="5f191-621">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-621">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-622">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-622">SQL</span></span>
* <span data-ttu-id="5f191-623">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="5f191-623">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-624">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-624">VM</span></span>
* <span data-ttu-id="5f191-625">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-625">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="5f191-626">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-626">December 18, 2018</span></span>

<span data-ttu-id="5f191-627">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="5f191-627">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="5f191-628">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-628">ACR</span></span>
* <span data-ttu-id="5f191-629">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-629">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="5f191-630">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="5f191-630">Condensed the table layout for task list</span></span>
* <span data-ttu-id="5f191-631">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="5f191-631">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-632">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-632">ACS</span></span>
* <span data-ttu-id="5f191-633">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-633">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5f191-634">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="5f191-634">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="5f191-635">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5f191-635">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="5f191-636">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-636">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="5f191-637">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="5f191-637">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="5f191-638">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-638">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-639">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-639">Appservice</span></span>
* <span data-ttu-id="5f191-640">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="5f191-640">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="5f191-641">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-641">Botservice</span></span>
* <span data-ttu-id="5f191-642">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-642">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="5f191-643">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="5f191-643">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="5f191-644">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="5f191-644">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="5f191-645">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="5f191-645">Reduced Kudu network calls</span></span>
* <span data-ttu-id="5f191-646">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-646">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-647">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-647">Consumption</span></span>
* <span data-ttu-id="5f191-648">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5f191-648">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-649">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-649">CosmosDB</span></span>
* <span data-ttu-id="5f191-650">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="5f191-650">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="5f191-651">Maps</span><span class="sxs-lookup"><span data-stu-id="5f191-651">Maps</span></span>
* <span data-ttu-id="5f191-652">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="5f191-652">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-653">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-653">Network</span></span>
* <span data-ttu-id="5f191-654">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="5f191-654">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="5f191-655">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="5f191-655">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-656">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-656">Resource</span></span>
* <span data-ttu-id="5f191-657">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-657">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="5f191-658">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-658">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-659">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-659">Storage</span></span>
*  <span data-ttu-id="5f191-660">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="5f191-660">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-661">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-661">VM</span></span>
* <span data-ttu-id="5f191-662">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-662">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="5f191-663">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-663">December 4, 2018</span></span>

<span data-ttu-id="5f191-664">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="5f191-664">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="5f191-665">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-665">Core</span></span>
* <span data-ttu-id="5f191-666">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-666">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="5f191-667">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="5f191-667">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-668">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-668">Appservice</span></span>
* <span data-ttu-id="5f191-669">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="5f191-669">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="5f191-670">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="5f191-670">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="5f191-671">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-671">Network</span></span>
* <span data-ttu-id="5f191-672">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="5f191-672">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="5f191-673">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-673">Role</span></span>
* <span data-ttu-id="5f191-674">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="5f191-674">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="5f191-675">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-675">VM</span></span>
* <span data-ttu-id="5f191-676">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f191-676">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="5f191-677">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="5f191-677">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="5f191-678">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="5f191-678">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="5f191-679">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="5f191-679">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="5f191-680">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-680">November 20, 2018</span></span>

<span data-ttu-id="5f191-681">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="5f191-681">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="5f191-682">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-682">Core</span></span>
* <span data-ttu-id="5f191-683">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="5f191-683">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-684">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-684">ACR</span></span>
* <span data-ttu-id="5f191-685">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="5f191-685">Added context token to task step</span></span>
* <span data-ttu-id="5f191-686">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-686">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="5f191-687">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5f191-687">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-688">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-688">Appservice</span></span>
* <span data-ttu-id="5f191-689">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="5f191-689">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="5f191-690">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-690">Updated the default `node_version`.</span></span> <span data-ttu-id="5f191-691">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="5f191-691">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="5f191-692">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="5f191-692">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="5f191-693">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5f191-693">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5f191-694">IotCentral</span><span class="sxs-lookup"><span data-stu-id="5f191-694">IotCentral</span></span>
* <span data-ttu-id="5f191-695">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5f191-695">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-696">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-696">KeyVault</span></span>
* <span data-ttu-id="5f191-697">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="5f191-697">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="5f191-698">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-698">Network</span></span>
* <span data-ttu-id="5f191-699">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-699">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="5f191-700">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="5f191-700">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="5f191-701">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="5f191-701">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="5f191-702">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="5f191-702">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-703">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f191-703">Rdbms</span></span>
* <span data-ttu-id="5f191-704">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5f191-704">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="5f191-705">RBAC:</span><span class="sxs-lookup"><span data-stu-id="5f191-705">Rbac</span></span>
* <span data-ttu-id="5f191-706">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-706">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="5f191-707">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="5f191-707">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="5f191-708">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-708">Storage</span></span>
* <span data-ttu-id="5f191-709">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="5f191-709">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="5f191-710">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-710">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="5f191-711">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5f191-711">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="5f191-712">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-712">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-713">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-713">VM</span></span>
* <span data-ttu-id="5f191-714">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="5f191-714">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="5f191-715">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="5f191-715">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="5f191-716">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="5f191-716">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="5f191-717">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="5f191-717">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="5f191-718">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-718">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="5f191-719">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-719">Added `snapshot wait` command</span></span>
* <span data-ttu-id="5f191-720">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-720">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="5f191-721">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-721">November 6, 2018</span></span>

<span data-ttu-id="5f191-722">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="5f191-722">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="5f191-723">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-723">Core</span></span>
* <span data-ttu-id="5f191-724">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="5f191-724">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-725">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-725">ACR</span></span>
* <span data-ttu-id="5f191-726">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="5f191-726">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="5f191-727">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="5f191-727">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-728">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-728">ACS</span></span>
* <span data-ttu-id="5f191-729">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-729">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="5f191-730">Помощник</span><span class="sxs-lookup"><span data-stu-id="5f191-730">Advisor</span></span>
* <span data-ttu-id="5f191-731">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="5f191-731">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-732">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-732">AMS</span></span>
* <span data-ttu-id="5f191-733">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="5f191-733">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="5f191-734">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="5f191-734">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="5f191-735">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-735">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="5f191-736">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="5f191-736">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="5f191-737">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="5f191-737">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="5f191-738">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="5f191-738">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="5f191-739">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="5f191-739">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="5f191-740">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="5f191-740">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="5f191-741">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="5f191-741">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="5f191-742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-742">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="5f191-743">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-743">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="5f191-744">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="5f191-744">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="5f191-745">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="5f191-745">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="5f191-746">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="5f191-746">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="5f191-747">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="5f191-747">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="5f191-748">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="5f191-748">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="5f191-749">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="5f191-749">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-750">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-750">AppService</span></span>
* <span data-ttu-id="5f191-751">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="5f191-751">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="5f191-752">Настройка</span><span class="sxs-lookup"><span data-stu-id="5f191-752">Configure</span></span>
* <span data-ttu-id="5f191-753">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-753">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="5f191-754">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-754">Container</span></span>
* <span data-ttu-id="5f191-755">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="5f191-755">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="5f191-756">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="5f191-756">EventHub</span></span>
* <span data-ttu-id="5f191-757">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-757">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-758">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-758">Interactive</span></span>
* <span data-ttu-id="5f191-759">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="5f191-759">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-760">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-760">Monitor</span></span>
* <span data-ttu-id="5f191-761">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-761">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-762">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-762">Network</span></span>
* <span data-ttu-id="5f191-763">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="5f191-763">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="5f191-764">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5f191-764">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="5f191-765">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-765">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="5f191-766">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-766">Profile</span></span>
* <span data-ttu-id="5f191-767">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-767">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-768">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-768">RDBMS</span></span>
* <span data-ttu-id="5f191-769">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="5f191-769">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-770">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-770">Resource</span></span>
* <span data-ttu-id="5f191-771">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-771">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="5f191-772">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-772">Role</span></span>
* <span data-ttu-id="5f191-773">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-773">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="5f191-774">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-774">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="5f191-775">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="5f191-775">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-776">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-776">Storage</span></span>
* <span data-ttu-id="5f191-777">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="5f191-777">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-778">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-778">VM</span></span>
* <span data-ttu-id="5f191-779">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="5f191-779">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="5f191-780">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="5f191-780">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="5f191-781">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="5f191-781">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="5f191-782">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="5f191-782">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="5f191-783">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-783">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="5f191-784">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="5f191-784">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="5f191-785">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-785">October 23, 2018</span></span>

<span data-ttu-id="5f191-786">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="5f191-786">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="5f191-787">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-787">Core</span></span>
* <span data-ttu-id="5f191-788">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5f191-788">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="5f191-789">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5f191-789">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-790">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-790">ACR</span></span>
* <span data-ttu-id="5f191-791">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="5f191-791">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-792">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-792">CDN</span></span>
* <span data-ttu-id="5f191-793">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-793">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5f191-794">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="5f191-794">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="5f191-795">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-795">Container</span></span>
* <span data-ttu-id="5f191-796">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="5f191-796">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="5f191-797">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="5f191-797">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="5f191-798">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-798">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="5f191-799">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-799">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="5f191-800">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="5f191-800">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="5f191-801">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="5f191-801">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="5f191-802">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-802">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-803">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-803">CosmosDB</span></span>
* <span data-ttu-id="5f191-804">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="5f191-804">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-805">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-805">Interactive</span></span>
* <span data-ttu-id="5f191-806">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="5f191-806">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f191-807">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f191-807">IoT Central</span></span>
* <span data-ttu-id="5f191-808">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="5f191-808">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="5f191-809">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="5f191-809">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-810">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-810">Monitor</span></span>
* <span data-ttu-id="5f191-811">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="5f191-811">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="5f191-812">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-812">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="5f191-813">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-813">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5f191-814">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-814">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="5f191-815">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="5f191-815">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="5f191-816">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="5f191-816">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="5f191-817">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="5f191-817">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="5f191-818">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-818">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5f191-819">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-819">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="5f191-820">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-820">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-821">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-821">Network</span></span>
* <span data-ttu-id="5f191-822">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5f191-822">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="5f191-823">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="5f191-823">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="5f191-824">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="5f191-824">ServiceBus</span></span>
* <span data-ttu-id="5f191-825">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5f191-825">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-826">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-826">SQL</span></span>
* <span data-ttu-id="5f191-827">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="5f191-827">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-828">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-828">Storage</span></span>
* <span data-ttu-id="5f191-829">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-829">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="5f191-830">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="5f191-830">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-831">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-831">VM</span></span>
* <span data-ttu-id="5f191-832">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="5f191-832">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f191-833">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="5f191-833">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="5f191-834">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="5f191-834">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="5f191-835">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-835">October 16, 2018</span></span>

<span data-ttu-id="5f191-836">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="5f191-836">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-837">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-837">VM</span></span>
* <span data-ttu-id="5f191-838">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5f191-838">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="5f191-839">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-839">October 9, 2018</span></span>

<span data-ttu-id="5f191-840">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="5f191-840">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="5f191-841">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-841">Core</span></span>
* <span data-ttu-id="5f191-842">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="5f191-842">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-843">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-843">ACR</span></span>
* <span data-ttu-id="5f191-844">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="5f191-844">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-845">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-845">ACS</span></span>
* <span data-ttu-id="5f191-846">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="5f191-846">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="5f191-847">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="5f191-847">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="5f191-848">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="5f191-848">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="5f191-849">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="5f191-849">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="5f191-850">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-850">Container</span></span>
* <span data-ttu-id="5f191-851">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="5f191-851">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="5f191-852">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-852">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="5f191-853">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="5f191-853">Event Hub</span></span>
* <span data-ttu-id="5f191-854">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-854">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="5f191-855">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5f191-855">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="5f191-856">расширения.</span><span class="sxs-lookup"><span data-stu-id="5f191-856">Extensions</span></span>
* <span data-ttu-id="5f191-857">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="5f191-857">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5f191-858">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5f191-858">HDInsight</span></span>
* <span data-ttu-id="5f191-859">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-859">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-860">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-860">IoT</span></span>
* <span data-ttu-id="5f191-861">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="5f191-861">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-862">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-862">KeyVault</span></span>
* <span data-ttu-id="5f191-863">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="5f191-863">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="5f191-864">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-864">Network</span></span>
* <span data-ttu-id="5f191-865">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-865">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="5f191-866">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="5f191-866">See #6052</span></span>
* <span data-ttu-id="5f191-867">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-867">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="5f191-868">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5f191-868">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="5f191-869">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5f191-869">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="5f191-870">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5f191-870">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="5f191-871">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="5f191-871">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="5f191-872">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-872">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="5f191-873">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-873">Role</span></span>
* <span data-ttu-id="5f191-874">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="5f191-874">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="5f191-875">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="5f191-875">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="5f191-876">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="5f191-876">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="5f191-877">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="5f191-877">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f191-878">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-878">Service Bus</span></span>
* <span data-ttu-id="5f191-879">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="5f191-879">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-880">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-880">VM</span></span>
* <span data-ttu-id="5f191-881">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="5f191-881">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="5f191-882">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="5f191-882">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="5f191-883">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="5f191-883">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="5f191-884">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="5f191-884">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="5f191-885">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="5f191-885">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="5f191-886">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="5f191-886">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="5f191-887">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-887">September 21, 2018</span></span>

<span data-ttu-id="5f191-888">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="5f191-888">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-889">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-889">ACR</span></span>
* <span data-ttu-id="5f191-890">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-890">Added ACR Task commands</span></span>
* <span data-ttu-id="5f191-891">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="5f191-891">Added quick run command</span></span>
* <span data-ttu-id="5f191-892">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="5f191-892">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="5f191-893">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-893">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="5f191-894">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="5f191-894">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="5f191-895">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="5f191-895">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-896">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-896">ACS</span></span>
* <span data-ttu-id="5f191-897">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="5f191-897">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="5f191-898">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="5f191-898">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-899">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-899">AppService</span></span>

* <span data-ttu-id="5f191-900">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="5f191-900">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="5f191-901">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="5f191-901">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="5f191-902">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-902">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="5f191-903">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="5f191-903">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-904">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-904">Batch</span></span>
* <span data-ttu-id="5f191-905">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="5f191-905">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="5f191-906">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="5f191-906">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="5f191-907">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-907">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="5f191-908">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="5f191-908">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f191-909">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-909">Batch AI</span></span> 
* <span data-ttu-id="5f191-910">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-910">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f191-911">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f191-911">Cognitive Services</span></span>
* <span data-ttu-id="5f191-912">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="5f191-912">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="5f191-913">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="5f191-913">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="5f191-914">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="5f191-914">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="5f191-915">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-915">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="5f191-916">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5f191-916">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="5f191-917">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5f191-917">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="5f191-918">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-918">Container</span></span>
* <span data-ttu-id="5f191-919">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-919">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="5f191-920">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="5f191-920">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="5f191-921">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5f191-921">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="5f191-922">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-922">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="5f191-923">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f191-923">Datalake</span></span>
* <span data-ttu-id="5f191-924">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5f191-924">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="5f191-925">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="5f191-925">Interactive Shell</span></span>
* <span data-ttu-id="5f191-926">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-926">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="5f191-927">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-927">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-928">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-928">IoT</span></span>
* <span data-ttu-id="5f191-929">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5f191-929">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f191-930">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5f191-930">Key Vault</span></span>
* <span data-ttu-id="5f191-931">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="5f191-931">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="5f191-932">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-932">Network</span></span>
* <span data-ttu-id="5f191-933">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5f191-933">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="5f191-934">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-934">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="5f191-935">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="5f191-935">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="5f191-936">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5f191-936">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="5f191-937">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-937">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="5f191-938">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-938">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="5f191-939">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="5f191-939">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="5f191-940">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="5f191-940">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="5f191-941">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="5f191-941">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="5f191-942">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="5f191-942">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="5f191-943">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="5f191-943">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="5f191-944">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="5f191-944">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="5f191-945">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="5f191-945">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="5f191-946">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="5f191-946">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="5f191-947">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="5f191-947">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="5f191-948">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5f191-948">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="5f191-949">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5f191-949">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="5f191-950">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5f191-950">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-951">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-951">RDBMS</span></span>
* <span data-ttu-id="5f191-952">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="5f191-952">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="5f191-953">резервирование.</span><span class="sxs-lookup"><span data-stu-id="5f191-953">Reservation</span></span>
* <span data-ttu-id="5f191-954">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-954">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="5f191-955">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="5f191-955">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="5f191-956">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="5f191-956">Manage App</span></span>
* <span data-ttu-id="5f191-957">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5f191-957">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="5f191-958">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="5f191-958">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="5f191-959">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-959">Role</span></span>
* <span data-ttu-id="5f191-960">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="5f191-960">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="5f191-961">SignalR</span><span class="sxs-lookup"><span data-stu-id="5f191-961">SignalR</span></span>
* <span data-ttu-id="5f191-962">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-962">First release</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-963">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-963">Storage</span></span>
* <span data-ttu-id="5f191-964">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="5f191-964">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="5f191-965">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="5f191-965">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-966">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-966">VM</span></span>
* <span data-ttu-id="5f191-967">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="5f191-967">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="5f191-968">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="5f191-968">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="5f191-969">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-969">August 28, 2018</span></span>

<span data-ttu-id="5f191-970">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="5f191-970">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="5f191-971">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-971">Core</span></span>

* <span data-ttu-id="5f191-972">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5f191-972">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="5f191-973">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f191-973">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-974">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-974">ACR</span></span>

* <span data-ttu-id="5f191-975">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="5f191-975">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="5f191-976">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="5f191-976">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-977">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-977">ACS</span></span>

* <span data-ttu-id="5f191-978">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="5f191-978">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="5f191-979">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="5f191-979">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-980">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-980">AppService</span></span>

* <span data-ttu-id="5f191-981">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="5f191-981">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="5f191-982">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="5f191-982">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="5f191-983">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-983">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="5f191-984">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="5f191-984">Backup</span></span>

* <span data-ttu-id="5f191-985">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-985">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="5f191-986">Служба Azure Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-986">Bot Service</span></span>

* <span data-ttu-id="5f191-987">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="5f191-987">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f191-988">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f191-988">Cognitive Services</span></span>

* <span data-ttu-id="5f191-989">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="5f191-989">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-990">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-990">IoT</span></span>

* <span data-ttu-id="5f191-991">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="5f191-991">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-992">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-992">Monitor</span></span>

* <span data-ttu-id="5f191-993">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-993">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="5f191-994">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="5f191-994">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f191-995">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-995">Network</span></span>

* <span data-ttu-id="5f191-996">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-996">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-997">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-997">Resource</span></span>

* <span data-ttu-id="5f191-998">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-998">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-999">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-999">Storage</span></span>

* <span data-ttu-id="5f191-1000">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-1000">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1001">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1001">VM</span></span>

* <span data-ttu-id="5f191-1002">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5f191-1002">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="5f191-1003">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1003">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="5f191-1004">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1004">Auguest 14, 2018</span></span>

<span data-ttu-id="5f191-1005">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="5f191-1005">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1006">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1006">Core</span></span>

* <span data-ttu-id="5f191-1007">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1007">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="5f191-1008">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="5f191-1008">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="5f191-1009">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="5f191-1009">Telemetry</span></span>

* <span data-ttu-id="5f191-1010">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1010">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1011">ACR</span></span>

* <span data-ttu-id="5f191-1012">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1012">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="5f191-1013">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1013">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1014">ACS</span></span>

* <span data-ttu-id="5f191-1015">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-1015">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="5f191-1016">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1016">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="5f191-1017">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5f191-1017">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="5f191-1018">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="5f191-1018">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="5f191-1019">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-1019">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="5f191-1020">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1020">AppService</span></span>

* <span data-ttu-id="5f191-1021">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1021">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="5f191-1022">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="5f191-1022">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="5f191-1023">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1023">BatchAI</span></span>

* <span data-ttu-id="5f191-1024">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="5f191-1024">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="5f191-1025">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1025">Container</span></span>

* <span data-ttu-id="5f191-1026">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="5f191-1026">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="5f191-1027">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-1027">IoT</span></span>

* <span data-ttu-id="5f191-1028">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1028">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="5f191-1029">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1029">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="5f191-1030">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f191-1030">Iot Central</span></span>

* <span data-ttu-id="5f191-1031">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="5f191-1031">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-1032">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-1032">KeyVault</span></span>


* <span data-ttu-id="5f191-1033">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1033">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="5f191-1034">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="5f191-1034">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="5f191-1035">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="5f191-1035">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="5f191-1036">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1036">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="5f191-1037">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1037">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="5f191-1038">Передача</span><span class="sxs-lookup"><span data-stu-id="5f191-1038">Relay</span></span>

* <span data-ttu-id="5f191-1039">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-1039">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1040">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1040">Sql</span></span>

* <span data-ttu-id="5f191-1041">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1041">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1042">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1042">Storage</span></span>

* <span data-ttu-id="5f191-1043">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="5f191-1043">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="5f191-1044">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="5f191-1044">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="5f191-1045">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1045">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="5f191-1046">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="5f191-1046">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="5f191-1047">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="5f191-1047">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1048">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1048">VM</span></span>

* <span data-ttu-id="5f191-1049">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="5f191-1049">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="5f191-1050">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1050">July 31, 2018</span></span>

<span data-ttu-id="5f191-1051">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="5f191-1051">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1052">ACR</span></span>

* <span data-ttu-id="5f191-1053">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1053">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="5f191-1054">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1054">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1055">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1055">ACS</span></span>

* <span data-ttu-id="5f191-1056">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="5f191-1056">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1057">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1057">Batch</span></span>

* <span data-ttu-id="5f191-1058">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="5f191-1058">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1059">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1059">Container</span></span>

* <span data-ttu-id="5f191-1060">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1060">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1061">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1061">Network</span></span>

* <span data-ttu-id="5f191-1062">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1062">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="5f191-1063">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1063">Resource</span></span>

* <span data-ttu-id="5f191-1064">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1064">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="5f191-1065">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="5f191-1065">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1066">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1066">Role</span></span>

* <span data-ttu-id="5f191-1067">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f191-1067">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="5f191-1068">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="5f191-1068">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="5f191-1069">Поиск</span><span class="sxs-lookup"><span data-stu-id="5f191-1069">Search</span></span>

* <span data-ttu-id="5f191-1070">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="5f191-1070">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f191-1071">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1071">Service Bus</span></span>

* <span data-ttu-id="5f191-1072">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="5f191-1072">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="5f191-1073">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="5f191-1073">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="5f191-1074">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="5f191-1074">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="5f191-1075">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1075">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1076">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1076">Storage</span></span>

* <span data-ttu-id="5f191-1077">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1077">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="5f191-1078">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="5f191-1078">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1079">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1079">VM</span></span>

* <span data-ttu-id="5f191-1080">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="5f191-1080">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="5f191-1081">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1081">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="5f191-1082">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5f191-1082">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="5f191-1083">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="5f191-1083">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="5f191-1084">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1084">July 18, 2018</span></span>

<span data-ttu-id="5f191-1085">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="5f191-1085">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1086">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1086">Core</span></span>

* <span data-ttu-id="5f191-1087">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="5f191-1087">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="5f191-1088">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="5f191-1088">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="5f191-1089">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5f191-1089">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1090">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1090">ACR</span></span>

* <span data-ttu-id="5f191-1091">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="5f191-1091">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="5f191-1092">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1092">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="5f191-1093">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1093">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="5f191-1094">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1094">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1095">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1095">ACS</span></span>

* <span data-ttu-id="5f191-1096">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="5f191-1096">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1097">AppService</span></span>

* <span data-ttu-id="5f191-1098">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="5f191-1098">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1099">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1099">Batch</span></span>

* <span data-ttu-id="5f191-1100">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5f191-1100">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="5f191-1101">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="5f191-1101">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f191-1102">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1102">Batch AI</span></span>

* <span data-ttu-id="5f191-1103">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1103">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1104">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1104">Container</span></span>

* <span data-ttu-id="5f191-1105">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="5f191-1105">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="5f191-1106">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="5f191-1106">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1107">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1107">Network</span></span>

* <span data-ttu-id="5f191-1108">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1108">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="5f191-1109">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1109">Added `network nic wait`</span></span>
* <span data-ttu-id="5f191-1110">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5f191-1110">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="5f191-1111">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="5f191-1111">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="5f191-1112">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1112">Resource</span></span>

* <span data-ttu-id="5f191-1113">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1113">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="5f191-1114">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1114">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="5f191-1115">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1115">Added `deployment wait` command</span></span>
* <span data-ttu-id="5f191-1116">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="5f191-1116">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1117">SQL</span></span>

* <span data-ttu-id="5f191-1118">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1118">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="5f191-1119">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1119">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="5f191-1120">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1120">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1121">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1121">Storage</span></span>

* <span data-ttu-id="5f191-1122">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1122">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1123">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1123">VM</span></span>

* <span data-ttu-id="5f191-1124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1124">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="5f191-1125">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1125">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="5f191-1126">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1126">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5f191-1127">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1127">July 3, 2018</span></span>

<span data-ttu-id="5f191-1128">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="5f191-1128">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="5f191-1129">AKS</span><span class="sxs-lookup"><span data-stu-id="5f191-1129">AKS</span></span>

* <span data-ttu-id="5f191-1130">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1130">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5f191-1131">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1131">July 3, 2018</span></span>

<span data-ttu-id="5f191-1132">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="5f191-1132">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1133">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1133">Core</span></span>

* <span data-ttu-id="5f191-1134">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1134">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1135">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1135">ACR</span></span>

* <span data-ttu-id="5f191-1136">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="5f191-1136">Added polling build status</span></span>
* <span data-ttu-id="5f191-1137">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="5f191-1137">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="5f191-1138">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1138">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1139">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1139">ACS</span></span>

* <span data-ttu-id="5f191-1140">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1140">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="5f191-1141">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1141">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="5f191-1142">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1142">Updated options for `aks browse` command.</span></span> <span data-ttu-id="5f191-1143">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1143">Added `--listen-port` support</span></span>
* <span data-ttu-id="5f191-1144">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1144">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="5f191-1145">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="5f191-1145">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="5f191-1146">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1146">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1147">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1147">AppService</span></span>

* <span data-ttu-id="5f191-1148">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1148">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="5f191-1149">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1149">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="5f191-1150">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="5f191-1150">Backup</span></span>

* <span data-ttu-id="5f191-1151">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="5f191-1151">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="5f191-1152">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1152">BatchAI</span></span>

* <span data-ttu-id="5f191-1153">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1153">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="5f191-1154">Облако</span><span class="sxs-lookup"><span data-stu-id="5f191-1154">Cloud</span></span>

* <span data-ttu-id="5f191-1155">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1155">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1156">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1156">Container</span></span>

* <span data-ttu-id="5f191-1157">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1157">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="5f191-1158">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1158">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="5f191-1159">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="5f191-1159">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1160">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1160">Extension</span></span>

* <span data-ttu-id="5f191-1161">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1161">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1162">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1162">Network</span></span>

* <span data-ttu-id="5f191-1163">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="5f191-1163">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-1164">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5f191-1164">Rdbms</span></span>

* <span data-ttu-id="5f191-1165">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1165">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1166">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1166">Resource</span></span>

* <span data-ttu-id="5f191-1167">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1167">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1168">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1168">VM</span></span>

* <span data-ttu-id="5f191-1169">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5f191-1169">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="5f191-1170">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1170">June 25, 2018</span></span>

<span data-ttu-id="5f191-1171">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="5f191-1171">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="5f191-1172">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="5f191-1172">CLI</span></span>

* <span data-ttu-id="5f191-1173">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1173">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5f191-1174">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1174">June 19, 2018</span></span>

<span data-ttu-id="5f191-1175">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5f191-1175">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1176">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1176">Core</span></span>

* <span data-ttu-id="5f191-1177">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1177">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1178">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1178">ACR</span></span>

* <span data-ttu-id="5f191-1179">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1179">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5f191-1180">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="5f191-1180">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1181">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1181">ACS</span></span>

* <span data-ttu-id="5f191-1182">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1182">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5f191-1183">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1183">Added `--update` support</span></span>
* <span data-ttu-id="5f191-1184">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1184">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5f191-1185">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1185">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5f191-1186">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1186">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5f191-1187">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1187">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5f191-1188">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1188">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5f191-1189">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1189">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1190">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1190">AppService</span></span>

* <span data-ttu-id="5f191-1191">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="5f191-1191">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5f191-1192">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1192">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1193">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1193">Batch</span></span>

* <span data-ttu-id="5f191-1194">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1194">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f191-1195">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1195">Batch AI</span></span>

* <span data-ttu-id="5f191-1196">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1196">Added support for workspaces.</span></span> <span data-ttu-id="5f191-1197">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1197">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5f191-1198">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1198">Added support for experiments.</span></span> <span data-ttu-id="5f191-1199">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="5f191-1199">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5f191-1200">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="5f191-1200">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5f191-1201">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1201">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5f191-1202">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1202">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5f191-1203">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1203">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="5f191-1204">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="5f191-1204">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5f191-1205">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1205">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5f191-1206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1206">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5f191-1207">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1207">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5f191-1208">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1208">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5f191-1209">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1209">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5f191-1210">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1210">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5f191-1211">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="5f191-1211">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5f191-1212">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1212">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5f191-1213">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="5f191-1213">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="5f191-1214">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="5f191-1214">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="5f191-1215">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="5f191-1215">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5f191-1216">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="5f191-1216">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5f191-1217">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="5f191-1217">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5f191-1218">Maps</span><span class="sxs-lookup"><span data-stu-id="5f191-1218">Maps</span></span>

* <span data-ttu-id="5f191-1219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1219">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1220">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1220">Network</span></span>

* <span data-ttu-id="5f191-1221">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="5f191-1221">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5f191-1222">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="5f191-1222">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5f191-1223">#6502</span><span class="sxs-lookup"><span data-stu-id="5f191-1223">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5f191-1224">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5f191-1224">Reservations</span></span>

* <span data-ttu-id="5f191-1225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1225">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5f191-1226">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1226">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5f191-1227">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1227">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5f191-1228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1228">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5f191-1229">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1229">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5f191-1230">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1230">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1231">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1231">Role</span></span>

* <span data-ttu-id="5f191-1232">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5f191-1232">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1233">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1233">SQL</span></span>

* <span data-ttu-id="5f191-1234">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1234">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1235">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1235">Storage</span></span>

* <span data-ttu-id="5f191-1236">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="5f191-1236">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1237">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1237">VM</span></span>

* <span data-ttu-id="5f191-1238">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1238">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5f191-1239">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1239">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5f191-1240">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="5f191-1240">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5f191-1241">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1241">June 13, 2018</span></span>

<span data-ttu-id="5f191-1242">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5f191-1242">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1243">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1243">Core</span></span>

* <span data-ttu-id="5f191-1244">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="5f191-1244">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5f191-1245">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1245">June 13, 2018</span></span>

<span data-ttu-id="5f191-1246">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5f191-1246">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5f191-1247">AKS</span><span class="sxs-lookup"><span data-stu-id="5f191-1247">AKS</span></span>

* <span data-ttu-id="5f191-1248">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="5f191-1248">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5f191-1249">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="5f191-1249">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="5f191-1250">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5f191-1250">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5f191-1251">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="5f191-1251">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5f191-1252">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f191-1252">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1253">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1253">AppService</span></span>

* <span data-ttu-id="5f191-1254">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="5f191-1254">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5f191-1255">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1255">June 5, 2018</span></span>

<span data-ttu-id="5f191-1256">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5f191-1256">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1257">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1257">Interactive</span></span>

* <span data-ttu-id="5f191-1258">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="5f191-1258">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5f191-1259">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1259">June 5, 2018</span></span>

<span data-ttu-id="5f191-1260">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5f191-1260">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1261">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1261">Core</span></span>

* <span data-ttu-id="5f191-1262">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="5f191-1262">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5f191-1263">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1263">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1264">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1264">ACR</span></span>

* <span data-ttu-id="5f191-1265">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="5f191-1265">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5f191-1266">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1266">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5f191-1267">AKS</span><span class="sxs-lookup"><span data-stu-id="5f191-1267">AKS</span></span>

* <span data-ttu-id="5f191-1268">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1268">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1269">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1269">Batch</span></span>

* <span data-ttu-id="5f191-1270">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5f191-1270">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-1271">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-1271">IOT</span></span>

* <span data-ttu-id="5f191-1272">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="5f191-1272">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1273">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1273">Network</span></span>

* <span data-ttu-id="5f191-1274">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1274">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5f191-1275">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="5f191-1275">Policy Insights</span></span>

* <span data-ttu-id="5f191-1276">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-1276">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5f191-1277">ARM</span><span class="sxs-lookup"><span data-stu-id="5f191-1277">ARM</span></span>

* <span data-ttu-id="5f191-1278">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1278">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1279">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1279">SQL</span></span>

* <span data-ttu-id="5f191-1280">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="5f191-1280">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5f191-1281">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="5f191-1281">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5f191-1282">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1282">Storage</span></span>

* <span data-ttu-id="5f191-1283">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1283">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1284">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1284">VM</span></span>

* <span data-ttu-id="5f191-1285">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1285">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5f191-1286">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1286">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5f191-1287">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1287">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5f191-1288">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1288">May 22, 2018</span></span>

<span data-ttu-id="5f191-1289">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5f191-1289">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1290">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1290">Core</span></span>

* <span data-ttu-id="5f191-1291">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1291">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1292">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1292">ACS</span></span>

* <span data-ttu-id="5f191-1293">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1293">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5f191-1294">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="5f191-1294">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1295">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-1295">AppService</span></span>

* <span data-ttu-id="5f191-1296">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="5f191-1296">Improved generic update commands</span></span>
* <span data-ttu-id="5f191-1297">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1297">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1298">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1298">Container</span></span>

* <span data-ttu-id="5f191-1299">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="5f191-1299">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5f191-1300">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1300">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1301">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1301">Extension</span></span>

* <span data-ttu-id="5f191-1302">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1302">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1303">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1303">Interactive</span></span>

* <span data-ttu-id="5f191-1304">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1304">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5f191-1305">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1305">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-1306">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-1306">KeyVault</span></span>

* <span data-ttu-id="5f191-1307">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="5f191-1307">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1308">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1308">Network</span></span>

* <span data-ttu-id="5f191-1309">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="5f191-1309">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5f191-1310">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="5f191-1310">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1311">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1311">SQL</span></span>

* <span data-ttu-id="5f191-1312">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="5f191-1312">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5f191-1313">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1313">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5f191-1314">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1314">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="5f191-1315">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="5f191-1315">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5f191-1316">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5f191-1316">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5f191-1317">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1317">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5f191-1318">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1318">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5f191-1319">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1319">`edition`.</span></span> <span data-ttu-id="5f191-1320">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1320">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5f191-1321">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1321">`elasticPoolName`.</span></span> <span data-ttu-id="5f191-1322">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1322">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5f191-1323">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="5f191-1323">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5f191-1324">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1324">`edition`.</span></span> <span data-ttu-id="5f191-1325">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1325">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5f191-1326">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1326">`dtu`.</span></span> <span data-ttu-id="5f191-1327">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1327">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5f191-1328">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1328">`databaseDtuMin`.</span></span> <span data-ttu-id="5f191-1329">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1329">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5f191-1330">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1330">`databaseDtuMax`.</span></span> <span data-ttu-id="5f191-1331">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1331">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5f191-1332">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1332">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5f191-1333">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1333">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1334">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1334">Storage</span></span>

* <span data-ttu-id="5f191-1335">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1335">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5f191-1336">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1336">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1337">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1337">VM</span></span>

* <span data-ttu-id="5f191-1338">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1338">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5f191-1339">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1339">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5f191-1340">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1340">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5f191-1341">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1341">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5f191-1342">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1342">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5f191-1343">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1343">May 7, 2018</span></span>

<span data-ttu-id="5f191-1344">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5f191-1344">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1345">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1345">Core</span></span>

* <span data-ttu-id="5f191-1346">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="5f191-1346">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5f191-1347">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1347">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5f191-1348">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1348">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5f191-1349">#5591</span><span class="sxs-lookup"><span data-stu-id="5f191-1349">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5f191-1350">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1350">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5f191-1351">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="5f191-1351">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5f191-1352">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="5f191-1352">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5f191-1353">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1353">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5f191-1354">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1354">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1355">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1355">ACR</span></span>

* <span data-ttu-id="5f191-1356">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-1356">Added ACR Build commands</span></span>
* <span data-ttu-id="5f191-1357">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5f191-1357">Improved resource not found error messages</span></span>
* <span data-ttu-id="5f191-1358">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="5f191-1358">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5f191-1359">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="5f191-1359">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5f191-1360">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="5f191-1360">Improved repository commands error messages</span></span>
* <span data-ttu-id="5f191-1361">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1361">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1362">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1362">ACS</span></span>

* <span data-ttu-id="5f191-1363">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1363">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5f191-1364">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="5f191-1364">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5f191-1365">AMS</span><span class="sxs-lookup"><span data-stu-id="5f191-1365">AMS</span></span>

* <span data-ttu-id="5f191-1366">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-1366">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1367">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1367">Appservice</span></span>

* <span data-ttu-id="5f191-1368">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5f191-1368">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5f191-1369">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1369">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5f191-1370">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="5f191-1370">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5f191-1371">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1371">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5f191-1372">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1372">Batch AI</span></span>

* <span data-ttu-id="5f191-1373">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="5f191-1373">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f191-1374">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f191-1374">Cognitive Services</span></span>

* <span data-ttu-id="5f191-1375">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="5f191-1375">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-1376">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-1376">Consumption</span></span>

* <span data-ttu-id="5f191-1377">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="5f191-1377">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1378">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1378">Container</span></span>

* <span data-ttu-id="5f191-1379">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1379">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5f191-1380">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-1380">Cosmos DB</span></span>

* <span data-ttu-id="5f191-1381">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-1381">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5f191-1382">DMS</span><span class="sxs-lookup"><span data-stu-id="5f191-1382">DMS</span></span>

* <span data-ttu-id="5f191-1383">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="5f191-1383">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1384">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1384">Extension</span></span>

* <span data-ttu-id="5f191-1385">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="5f191-1385">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1386">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1386">Interactive</span></span>

* <span data-ttu-id="5f191-1387">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="5f191-1387">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5f191-1388">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="5f191-1388">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5f191-1389">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1389">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5f191-1390">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1390">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5f191-1391">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5f191-1391">Lab</span></span>

* <span data-ttu-id="5f191-1392">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="5f191-1392">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1393">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1393">Network</span></span>

* <span data-ttu-id="5f191-1394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="5f191-1394">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5f191-1395">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1395">Profile</span></span>

* <span data-ttu-id="5f191-1396">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1396">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5f191-1397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="5f191-1397">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5f191-1398">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1398">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5f191-1399">Redis</span><span class="sxs-lookup"><span data-stu-id="5f191-1399">Redis</span></span>

* <span data-ttu-id="5f191-1400">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1400">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5f191-1401">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="5f191-1401">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5f191-1402">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1402">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5f191-1403">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1403">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5f191-1404">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1404">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1405">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1405">Role</span></span>

* <span data-ttu-id="5f191-1406">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="5f191-1406">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1407">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1407">Storage</span></span>

* <span data-ttu-id="5f191-1408">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="5f191-1408">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5f191-1409">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5f191-1409">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5f191-1410">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1410">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5f191-1411">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="5f191-1411">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5f191-1412">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="5f191-1412">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1413">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1413">VM</span></span>

* <span data-ttu-id="5f191-1414">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="5f191-1414">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5f191-1415">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="5f191-1415">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5f191-1416">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1416">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5f191-1417">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1417">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5f191-1418">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="5f191-1418">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5f191-1419">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="5f191-1419">Added write accelerator support</span></span>
* <span data-ttu-id="5f191-1420">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1420">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5f191-1421">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5f191-1421">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5f191-1422">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="5f191-1422">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5f191-1423">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1423">April 10, 2018</span></span>

<span data-ttu-id="5f191-1424">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5f191-1424">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1425">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1425">ACR</span></span>

* <span data-ttu-id="5f191-1426">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="5f191-1426">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1427">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1427">ACS</span></span>

* <span data-ttu-id="5f191-1428">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="5f191-1428">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1429">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1429">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5f191-1431">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1431">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5f191-1432">Batch AI</span><span class="sxs-lookup"><span data-stu-id="5f191-1432">BatchAI</span></span>

* <span data-ttu-id="5f191-1433">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="5f191-1433">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="5f191-1434">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="5f191-1434">Job level mounting</span></span>
  - <span data-ttu-id="5f191-1435">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1435">Environment variables with secret values</span></span>
  - <span data-ttu-id="5f191-1436">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="5f191-1436">Performance counters settings</span></span>
  - <span data-ttu-id="5f191-1437">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="5f191-1437">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="5f191-1438">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1438">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="5f191-1439">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="5f191-1439">Usage and limits reporting</span></span>
  - <span data-ttu-id="5f191-1440">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1440">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="5f191-1441">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1441">Support for custom images</span></span>
  - <span data-ttu-id="5f191-1442">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="5f191-1442">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5f191-1443">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="5f191-1443">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5f191-1444">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1444">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5f191-1445">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="5f191-1445">National clouds are supported</span></span>
* <span data-ttu-id="5f191-1446">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1446">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5f191-1447">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1447">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5f191-1448">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1448">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5f191-1449">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1449">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5f191-1450">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="5f191-1450">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5f191-1451">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="5f191-1451">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5f191-1452">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1452">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5f191-1453">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="5f191-1453">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5f191-1454">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="5f191-1454">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5f191-1455">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1455">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5f191-1456">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="5f191-1456">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5f191-1457">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1457">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5f191-1458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1458">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5f191-1459">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="5f191-1459">Billing</span></span>

* <span data-ttu-id="5f191-1460">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1460">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-1461">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-1461">Consumption</span></span>

* <span data-ttu-id="5f191-1462">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1462">Added `marketplace` commands</span></span>
* <span data-ttu-id="5f191-1463">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1463">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5f191-1464">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1464">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5f191-1465">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1465">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5f191-1466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1466">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5f191-1467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1467">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1468">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1468">Container</span></span>

* <span data-ttu-id="5f191-1469">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1469">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5f191-1470">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="5f191-1470">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1471">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1471">Extension</span></span>

* <span data-ttu-id="5f191-1472">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1472">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1473">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1473">Interactive</span></span>

* <span data-ttu-id="5f191-1474">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="5f191-1474">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5f191-1475">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1475">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5f191-1476">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1476">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1477">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1477">Network</span></span>

* <span data-ttu-id="5f191-1478">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1478">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5f191-1479">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1479">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="5f191-1480">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="5f191-1480">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="5f191-1481">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1481">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="5f191-1482">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1482">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5f191-1483">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1483">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5f191-1484">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1484">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5f191-1485">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="5f191-1485">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-1486">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1486">Profile</span></span>

* <span data-ttu-id="5f191-1487">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1487">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5f191-1488">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1488">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-1489">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-1489">RDBMS</span></span>

* <span data-ttu-id="5f191-1490">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1490">Added `georestore` command</span></span>
* <span data-ttu-id="5f191-1491">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="5f191-1491">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1492">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1492">Resource</span></span>

* <span data-ttu-id="5f191-1493">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1493">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5f191-1494">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1494">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1495">SQL</span></span>

* <span data-ttu-id="5f191-1496">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1496">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1497">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1497">Storage</span></span>

* <span data-ttu-id="5f191-1498">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="5f191-1498">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1499">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1499">VM</span></span>

* <span data-ttu-id="5f191-1500">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="5f191-1500">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5f191-1501">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1501">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="5f191-1503">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1503">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5f191-1504">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="5f191-1504">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="5f191-1505">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="5f191-1505">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="5f191-1506">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="5f191-1506">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5f191-1507">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1507">March 27, 2018</span></span>

<span data-ttu-id="5f191-1508">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5f191-1508">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1509">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1509">Core</span></span>

* <span data-ttu-id="5f191-1510">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5f191-1510">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1511">ACS</span></span>

* <span data-ttu-id="5f191-1512">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5f191-1512">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1513">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1513">Appservice</span></span>

* <span data-ttu-id="5f191-1514">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1514">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5f191-1515">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1515">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f191-1516">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="5f191-1516">Backup</span></span>

* <span data-ttu-id="5f191-1517">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1517">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5f191-1518">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="5f191-1518">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5f191-1519">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5f191-1519">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5f191-1520">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1520">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1521">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1521">Container</span></span>

* <span data-ttu-id="5f191-1522">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1522">Added `container exec` command.</span></span> <span data-ttu-id="5f191-1523">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1523">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5f191-1524">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1524">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1525">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1525">Extension</span></span>

* <span data-ttu-id="5f191-1526">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1526">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5f191-1527">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1527">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5f191-1528">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1528">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1529">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1529">Interactive</span></span>

* <span data-ttu-id="5f191-1530">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1530">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5f191-1531">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1531">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5f191-1532">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1532">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5f191-1533">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1533">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5f191-1534">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5f191-1534">Lab</span></span>

* <span data-ttu-id="5f191-1535">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1535">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1536">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1536">Monitor</span></span>

* <span data-ttu-id="5f191-1537">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="5f191-1537">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5f191-1538">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1538">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5f191-1539">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="5f191-1539">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1540">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1540">Network</span></span>

* <span data-ttu-id="5f191-1541">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1541">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-1542">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1542">Profile</span></span>

* <span data-ttu-id="5f191-1543">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1543">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-1544">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-1544">RDBMS</span></span>

* <span data-ttu-id="5f191-1545">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="5f191-1545">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1546">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1546">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5f191-1548">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1548">Role</span></span>

* <span data-ttu-id="5f191-1549">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1549">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5f191-1550">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="5f191-1550">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5f191-1551">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="5f191-1551">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5f191-1552">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1552">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5f191-1553">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1553">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1554">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1554">Storage</span></span>

* <span data-ttu-id="5f191-1555">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5f191-1555">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5f191-1556">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5f191-1556">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1557">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1557">VM</span></span>

* <span data-ttu-id="5f191-1558">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1558">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5f191-1559">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1559">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5f191-1560">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="5f191-1560">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5f191-1561">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="5f191-1561">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5f191-1562">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1562">March 13, 2018</span></span>

<span data-ttu-id="5f191-1563">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5f191-1563">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1564">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1564">ACR</span></span>

* <span data-ttu-id="5f191-1565">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1565">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5f191-1566">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5f191-1566">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5f191-1567">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-1567">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1568">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1568">ACS</span></span>

* <span data-ttu-id="5f191-1569">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="5f191-1569">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5f191-1570">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1570">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5f191-1571">Помощник</span><span class="sxs-lookup"><span data-stu-id="5f191-1571">Advisor</span></span>

* <span data-ttu-id="5f191-1572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1572">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5f191-1573">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1573">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5f191-1574">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1574">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="5f191-1575">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1575">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5f191-1576">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1576">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1577">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1577">Appservice</span></span>

* <span data-ttu-id="5f191-1578">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="5f191-1578">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5f191-1579">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1579">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5f191-1580">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="5f191-1580">Eventhubs</span></span>

* <span data-ttu-id="5f191-1581">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-1581">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1582">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1582">Extension</span></span>

* <span data-ttu-id="5f191-1583">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="5f191-1583">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1584">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1584">Interactive</span></span>

* <span data-ttu-id="5f191-1585">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="5f191-1585">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5f191-1586">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="5f191-1586">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5f191-1587">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="5f191-1587">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5f191-1588">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1588">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1589">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1589">Monitor</span></span>

* <span data-ttu-id="5f191-1590">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5f191-1590">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5f191-1591">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1591">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5f191-1592">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1592">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5f191-1593">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1593">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1594">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1594">Network</span></span>

* <span data-ttu-id="5f191-1595">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1595">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5f191-1596">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5f191-1596">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5f191-1597">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1597">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5f191-1598">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1598">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-1599">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1599">Profile</span></span>

* <span data-ttu-id="5f191-1600">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="5f191-1600">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5f191-1601">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1601">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-1602">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-1602">RDBMS</span></span>

* <span data-ttu-id="5f191-1603">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="5f191-1603">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5f191-1604">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1604">Service Bus</span></span>

* <span data-ttu-id="5f191-1605">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-1605">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1606">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1606">Storage</span></span>

* <span data-ttu-id="5f191-1607">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="5f191-1607">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5f191-1608">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1608">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1609">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1609">VM</span></span>

* <span data-ttu-id="5f191-1610">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="5f191-1610">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5f191-1611">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="5f191-1611">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5f191-1612">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1612">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5f191-1613">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="5f191-1613">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5f191-1614">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="5f191-1614">February 27, 2018</span></span>

<span data-ttu-id="5f191-1615">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5f191-1615">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1616">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1616">Core</span></span>

* <span data-ttu-id="5f191-1617">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="5f191-1617">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5f191-1618">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1618">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5f191-1619">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1619">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1620">ACS</span></span>

* <span data-ttu-id="5f191-1621">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1621">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5f191-1622">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1622">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5f191-1623">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1623">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5f191-1624">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1624">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1625">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1625">Appservice</span></span>

* <span data-ttu-id="5f191-1626">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5f191-1626">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5f191-1627">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="5f191-1627">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5f191-1628">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="5f191-1628">Cognitive Services</span></span>

* <span data-ttu-id="5f191-1629">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5f191-1629">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-1630">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-1630">Consumption</span></span>

* <span data-ttu-id="5f191-1631">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="5f191-1631">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5f191-1632">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="5f191-1632">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1633">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1633">Container</span></span>

* <span data-ttu-id="5f191-1634">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1634">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1635">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1635">Network</span></span>

* <span data-ttu-id="5f191-1636">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1636">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1637">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1637">Resource</span></span>

* <span data-ttu-id="5f191-1638">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="5f191-1638">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1639">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1639">Role</span></span>

* <span data-ttu-id="5f191-1640">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1640">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1641">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1641">SQL</span></span>

* <span data-ttu-id="5f191-1642">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1642">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1643">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1643">Storage</span></span>

* <span data-ttu-id="5f191-1644">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1644">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1645">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1645">VM</span></span>

* <span data-ttu-id="5f191-1646">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1646">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5f191-1647">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1647">February 13, 2018</span></span>

<span data-ttu-id="5f191-1648">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5f191-1648">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1649">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1649">Core</span></span>

* <span data-ttu-id="5f191-1650">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="5f191-1650">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1651">ACS</span></span>

* <span data-ttu-id="5f191-1652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="5f191-1652">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5f191-1653">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1653">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5f191-1654">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5f191-1654">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5f191-1655">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1655">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5f191-1656">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="5f191-1656">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5f191-1657">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1657">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5f191-1658">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5f191-1658">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5f191-1659">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1659">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1660">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1660">Appservice</span></span>

* <span data-ttu-id="5f191-1661">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1661">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5f191-1662">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1662">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-1663">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-1663">CDN</span></span>

* <span data-ttu-id="5f191-1664">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1664">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1665">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1665">Container</span></span>

* <span data-ttu-id="5f191-1666">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="5f191-1666">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5f191-1667">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1667">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-1668">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-1668">CosmosDB</span></span>

* <span data-ttu-id="5f191-1669">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1669">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1670">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1670">Extension</span></span>

* <span data-ttu-id="5f191-1671">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1671">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5f191-1672">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1672">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5f191-1673">Отзыв</span><span class="sxs-lookup"><span data-stu-id="5f191-1673">Feedback</span></span>

* <span data-ttu-id="5f191-1674">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1674">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1675">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1675">Interactive</span></span>

* <span data-ttu-id="5f191-1676">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5f191-1676">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5f191-1677">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1677">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-1678">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-1678">IoT</span></span>

* <span data-ttu-id="5f191-1679">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5f191-1679">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5f191-1680">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="5f191-1680">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5f191-1681">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1681">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5f191-1682">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1682">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1683">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1683">Monitor</span></span>

* <span data-ttu-id="5f191-1684">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1684">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1685">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1685">Network</span></span>

* <span data-ttu-id="5f191-1686">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="5f191-1686">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5f191-1687">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1687">Profile</span></span>

* <span data-ttu-id="5f191-1688">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5f191-1688">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1689">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1689">Resource</span></span>

* <span data-ttu-id="5f191-1690">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1690">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1691">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1691">Role</span></span>

* <span data-ttu-id="5f191-1692">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="5f191-1692">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1693">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1693">SQL</span></span>

* <span data-ttu-id="5f191-1694">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1694">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5f191-1695">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1695">Added `sql db rename`</span></span>
* <span data-ttu-id="5f191-1696">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="5f191-1696">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1697">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1697">Storage</span></span>

* <span data-ttu-id="5f191-1698">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="5f191-1698">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1699">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1699">VM</span></span>

* <span data-ttu-id="5f191-1700">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="5f191-1700">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5f191-1701">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1701">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5f191-1702">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="5f191-1702">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5f191-1703">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1703">January 31, 2018</span></span>

<span data-ttu-id="5f191-1704">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5f191-1704">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1705">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1705">Core</span></span>

* <span data-ttu-id="5f191-1706">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="5f191-1706">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5f191-1707">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-1707">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5f191-1708">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="5f191-1708">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5f191-1709">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="5f191-1709">Use `--verbose` to see</span></span>
* <span data-ttu-id="5f191-1710">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1710">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1711">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1711">ACS</span></span>

* <span data-ttu-id="5f191-1712">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1712">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5f191-1713">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1713">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1714">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1714">Appservice</span></span>

* <span data-ttu-id="5f191-1715">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1715">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5f191-1716">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="5f191-1716">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-1717">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-1717">CDN</span></span>

* <span data-ttu-id="5f191-1718">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1718">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-1719">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-1719">CosmosDB</span></span>

* <span data-ttu-id="5f191-1720">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1720">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1721">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1721">Interactive</span></span>

* <span data-ttu-id="5f191-1722">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="5f191-1722">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1723">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1723">Network</span></span>

* <span data-ttu-id="5f191-1724">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1724">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5f191-1725">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1725">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5f191-1726">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1726">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5f191-1727">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1727">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5f191-1728">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1728">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5f191-1729">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="5f191-1729">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5f191-1730">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="5f191-1730">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5f191-1731">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="5f191-1731">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5f191-1732">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1732">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="5f191-1733">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1733">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-1734">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1734">Profile</span></span>

* <span data-ttu-id="5f191-1735">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="5f191-1735">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1736">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1736">Resource</span></span>

* <span data-ttu-id="5f191-1737">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="5f191-1737">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1738">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1738">Storage</span></span>

* <span data-ttu-id="5f191-1739">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="5f191-1739">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5f191-1740">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="5f191-1740">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5f191-1741">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1741">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="5f191-1742">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1742">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5f191-1743">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="5f191-1743">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1744">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1744">VM</span></span>

* <span data-ttu-id="5f191-1745">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="5f191-1745">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5f191-1746">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1746">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5f191-1747">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1747">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5f191-1748">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1748">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5f191-1749">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1749">January 17, 2018</span></span>

<span data-ttu-id="5f191-1750">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5f191-1750">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1751">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1751">ACR</span></span>

* <span data-ttu-id="5f191-1752">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-1752">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5f191-1753">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="5f191-1753">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1754">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1754">ACS</span></span>

* <span data-ttu-id="5f191-1755">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1755">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5f191-1756">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1756">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1757">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1757">Appservice</span></span>

* <span data-ttu-id="5f191-1758">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="5f191-1758">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5f191-1759">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1759">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5f191-1760">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1760">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5f191-1761">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="5f191-1761">Backup</span></span>

* <span data-ttu-id="5f191-1762">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5f191-1762">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5f191-1763">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="5f191-1763">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5f191-1764">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="5f191-1764">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5f191-1765">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="5f191-1765">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5f191-1766">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="5f191-1766">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1767">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1767">Batch</span></span>

* <span data-ttu-id="5f191-1768">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1768">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5f191-1769">Облако</span><span class="sxs-lookup"><span data-stu-id="5f191-1769">Cloud</span></span>

* <span data-ttu-id="5f191-1770">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1770">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-1771">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-1771">Consumption</span></span>

* <span data-ttu-id="5f191-1772">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1772">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f191-1773">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1773">Event Grid</span></span>

* <span data-ttu-id="5f191-1774">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1774">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f191-1775">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1775">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f191-1776">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1776">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5f191-1777">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1777">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5f191-1778">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1778">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5f191-1779">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1779">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5f191-1780">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1780">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5f191-1781">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1781">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-1782">Interactive</span><span class="sxs-lookup"><span data-stu-id="5f191-1782">Interactive</span></span>

* <span data-ttu-id="5f191-1783">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="5f191-1783">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5f191-1784">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="5f191-1784">Fixed errors on startup</span></span>
* <span data-ttu-id="5f191-1785">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="5f191-1785">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-1786">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-1786">IoT</span></span>

* <span data-ttu-id="5f191-1787">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="5f191-1787">Added support for device provisioning service</span></span>
* <span data-ttu-id="5f191-1788">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="5f191-1788">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5f191-1789">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="5f191-1789">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1790">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1790">Monitor</span></span>

* <span data-ttu-id="5f191-1791">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1791">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5f191-1792">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1792">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5f191-1793">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="5f191-1793">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1794">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1794">Network</span></span>

* <span data-ttu-id="5f191-1795">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="5f191-1795">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5f191-1796">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="5f191-1796">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-1797">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-1797">Profile</span></span>

* <span data-ttu-id="5f191-1798">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1798">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1799">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1799">Role</span></span>

* <span data-ttu-id="5f191-1800">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1800">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f191-1801">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f191-1801">Service Fabric</span></span>

* <span data-ttu-id="5f191-1802">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="5f191-1802">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5f191-1803">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-1803">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1804">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1804">VM</span></span>

* <span data-ttu-id="5f191-1805">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1805">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5f191-1806">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="5f191-1806">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5f191-1807">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1807">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5f191-1808">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="5f191-1808">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5f191-1809">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="5f191-1809">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5f191-1810">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1810">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f191-1811">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1811">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f191-1812">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1812">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5f191-1813">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1813">December 19, 2017</span></span>

<span data-ttu-id="5f191-1814">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5f191-1814">Version 2.0.23</span></span>

* <span data-ttu-id="5f191-1815">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1815">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1816">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1816">Container</span></span>

* <span data-ttu-id="5f191-1817">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1817">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1818">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1818">Network</span></span>

* <span data-ttu-id="5f191-1819">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1819">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5f191-1820">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1820">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1821">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1821">Storage</span></span>

* <span data-ttu-id="5f191-1822">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="5f191-1822">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1823">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1823">VM</span></span>

* <span data-ttu-id="5f191-1824">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="5f191-1824">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5f191-1825">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1825">December 5, 2017</span></span>

<span data-ttu-id="5f191-1826">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5f191-1826">Version 2.0.22</span></span>

* <span data-ttu-id="5f191-1827">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1827">Removed `az component` commands.</span></span> <span data-ttu-id="5f191-1828">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1828">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1829">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1829">Core</span></span>
* <span data-ttu-id="5f191-1830">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="5f191-1830">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5f191-1831">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1831">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1832">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1832">ACS</span></span>

* <span data-ttu-id="5f191-1833">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1833">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5f191-1834">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1834">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5f191-1835">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="5f191-1835">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5f191-1836">Помощник</span><span class="sxs-lookup"><span data-stu-id="5f191-1836">Advisor</span></span>

* <span data-ttu-id="5f191-1837">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-1837">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1838">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1838">Appservice</span></span>

* <span data-ttu-id="5f191-1839">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1839">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5f191-1840">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1840">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5f191-1841">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1841">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5f191-1842">Потребление</span><span class="sxs-lookup"><span data-stu-id="5f191-1842">Consumption</span></span>

* <span data-ttu-id="5f191-1843">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="5f191-1843">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1844">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1844">Container</span></span>

* <span data-ttu-id="5f191-1845">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="5f191-1845">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1846">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1846">Monitor</span></span>

* <span data-ttu-id="5f191-1847">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="5f191-1847">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1848">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1848">Resource</span></span>

* <span data-ttu-id="5f191-1849">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="5f191-1849">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5f191-1850">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-1850">Role</span></span>

* <span data-ttu-id="5f191-1851">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1851">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5f191-1852">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="5f191-1852">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5f191-1853">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1853">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1854">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1854">SQL</span></span>

* <span data-ttu-id="5f191-1855">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1855">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5f191-1856">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1856">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1857">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1857">VM</span></span>

* <span data-ttu-id="5f191-1858">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1858">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5f191-1859">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1859">November 14, 2017</span></span>

<span data-ttu-id="5f191-1860">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5f191-1860">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1861">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1861">ACR</span></span>

* <span data-ttu-id="5f191-1862">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="5f191-1862">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5f191-1863">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1863">ACS</span></span>

* <span data-ttu-id="5f191-1864">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="5f191-1864">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5f191-1865">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="5f191-1865">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5f191-1866">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1866">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5f191-1867">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-1867">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5f191-1868">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-1868">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1869">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1869">Appservice</span></span>

* <span data-ttu-id="5f191-1870">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1870">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5f191-1871">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1871">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5f191-1872">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1872">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5f191-1873">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1873">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5f191-1874">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="5f191-1874">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5f191-1875">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="5f191-1875">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1876">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1876">Batch</span></span>

* <span data-ttu-id="5f191-1877">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1877">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5f191-1878">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5f191-1878">Batchai</span></span>

* <span data-ttu-id="5f191-1879">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1879">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5f191-1880">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1880">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5f191-1881">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1881">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5f191-1882">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1882">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5f191-1883">Облако</span><span class="sxs-lookup"><span data-stu-id="5f191-1883">Cloud</span></span>

* <span data-ttu-id="5f191-1884">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1884">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5f191-1885">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-1885">Container</span></span>

* <span data-ttu-id="5f191-1886">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1886">Added support to open multiple ports</span></span>
* <span data-ttu-id="5f191-1887">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-1887">Added container group restart policy</span></span>
* <span data-ttu-id="5f191-1888">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="5f191-1888">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5f191-1889">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="5f191-1889">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f191-1890">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f191-1890">Data Lake Analytics</span></span>

* <span data-ttu-id="5f191-1891">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1891">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f191-1892">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f191-1892">Data Lake Store</span></span>

* <span data-ttu-id="5f191-1893">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="5f191-1893">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-1894">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-1894">Extension</span></span>

* <span data-ttu-id="5f191-1895">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5f191-1895">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5f191-1896">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="5f191-1896">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-1897">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-1897">IoT</span></span>

* <span data-ttu-id="5f191-1898">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1898">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1899">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1899">Monitor</span></span>

* <span data-ttu-id="5f191-1900">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1900">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1901">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1901">Network</span></span>

* <span data-ttu-id="5f191-1902">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="5f191-1902">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5f191-1903">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1903">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5f191-1904">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="5f191-1904">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5f191-1905">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1905">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5f191-1906">Резервирование</span><span class="sxs-lookup"><span data-stu-id="5f191-1906">Reservations</span></span>

* <span data-ttu-id="5f191-1907">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="5f191-1907">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1908">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1908">Resource</span></span>

* <span data-ttu-id="5f191-1909">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1909">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1910">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1910">SQL</span></span>

* <span data-ttu-id="5f191-1911">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1911">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1912">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1912">Storage</span></span>

* <span data-ttu-id="5f191-1913">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-1913">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5f191-1914">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="5f191-1914">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5f191-1915">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1915">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5f191-1916">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1916">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5f191-1917">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1917">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5f191-1918">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1918">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5f191-1919">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1919">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1920">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1920">VM</span></span>

* <span data-ttu-id="5f191-1921">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1921">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5f191-1922">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1922">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5f191-1923">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1923">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5f191-1924">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1924">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5f191-1925">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5f191-1925">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5f191-1926">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1926">October 24, 2017</span></span>

<span data-ttu-id="5f191-1927">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5f191-1927">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1928">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1928">Core</span></span>

* <span data-ttu-id="5f191-1929">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="5f191-1929">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-1930">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-1930">ACR</span></span>

* <span data-ttu-id="5f191-1931">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="5f191-1931">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5f191-1932">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="5f191-1932">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5f191-1933">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="5f191-1933">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-1934">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-1934">ACS</span></span>

* <span data-ttu-id="5f191-1935">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="5f191-1935">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5f191-1936">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="5f191-1936">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1937">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1937">Appservice</span></span>

* <span data-ttu-id="5f191-1938">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="5f191-1938">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5f191-1939">Компонент</span><span class="sxs-lookup"><span data-stu-id="5f191-1939">Component</span></span>

* <span data-ttu-id="5f191-1940">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="5f191-1940">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-1941">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-1941">Monitor</span></span>

* <span data-ttu-id="5f191-1942">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1942">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1943">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1943">Resource</span></span>

* <span data-ttu-id="5f191-1944">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="5f191-1944">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5f191-1945">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="5f191-1945">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1946">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-1946">VM</span></span>

* <span data-ttu-id="5f191-1947">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f191-1947">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5f191-1948">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1948">October 9, 2017</span></span>

<span data-ttu-id="5f191-1949">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5f191-1949">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5f191-1950">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-1950">Core</span></span>

* <span data-ttu-id="5f191-1951">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="5f191-1951">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-1952">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-1952">Appservice</span></span>

* <span data-ttu-id="5f191-1953">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1953">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-1954">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-1954">Batch</span></span>

* <span data-ttu-id="5f191-1955">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5f191-1955">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5f191-1956">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="5f191-1956">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5f191-1957">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1957">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5f191-1958">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1958">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5f191-1959">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5f191-1959">Batchai</span></span>

* <span data-ttu-id="5f191-1960">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="5f191-1960">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-1961">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-1961">Keyvault</span></span>

* <span data-ttu-id="5f191-1962">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f191-1962">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5f191-1963">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5f191-1963">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5f191-1964">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1964">Network</span></span>

* <span data-ttu-id="5f191-1965">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="5f191-1965">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5f191-1966">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="5f191-1966">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1967">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1967">Resource</span></span>

* <span data-ttu-id="5f191-1968">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1968">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5f191-1969">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="5f191-1969">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5f191-1970">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="5f191-1970">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5f191-1971">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f191-1971">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-1972">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-1972">Sql</span></span>

* <span data-ttu-id="5f191-1973">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="5f191-1973">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5f191-1974">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-1974">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5f191-1975">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-1975">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1976">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1976">Storage</span></span>

* <span data-ttu-id="5f191-1977">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1977">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-1978">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="5f191-1978">Vm</span></span>

* <span data-ttu-id="5f191-1979">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="5f191-1979">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5f191-1980">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1980">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5f191-1981">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1981">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5f191-1982">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1982">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5f191-1983">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="5f191-1983">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5f191-1984">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-1984">September 22, 2017</span></span>

<span data-ttu-id="5f191-1985">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="5f191-1985">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-1986">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-1986">Resource</span></span>

* <span data-ttu-id="5f191-1987">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="5f191-1987">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5f191-1988">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="5f191-1988">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5f191-1989">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5f191-1989">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5f191-1990">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1990">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-1991">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-1991">Network</span></span>

* <span data-ttu-id="5f191-1992">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5f191-1992">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5f191-1993">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="5f191-1993">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5f191-1994">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="5f191-1994">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5f191-1995">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1995">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5f191-1996">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1996">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f191-1997">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-1997">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5f191-1998">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-1998">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-1999">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-1999">Storage</span></span>

* <span data-ttu-id="5f191-2000">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="5f191-2000">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f191-2001">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="5f191-2001">Eventgrid</span></span>

* <span data-ttu-id="5f191-2002">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="5f191-2002">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-2003">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-2003">SQL</span></span>

* <span data-ttu-id="5f191-2004">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="5f191-2004">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5f191-2005">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="5f191-2005">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5f191-2006">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f191-2006">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-2007">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-2007">Keyvault</span></span>

* <span data-ttu-id="5f191-2008">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="5f191-2008">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2009">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2009">VM</span></span>

* <span data-ttu-id="5f191-2010">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5f191-2010">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5f191-2011">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="5f191-2011">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5f191-2012">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f191-2012">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5f191-2013">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5f191-2013">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5f191-2014">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5f191-2014">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5f191-2015">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5f191-2015">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2016">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2016">ACS</span></span>

* <span data-ttu-id="5f191-2017">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="5f191-2017">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2018">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-2018">Appservice</span></span>

* <span data-ttu-id="5f191-2019">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5f191-2019">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f191-2020">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="5f191-2020">Backup</span></span>

* <span data-ttu-id="5f191-2021">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5f191-2021">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5f191-2022">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2022">September 11, 2017</span></span>

<span data-ttu-id="5f191-2023">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5f191-2023">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5f191-2024">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-2024">Core</span></span>

* <span data-ttu-id="5f191-2025">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="5f191-2025">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5f191-2026">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="5f191-2026">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2027">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2027">Acs</span></span>

* <span data-ttu-id="5f191-2028">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2028">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5f191-2029">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-2029">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2030">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-2030">Appservice</span></span>

* <span data-ttu-id="5f191-2031">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="5f191-2031">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-2032">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-2032">CDN</span></span>

* <span data-ttu-id="5f191-2033">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2033">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5f191-2034">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="5f191-2034">Extension</span></span>

* <span data-ttu-id="5f191-2035">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-2035">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-2036">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-2036">Keyvault</span></span>

* <span data-ttu-id="5f191-2037">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2037">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-2038">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-2038">Network</span></span>

* <span data-ttu-id="5f191-2039">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2039">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f191-2040">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2040">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5f191-2041">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2041">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5f191-2042">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2042">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f191-2043">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2043">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-2044">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-2044">Resource</span></span>

* <span data-ttu-id="5f191-2045">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2045">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5f191-2046">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2046">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5f191-2047">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="5f191-2047">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5f191-2048">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="5f191-2048">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-2049">SQL</span></span>

* <span data-ttu-id="5f191-2050">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2050">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2051">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2051">VM</span></span>

* <span data-ttu-id="5f191-2052">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="5f191-2052">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5f191-2053">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="5f191-2053">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5f191-2054">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2054">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5f191-2055">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="5f191-2055">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5f191-2056">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="5f191-2056">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5f191-2057">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2057">August 31, 2017</span></span>

<span data-ttu-id="5f191-2058">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5f191-2058">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-2059">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-2059">Keyvault</span></span>

* <span data-ttu-id="5f191-2060">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2060">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5f191-2061">Sf</span><span class="sxs-lookup"><span data-stu-id="5f191-2061">Sf</span></span>

* <span data-ttu-id="5f191-2062">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="5f191-2062">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-2063">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2063">Storage</span></span>

* <span data-ttu-id="5f191-2064">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="5f191-2064">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5f191-2065">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="5f191-2065">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5f191-2066">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2066">August 28, 2017</span></span>

<span data-ttu-id="5f191-2067">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5f191-2067">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5f191-2068">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="5f191-2068">CLI</span></span>

* <span data-ttu-id="5f191-2069">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="5f191-2069">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2070">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2070">ACS</span></span>

* <span data-ttu-id="5f191-2071">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5f191-2071">Corrected preview regions</span></span>
* <span data-ttu-id="5f191-2072">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2072">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5f191-2073">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="5f191-2073">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2074">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-2074">Appservice</span></span>

* <span data-ttu-id="5f191-2075">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2075">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5f191-2076">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2076">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5f191-2077">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2077">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5f191-2078">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="5f191-2078">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5f191-2079">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="5f191-2079">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-2080">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-2080">IoT</span></span>

* <span data-ttu-id="5f191-2081">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="5f191-2081">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5f191-2082">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-2082">Network</span></span>

* <span data-ttu-id="5f191-2083">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2083">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f191-2084">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2084">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5f191-2085">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2085">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f191-2086">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2086">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f191-2087">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2087">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-2088">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-2088">Profile</span></span>

* <span data-ttu-id="5f191-2089">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="5f191-2089">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f191-2090">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f191-2090">Service Fabric</span></span>

* <span data-ttu-id="5f191-2091">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="5f191-2091">Preview release</span></span>
* <span data-ttu-id="5f191-2092">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="5f191-2092">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5f191-2093">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="5f191-2093">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5f191-2094">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2094">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-2095">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2095">Storage</span></span>

* <span data-ttu-id="5f191-2096">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="5f191-2096">Enabled setting blob tier</span></span>
* <span data-ttu-id="5f191-2097">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-2097">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5f191-2098">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2098">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5f191-2099">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="5f191-2099">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5f191-2100">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2100">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5f191-2101">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2101">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2102">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2102">VM</span></span>

* <span data-ttu-id="5f191-2103">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2103">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5f191-2104">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2104">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5f191-2105">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="5f191-2105">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f191-2106">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="5f191-2106">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5f191-2107">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5f191-2107">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5f191-2108">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2108">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5f191-2109">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2109">August 15, 2017</span></span>

<span data-ttu-id="5f191-2110">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5f191-2110">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2111">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2111">ACS</span></span>

* <span data-ttu-id="5f191-2112">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="5f191-2112">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2113">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-2113">Appservice</span></span>

* <span data-ttu-id="5f191-2114">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="5f191-2114">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f191-2115">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-2115">Event Grid</span></span>

* <span data-ttu-id="5f191-2116">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5f191-2116">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5f191-2117">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2117">August 11, 2017</span></span>

<span data-ttu-id="5f191-2118">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5f191-2118">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2119">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2119">ACS</span></span>

* <span data-ttu-id="5f191-2120">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="5f191-2120">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-2121">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-2121">Batch</span></span>

* <span data-ttu-id="5f191-2122">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="5f191-2122">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5f191-2123">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="5f191-2123">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5f191-2124">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-2124">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5f191-2125">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="5f191-2125">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5f191-2126">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="5f191-2126">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5f191-2127">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2127">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5f191-2128">Компонент</span><span class="sxs-lookup"><span data-stu-id="5f191-2128">Component</span></span>

* <span data-ttu-id="5f191-2129">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="5f191-2129">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5f191-2130">Контейнер</span><span class="sxs-lookup"><span data-stu-id="5f191-2130">Container</span></span>

* <span data-ttu-id="5f191-2131">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="5f191-2131">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5f191-2132">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f191-2132">Data Lake Store</span></span>

* <span data-ttu-id="5f191-2133">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="5f191-2133">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f191-2134">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-2134">Event Grid</span></span>

* <span data-ttu-id="5f191-2135">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="5f191-2135">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5f191-2136">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-2136">Network</span></span>

* <span data-ttu-id="5f191-2137">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="5f191-2137">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5f191-2138">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2138">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5f191-2139">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2139">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5f191-2140">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2140">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-2141">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-2141">Profile</span></span>

* <span data-ttu-id="5f191-2142">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="5f191-2142">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-2143">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2143">Storage</span></span>

* <span data-ttu-id="5f191-2144">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="5f191-2144">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2145">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2145">VM</span></span>

* <span data-ttu-id="5f191-2146">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="5f191-2146">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5f191-2147">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2147">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5f191-2148">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="5f191-2148">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5f191-2149">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="5f191-2149">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5f191-2150">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="5f191-2150">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5f191-2151">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2151">July 28, 2017</span></span>

<span data-ttu-id="5f191-2152">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5f191-2152">Version 2.0.12</span></span>

* <span data-ttu-id="5f191-2153">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="5f191-2153">Added container commands</span></span>
* <span data-ttu-id="5f191-2154">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5f191-2154">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5f191-2155">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-2155">Core</span></span>

* <span data-ttu-id="5f191-2156">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5f191-2156">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5f191-2157">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="5f191-2157">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5f191-2158">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5f191-2158">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5f191-2159">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="5f191-2159">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5f191-2160">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="5f191-2160">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5f191-2161">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="5f191-2161">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5f191-2162">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5f191-2162">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f191-2163">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="5f191-2163">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5f191-2164">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="5f191-2164">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5f191-2165">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="5f191-2165">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5f191-2166">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="5f191-2166">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5f191-2167">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="5f191-2167">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5f191-2168">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5f191-2168">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5f191-2169">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="5f191-2169">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5f191-2170">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f191-2170">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5f191-2171">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="5f191-2171">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5f191-2172">ACR</span><span class="sxs-lookup"><span data-stu-id="5f191-2172">ACR</span></span>

* <span data-ttu-id="5f191-2173">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5f191-2173">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5f191-2174">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="5f191-2174">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5f191-2175">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="5f191-2175">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5f191-2176">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="5f191-2176">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5f191-2177">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="5f191-2177">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5f191-2178">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="5f191-2178">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2179">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2179">ACS</span></span>

* <span data-ttu-id="5f191-2180">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="5f191-2180">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2181">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="5f191-2181">Appservice</span></span>

* <span data-ttu-id="5f191-2182">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="5f191-2182">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5f191-2183">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="5f191-2183">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5f191-2184">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2184">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5f191-2185">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="5f191-2185">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5f191-2186">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="5f191-2186">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5f191-2187">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="5f191-2187">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5f191-2188">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="5f191-2188">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5f191-2189">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="5f191-2189">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5f191-2190">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="5f191-2190">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5f191-2191">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2191">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5f191-2192">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="5f191-2192">Batch</span></span>

* <span data-ttu-id="5f191-2193">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="5f191-2193">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5f191-2194">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2194">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5f191-2195">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2195">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f191-2196">CDN</span><span class="sxs-lookup"><span data-stu-id="5f191-2196">CDN</span></span>

* <span data-ttu-id="5f191-2197">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-2197">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5f191-2198">Облако</span><span class="sxs-lookup"><span data-stu-id="5f191-2198">Cloud</span></span>

* <span data-ttu-id="5f191-2199">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5f191-2199">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5f191-2200">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="5f191-2200">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5f191-2201">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="5f191-2201">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5f191-2202">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="5f191-2202">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5f191-2203">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2203">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-2204">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-2204">CosmosDB</span></span>

* <span data-ttu-id="5f191-2205">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="5f191-2205">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5f191-2206">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="5f191-2206">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f191-2207">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f191-2207">Data Lake Analytics</span></span>

* <span data-ttu-id="5f191-2208">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2208">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5f191-2209">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2209">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5f191-2210">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2210">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f191-2211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f191-2211">Data Lake Store</span></span>

* <span data-ttu-id="5f191-2212">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2212">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5f191-2213">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="5f191-2213">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5f191-2214">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2214">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5f191-2215">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f191-2215">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f191-2216">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="5f191-2216">Interactive</span></span>

* <span data-ttu-id="5f191-2217">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="5f191-2217">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5f191-2218">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="5f191-2218">Increased test coverage</span></span>
* <span data-ttu-id="5f191-2219">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="5f191-2219">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5f191-2220">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="5f191-2220">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5f191-2221">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="5f191-2221">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5f191-2222">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="5f191-2222">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5f191-2223">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="5f191-2223">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f191-2224">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2224">Added `--progress` flag</span></span>
* <span data-ttu-id="5f191-2225">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2225">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5f191-2226">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="5f191-2226">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5f191-2227">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="5f191-2227">IoT</span></span>

* <span data-ttu-id="5f191-2228">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="5f191-2228">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5f191-2229">(3934).</span><span class="sxs-lookup"><span data-stu-id="5f191-2229">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f191-2230">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-2230">Key vault</span></span>

* <span data-ttu-id="5f191-2231">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="5f191-2231">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5f191-2232">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2232">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5f191-2233">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="5f191-2233">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f191-2234">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="5f191-2234">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f191-2235">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2235">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5f191-2236">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="5f191-2236">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5f191-2237">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="5f191-2237">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5f191-2238">(3307).</span><span class="sxs-lookup"><span data-stu-id="5f191-2238">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5f191-2239">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5f191-2239">Lab</span></span>

* <span data-ttu-id="5f191-2240">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2240">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5f191-2241">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2241">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-2242">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-2242">Monitor</span></span>

* <span data-ttu-id="5f191-2243">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="5f191-2243">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5f191-2244">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2244">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5f191-2245">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2245">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5f191-2246">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2246">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5f191-2247">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2247">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5f191-2248">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="5f191-2248">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5f191-2249">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="5f191-2249">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5f191-2250">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="5f191-2250">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5f191-2251">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5f191-2251">`location` no longer required</span></span>
  * <span data-ttu-id="5f191-2252">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="5f191-2252">Add name and ID support for target</span></span>
  * <span data-ttu-id="5f191-2253">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="5f191-2253">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5f191-2254">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="5f191-2254">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5f191-2255">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="5f191-2255">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5f191-2256">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="5f191-2256">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5f191-2257">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2257">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5f191-2258">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2258">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5f191-2259">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-2259">Network</span></span>

* <span data-ttu-id="5f191-2260">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2260">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5f191-2261">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2261">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5f191-2262">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="5f191-2262">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5f191-2263">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2263">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5f191-2264">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2264">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5f191-2265">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2265">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5f191-2266">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2266">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5f191-2267">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2267">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5f191-2268">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2268">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5f191-2269">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2269">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5f191-2270">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2270">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5f191-2271">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2271">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5f191-2272">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2272">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5f191-2273">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2273">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5f191-2274">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2274">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5f191-2275">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2275">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5f191-2276">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="5f191-2276">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5f191-2277">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2277">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5f191-2278">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2278">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5f191-2279">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2279">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5f191-2280">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2280">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5f191-2281">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2281">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5f191-2282">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2282">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5f191-2283">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-2283">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5f191-2284">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5f191-2284">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5f191-2285">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="5f191-2285">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5f191-2286">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-2286">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-2287">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-2287">Profile</span></span>

* <span data-ttu-id="5f191-2288">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5f191-2288">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5f191-2289">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5f191-2289">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5f191-2290">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5f191-2290">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5f191-2291">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="5f191-2291">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5f191-2292">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="5f191-2292">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f191-2293">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="5f191-2293">RDBMS</span></span>

* <span data-ttu-id="5f191-2294">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="5f191-2294">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5f191-2295">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="5f191-2295">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5f191-2296">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="5f191-2296">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5f191-2297">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="5f191-2297">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-2298">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-2298">Resource</span></span>

* <span data-ttu-id="5f191-2299">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2299">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5f191-2300">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2300">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5f191-2301">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2301">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5f191-2302">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2302">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5f191-2303">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="5f191-2303">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5f191-2304">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2304">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5f191-2305">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="5f191-2305">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5f191-2306">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2306">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5f191-2307">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-2307">Role</span></span>

* <span data-ttu-id="5f191-2308">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="5f191-2308">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5f191-2309">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="5f191-2309">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5f191-2310">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="5f191-2310">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5f191-2311">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="5f191-2311">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5f191-2312">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2312">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f191-2313">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f191-2313">Service Fabric</span></span>
* <span data-ttu-id="5f191-2314">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="5f191-2314">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5f191-2315">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="5f191-2315">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5f191-2316">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="5f191-2316">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-2317">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-2317">SQL</span></span>

* <span data-ttu-id="5f191-2318">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2318">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5f191-2319">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2319">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5f191-2320">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2320">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-2321">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2321">Storage</span></span>

* <span data-ttu-id="5f191-2322">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="5f191-2322">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5f191-2323">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="5f191-2323">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5f191-2324">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="5f191-2324">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5f191-2325">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="5f191-2325">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5f191-2326">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="5f191-2326">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5f191-2327">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="5f191-2327">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2328">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2328">VM</span></span>

* <span data-ttu-id="5f191-2329">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="5f191-2329">Support configuring nsg</span></span>
* <span data-ttu-id="5f191-2330">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="5f191-2330">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5f191-2331">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="5f191-2331">Support managed service identities</span></span>
* <span data-ttu-id="5f191-2332">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2332">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5f191-2333">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="5f191-2333">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5f191-2334">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2334">May 10, 2017</span></span>

<span data-ttu-id="5f191-2335">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5f191-2335">Version 2.0.6</span></span>

* <span data-ttu-id="5f191-2336">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5f191-2336">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5f191-2337">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="5f191-2337">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5f191-2338">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5f191-2338">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5f191-2339">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="5f191-2339">Include Cognitive Services module</span></span>
* <span data-ttu-id="5f191-2340">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="5f191-2340">Include Service Fabric module</span></span>
* <span data-ttu-id="5f191-2341">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="5f191-2341">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5f191-2342">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="5f191-2342">Add support for CDN commands</span></span>
* <span data-ttu-id="5f191-2343">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="5f191-2343">Remove Container module</span></span>
* <span data-ttu-id="5f191-2344">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2344">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5f191-2345">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2345">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5f191-2346">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-2346">Core</span></span>

* <span data-ttu-id="5f191-2347">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="5f191-2347">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5f191-2348">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2348">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5f191-2349">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2349">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5f191-2350">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2350">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5f191-2351">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2351">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5f191-2352">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2352">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5f191-2353">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2353">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5f191-2354">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2354">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5f191-2355">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2355">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5f191-2356">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="5f191-2356">core: Improved performance</span></span>
* <span data-ttu-id="5f191-2357">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="5f191-2357">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5f191-2358">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="5f191-2358">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2359">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2359">ACS</span></span>

* <span data-ttu-id="5f191-2360">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="5f191-2360">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5f191-2361">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="5f191-2361">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5f191-2362">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="5f191-2362">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5f191-2363">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2363">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-2364">AppService</span></span>

* <span data-ttu-id="5f191-2365">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="5f191-2365">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5f191-2366">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2366">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5f191-2367">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="5f191-2367">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5f191-2368">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="5f191-2368">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5f191-2369">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="5f191-2369">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5f191-2370">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2370">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5f191-2371">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="5f191-2371">support slot swap with preview</span></span>
* <span data-ttu-id="5f191-2372">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2372">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5f191-2373">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2373">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f191-2374">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5f191-2374">CosmosDB</span></span>

* <span data-ttu-id="5f191-2375">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="5f191-2375">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5f191-2376">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="5f191-2376">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5f191-2377">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="5f191-2377">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5f191-2378">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="5f191-2378">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f191-2379">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f191-2379">Data Lake Analytics</span></span>

* <span data-ttu-id="5f191-2380">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="5f191-2380">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5f191-2381">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="5f191-2381">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5f191-2382">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2382">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5f191-2383">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="5f191-2383">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5f191-2384">Таблица</span><span class="sxs-lookup"><span data-stu-id="5f191-2384">Table</span></span>
  * <span data-ttu-id="5f191-2385">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="5f191-2385">Table valued function</span></span>
  * <span data-ttu-id="5f191-2386">Просмотр</span><span class="sxs-lookup"><span data-stu-id="5f191-2386">View</span></span>
  * <span data-ttu-id="5f191-2387">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="5f191-2387">Table Statistics.</span></span> <span data-ttu-id="5f191-2388">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="5f191-2388">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f191-2389">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f191-2389">Data Lake Store</span></span>

* <span data-ttu-id="5f191-2390">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="5f191-2390">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5f191-2391">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2391">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5f191-2392">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="5f191-2392">missed help for access show.</span></span> <span data-ttu-id="5f191-2393">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="5f191-2393">adding it.</span></span> <span data-ttu-id="5f191-2394">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5f191-2394">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5f191-2395">Поиск</span><span class="sxs-lookup"><span data-stu-id="5f191-2395">Find</span></span>

* <span data-ttu-id="5f191-2396">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="5f191-2396">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f191-2397">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="5f191-2397">KeyVault</span></span>

* <span data-ttu-id="5f191-2398">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="5f191-2398">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5f191-2399">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="5f191-2399">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5f191-2400">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="5f191-2400">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5f191-2401">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="5f191-2401">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5f191-2402">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2402">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5f191-2403">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="5f191-2403">Lab</span></span>

* <span data-ttu-id="5f191-2404">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5f191-2404">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5f191-2405">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5f191-2405">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5f191-2406">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5f191-2406">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5f191-2407">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5f191-2407">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5f191-2408">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="5f191-2408">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5f191-2409">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="5f191-2409">Monitor</span></span>

* <span data-ttu-id="5f191-2410">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2410">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5f191-2411">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2411">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5f191-2412">Network</span><span class="sxs-lookup"><span data-stu-id="5f191-2412">Network</span></span>

* <span data-ttu-id="5f191-2413">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2413">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5f191-2414">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2414">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5f191-2415">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2415">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5f191-2416">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2416">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5f191-2417">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5f191-2417">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5f191-2418">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="5f191-2418">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5f191-2419">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2419">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5f191-2420">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="5f191-2420">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5f191-2421">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2421">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5f191-2422">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="5f191-2422">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5f191-2423">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2423">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5f191-2424">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2424">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5f191-2425">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="5f191-2425">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5f191-2426">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="5f191-2426">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5f191-2427">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="5f191-2427">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5f191-2428">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="5f191-2428">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5f191-2429">Профиль</span><span class="sxs-lookup"><span data-stu-id="5f191-2429">Profile</span></span>

* <span data-ttu-id="5f191-2430">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2430">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5f191-2431">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2431">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5f191-2432">Redis</span><span class="sxs-lookup"><span data-stu-id="5f191-2432">Redis</span></span>

* <span data-ttu-id="5f191-2433">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="5f191-2433">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5f191-2434">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="5f191-2434">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5f191-2435">Ресурс</span><span class="sxs-lookup"><span data-stu-id="5f191-2435">Resource</span></span>

* <span data-ttu-id="5f191-2436">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2436">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5f191-2437">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2437">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5f191-2438">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2438">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5f191-2439">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="5f191-2439">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5f191-2440">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5f191-2440">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5f191-2441">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="5f191-2441">Add docs for az lock update.</span></span> <span data-ttu-id="5f191-2442">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5f191-2442">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5f191-2443">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="5f191-2443">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5f191-2444">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5f191-2444">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5f191-2445">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="5f191-2445">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5f191-2446">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5f191-2446">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5f191-2447">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2447">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5f191-2448">Роль</span><span class="sxs-lookup"><span data-stu-id="5f191-2448">Role</span></span>

* <span data-ttu-id="5f191-2449">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2449">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5f191-2450">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2450">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5f191-2451">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2451">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5f191-2452">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="5f191-2452">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5f191-2453">SQL</span><span class="sxs-lookup"><span data-stu-id="5f191-2453">SQL</span></span>

* <span data-ttu-id="5f191-2454">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="5f191-2454">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5f191-2455">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2455">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5f191-2456">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2456">Storage</span></span>

* <span data-ttu-id="5f191-2457">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2457">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5f191-2458">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-2458">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5f191-2459">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="5f191-2459">Add support for large block blob upload</span></span>
* <span data-ttu-id="5f191-2460">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="5f191-2460">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2461">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2461">VM</span></span>

* <span data-ttu-id="5f191-2462">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="5f191-2462">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5f191-2463">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="5f191-2463">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5f191-2464">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5f191-2464">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5f191-2465">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5f191-2465">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5f191-2466">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="5f191-2466">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5f191-2467">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="5f191-2467">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5f191-2468">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2468">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5f191-2469">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2469">April 3, 2017</span></span>

<span data-ttu-id="5f191-2470">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5f191-2470">Version 2.0.2</span></span>

<span data-ttu-id="5f191-2471">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="5f191-2471">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5f191-2472">Core</span><span class="sxs-lookup"><span data-stu-id="5f191-2472">Core</span></span>

* <span data-ttu-id="5f191-2473">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-2473">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5f191-2474">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2474">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5f191-2475">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2475">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5f191-2476">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2476">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f191-2477">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2477">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5f191-2478">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="5f191-2478">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5f191-2479">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2479">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5f191-2480">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f191-2480">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5f191-2481">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="5f191-2481">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5f191-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="5f191-2482">ACS</span></span>

* <span data-ttu-id="5f191-2483">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2483">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5f191-2484">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="5f191-2484">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5f191-2485">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2485">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5f191-2486">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="5f191-2486">Add support for windows clusters.</span></span> <span data-ttu-id="5f191-2487">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2487">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5f191-2488">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="5f191-2488">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5f191-2489">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2489">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f191-2490">AppService</span><span class="sxs-lookup"><span data-stu-id="5f191-2490">AppService</span></span>

* <span data-ttu-id="5f191-2491">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2491">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5f191-2492">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2492">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5f191-2493">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2493">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5f191-2494">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2494">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5f191-2495">Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f191-2495">DataLake</span></span>

* <span data-ttu-id="5f191-2496">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5f191-2496">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5f191-2497">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f191-2497">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5f191-2498">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="5f191-2498">DocuemntDB</span></span>

* <span data-ttu-id="5f191-2499">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2499">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5f191-2500">ВМ</span><span class="sxs-lookup"><span data-stu-id="5f191-2500">VM</span></span>

* <span data-ttu-id="5f191-2501">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2501">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5f191-2502">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2502">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5f191-2503">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2503">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5f191-2504">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2504">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f191-2505">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2505">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5f191-2506">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2506">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="5f191-2507">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="5f191-2507">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5f191-2508">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="5f191-2508">February 27, 2017</span></span>

<span data-ttu-id="5f191-2509">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5f191-2509">Version 2.0.0</span></span>

<span data-ttu-id="5f191-2510">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="5f191-2510">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5f191-2511">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="5f191-2511">Container Service (acs)</span></span>
- <span data-ttu-id="5f191-2512">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="5f191-2512">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5f191-2513">Сеть</span><span class="sxs-lookup"><span data-stu-id="5f191-2513">Networking</span></span>
- <span data-ttu-id="5f191-2514">Хранилище</span><span class="sxs-lookup"><span data-stu-id="5f191-2514">Storage</span></span>

<span data-ttu-id="5f191-2515">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2515">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5f191-2516">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="5f191-2516">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5f191-2517">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="5f191-2517">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5f191-2518">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="5f191-2518">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5f191-2519">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5f191-2519">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5f191-2520">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="5f191-2520">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5f191-2521">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="5f191-2521">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5f191-2522">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="5f191-2522">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5f191-2523">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f191-2523">Provide feedback from the command line with the `az feedback` command</span></span>

