---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/06/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ce11abccc23ee1f150916ef2f91dc895d4664d31
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240520"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="a6a88-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a6a88-103">Azure CLI release notes</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="a6a88-104">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-104">May 6, 2019</span></span>

<span data-ttu-id="a6a88-105">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="a6a88-105">Version 2.0.64</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-106">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-106">Appservice</span></span>
* <span data-ttu-id="a6a88-107">Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="a6a88-107">Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="a6a88-108">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-108">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="a6a88-109">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-109">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="a6a88-110">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-110">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="a6a88-111">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-111">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="a6a88-112">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-112">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="a6a88-113">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="a6a88-113">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="a6a88-114">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="a6a88-114">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="a6a88-115">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-115">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="a6a88-116">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-116">Added `create-remote-connection` command</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-117">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-117">Role</span></span>
* <span data-ttu-id="a6a88-118">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="a6a88-118">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="a6a88-119">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-119">April 23, 2019</span></span>

<span data-ttu-id="a6a88-120">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="a6a88-120">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-121">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-121">ACS</span></span>
* <span data-ttu-id="a6a88-122">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-122">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="a6a88-123">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="a6a88-123">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-124">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-124">AMS</span></span>
* <span data-ttu-id="a6a88-125">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-125">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-126">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-126">AppService</span></span>
* <span data-ttu-id="a6a88-127">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-127">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="a6a88-128">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-128">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="a6a88-129">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="a6a88-129">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="a6a88-130">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="a6a88-130">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="a6a88-131">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-131">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="a6a88-132">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-132">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="a6a88-133">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="a6a88-133">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="a6a88-134">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="a6a88-134">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="a6a88-135">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-135">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="a6a88-136">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="a6a88-136">Deployment Manager</span></span>
* <span data-ttu-id="a6a88-137">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="a6a88-137">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="a6a88-138">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a6a88-138">Lab</span></span>
* <span data-ttu-id="a6a88-139">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-139">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-140">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-140">Network</span></span>
* <span data-ttu-id="a6a88-141">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="a6a88-141">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-142">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-142">Resource</span></span>
* <span data-ttu-id="a6a88-143">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-143">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="a6a88-144">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-144">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="a6a88-145">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="a6a88-145">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="a6a88-146">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="a6a88-146">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-147">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-147">SQL</span></span>
* <span data-ttu-id="a6a88-148">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-148">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="a6a88-149">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-149">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="a6a88-150">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-150">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="a6a88-151">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-151">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-152">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-152">Storage</span></span>
* <span data-ttu-id="a6a88-153">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-153">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-154">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-154">VM</span></span>
* <span data-ttu-id="a6a88-155">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-155">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="a6a88-156">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-156">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="a6a88-157">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="a6a88-157">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="a6a88-158">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-158">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-159">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-159">Core</span></span>
* <span data-ttu-id="a6a88-160">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="a6a88-160">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-161">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-161">ACR</span></span>
* <span data-ttu-id="a6a88-162">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="a6a88-162">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-163">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-163">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="a6a88-166">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-166">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="a6a88-167">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-167">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-168">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-168">AppService</span></span>
* <span data-ttu-id="a6a88-169">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-169">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="a6a88-170">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-170">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="a6a88-171">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-171">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="a6a88-172">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-172">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="a6a88-173">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="a6a88-173">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="a6a88-174">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-174">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="a6a88-175">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-175">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-176">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-176">CDN</span></span>
* <span data-ttu-id="a6a88-177">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-177">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="a6a88-178">Отзыв</span><span class="sxs-lookup"><span data-stu-id="a6a88-178">Feedback</span></span>
* <span data-ttu-id="a6a88-179">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-179">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="a6a88-180">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-180">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="a6a88-181">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="a6a88-181">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-182">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-182">Monitor</span></span>
* <span data-ttu-id="a6a88-183">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-183">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="a6a88-184">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-184">Network</span></span>
* <span data-ttu-id="a6a88-185">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-185">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="a6a88-186">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-186">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="a6a88-187">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-187">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="a6a88-188">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-188">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="a6a88-189">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="a6a88-189">PrivateDNS</span></span>
* <span data-ttu-id="a6a88-190">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-190">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-191">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-191">Resource</span></span>
* <span data-ttu-id="a6a88-192">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="a6a88-192">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-193">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-193">Role</span></span>
* <span data-ttu-id="a6a88-194">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="a6a88-194">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="a6a88-195">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="a6a88-195">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-196">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-196">SQL</span></span>
* <span data-ttu-id="a6a88-197">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="a6a88-197">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-198">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-198">Storage</span></span>
* <span data-ttu-id="a6a88-199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-199">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="a6a88-200">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-200">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="a6a88-201">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="a6a88-201">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="a6a88-202">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a6a88-202">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="a6a88-203">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-203">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="a6a88-204">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-204">Core</span></span>
* <span data-ttu-id="a6a88-205">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-205">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="a6a88-206">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="a6a88-206">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="a6a88-207">Облако</span><span class="sxs-lookup"><span data-stu-id="a6a88-207">Cloud</span></span>
* <span data-ttu-id="a6a88-208">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-208">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-209">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-209">ACR</span></span>
* <span data-ttu-id="a6a88-210">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-210">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="a6a88-211">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-211">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="a6a88-212">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-212">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="a6a88-213">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-213">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-214">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-214">AppService</span></span>
* <span data-ttu-id="a6a88-215">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="a6a88-215">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="a6a88-216">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-216">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="a6a88-217">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-217">BOT Service</span></span>
* <span data-ttu-id="a6a88-218">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-218">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="a6a88-219">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="a6a88-219">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="a6a88-220">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-220">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="a6a88-221">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="a6a88-221">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-222">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-222">CDN</span></span>
* <span data-ttu-id="a6a88-223">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-223">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="a6a88-224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-224">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="a6a88-225">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-225">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a6a88-226">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="a6a88-226">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-227">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-227">Cosmosdb</span></span>
* <span data-ttu-id="a6a88-228">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-228">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="a6a88-229">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="a6a88-229">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-230">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-230">Interactive</span></span>
* <span data-ttu-id="a6a88-231">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="a6a88-231">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-232">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-232">Monitor</span></span>
* <span data-ttu-id="a6a88-233">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-233">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-234">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-234">Network</span></span>
* <span data-ttu-id="a6a88-235">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-235">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-236">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-236">Profile</span></span>
* <span data-ttu-id="a6a88-237">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-237">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="a6a88-238">Postgres</span><span class="sxs-lookup"><span data-stu-id="a6a88-238">Postgres</span></span> 
* <span data-ttu-id="a6a88-239">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-239">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="a6a88-240">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-240">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-241">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-241">Resource</span></span>
* <span data-ttu-id="a6a88-242">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-242">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="a6a88-243">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="a6a88-243">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="a6a88-244">График</span><span class="sxs-lookup"><span data-stu-id="a6a88-244">Graph</span></span>
* <span data-ttu-id="a6a88-245">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-245">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="a6a88-246">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-246">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="a6a88-247">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-247">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="a6a88-248">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-248">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="a6a88-249">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="a6a88-249">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-250">storage</span><span class="sxs-lookup"><span data-stu-id="a6a88-250">storage</span></span>
* <span data-ttu-id="a6a88-251">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-251">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="a6a88-252">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="a6a88-252">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="a6a88-253">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-253">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="a6a88-254">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="a6a88-254">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-255">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-255">VM</span></span>
* <span data-ttu-id="a6a88-256">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-256">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="a6a88-257">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-257">March 12, 2019</span></span>

<span data-ttu-id="a6a88-258">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="a6a88-258">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-259">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-259">Core</span></span>

* <span data-ttu-id="a6a88-260">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="a6a88-260">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-261">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-261">ACR</span></span>

* <span data-ttu-id="a6a88-262">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-262">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-263">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-263">ACS</span></span>

* <span data-ttu-id="a6a88-264">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="a6a88-264">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="a6a88-265">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-265">AppService</span></span>

* <span data-ttu-id="a6a88-266">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-266">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="a6a88-267">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-267">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="a6a88-268">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="a6a88-268">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="a6a88-269">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="a6a88-269">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="a6a88-270">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-270">Botservice</span></span>

* <span data-ttu-id="a6a88-271">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="a6a88-271">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a6a88-272">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="a6a88-272">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a6a88-273">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-273">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="a6a88-274">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-274">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-275">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-275">Container</span></span>

* <span data-ttu-id="a6a88-276">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-276">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="a6a88-277">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="a6a88-277">EventHub</span></span>

* <span data-ttu-id="a6a88-278">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-278">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="a6a88-279">Поиск</span><span class="sxs-lookup"><span data-stu-id="a6a88-279">Find</span></span>

* <span data-ttu-id="a6a88-280">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="a6a88-280">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6a88-281">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6a88-281">HDInsight</span></span>

* <span data-ttu-id="a6a88-282">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-282">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-283">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-283">Network</span></span>

* <span data-ttu-id="a6a88-284">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-284">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-285">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6a88-285">Rdbms</span></span>

* <span data-ttu-id="a6a88-286">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-286">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-287">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-287">Role</span></span>

* <span data-ttu-id="a6a88-288">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-288">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="a6a88-289">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-289">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6a88-290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6a88-290">Service Fabric</span></span>

* <span data-ttu-id="a6a88-291">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-291">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="a6a88-292">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-292">February 26, 2019</span></span>

<span data-ttu-id="a6a88-293">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="a6a88-293">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-294">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-294">Core</span></span>

* <span data-ttu-id="a6a88-295">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="a6a88-295">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-296">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-296">ACR</span></span>

* <span data-ttu-id="a6a88-297">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-297">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="a6a88-298">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-298">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-299">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-299">ACS</span></span>

* <span data-ttu-id="a6a88-300">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-300">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-301">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-301">AppService</span></span>

* <span data-ttu-id="a6a88-302">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-302">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-303">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-303">Batch</span></span>
* <span data-ttu-id="a6a88-304">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-304">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="a6a88-305">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-305">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="a6a88-306">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-306">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="a6a88-307">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-307">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="a6a88-308">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="a6a88-308">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="a6a88-309">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a6a88-309">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-310">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-310">CosmosDB</span></span>

* <span data-ttu-id="a6a88-311">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="a6a88-311">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="a6a88-312">Kusto</span><span class="sxs-lookup"><span data-stu-id="a6a88-312">Kusto</span></span>

* <span data-ttu-id="a6a88-313">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="a6a88-313">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-314">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-314">Network</span></span>

* <span data-ttu-id="a6a88-315">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-315">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="a6a88-316">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-316">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="a6a88-317">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-317">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="a6a88-318">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-318">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="a6a88-319">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-319">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="a6a88-320">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-320">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="a6a88-321">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-321">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-322">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-322">Resource</span></span>

* <span data-ttu-id="a6a88-323">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="a6a88-323">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="a6a88-324">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-324">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="a6a88-325">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-325">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="a6a88-326">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-326">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="a6a88-327">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-327">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-328">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-328">Role</span></span>

* <span data-ttu-id="a6a88-329">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-329">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-330">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-330">VM</span></span>

* <span data-ttu-id="a6a88-331">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="a6a88-331">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="a6a88-332">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-332">February 12, 2019</span></span>

<span data-ttu-id="a6a88-333">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="a6a88-333">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-334">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-334">Core</span></span>

* <span data-ttu-id="a6a88-335">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="a6a88-335">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="a6a88-336">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="a6a88-336">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-337">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-337">ACR</span></span>
* <span data-ttu-id="a6a88-338">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-338">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="a6a88-339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-339">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-340">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-340">ACS</span></span>
* <span data-ttu-id="a6a88-341">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-341">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="a6a88-342">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-342">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="a6a88-343">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="a6a88-343">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-344">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-344">AMS</span></span>
* <span data-ttu-id="a6a88-345">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-345">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="a6a88-346">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-346">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-347">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-347">Appservice</span></span>
* <span data-ttu-id="a6a88-348">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-348">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="a6a88-349">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="a6a88-349">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="a6a88-350">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-350">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="a6a88-351">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-351">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="a6a88-352">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-352">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="a6a88-353">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-353">Botservice</span></span>
* <span data-ttu-id="a6a88-354">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-354">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="a6a88-355">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-355">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="a6a88-356">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-356">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="a6a88-357">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="a6a88-357">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="a6a88-358">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-358">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="a6a88-359">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="a6a88-359">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="a6a88-360">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-360">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="a6a88-361">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-361">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="a6a88-362">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="a6a88-362">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="a6a88-363">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="a6a88-363">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6a88-364">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6a88-364">Key Vault</span></span>
* <span data-ttu-id="a6a88-365">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-365">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-366">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-366">Monitor</span></span>
* <span data-ttu-id="a6a88-367">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-367">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-368">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-368">Network</span></span>
* <span data-ttu-id="a6a88-369">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="a6a88-369">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="a6a88-370">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-370">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="a6a88-371">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="a6a88-371">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="a6a88-372">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-372">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a6a88-373">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a6a88-373">Policy Insights</span></span>
* <span data-ttu-id="a6a88-374">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-374">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-375">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-375">RDBMS</span></span>
* <span data-ttu-id="a6a88-376">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="a6a88-376">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="a6a88-377">Redis</span><span class="sxs-lookup"><span data-stu-id="a6a88-377">Redis</span></span>
* <span data-ttu-id="a6a88-378">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="a6a88-378">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="a6a88-379">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="a6a88-379">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="a6a88-380">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="a6a88-380">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="a6a88-381">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="a6a88-381">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="a6a88-382">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-382">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="a6a88-383">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="a6a88-383">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="a6a88-384">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-384">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-385">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-385">Role</span></span>
* <span data-ttu-id="a6a88-386">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-386">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="a6a88-387">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-387">SQL VM</span></span>
* <span data-ttu-id="a6a88-388">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-388">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-389">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-389">VM</span></span>
* <span data-ttu-id="a6a88-390">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-390">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="a6a88-391">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-391">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="a6a88-392">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="a6a88-392">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="a6a88-393">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-393">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="a6a88-394">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-394">January 31, 2019</span></span>

<span data-ttu-id="a6a88-395">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="a6a88-395">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-396">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-396">Core</span></span>

* <span data-ttu-id="a6a88-397">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="a6a88-397">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="a6a88-398">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-398">January 28, 2019</span></span>

<span data-ttu-id="a6a88-399">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="a6a88-399">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-400">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-400">ACR</span></span>
* <span data-ttu-id="a6a88-401">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-401">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-402">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-402">ACS</span></span>
* <span data-ttu-id="a6a88-403">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-403">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a6a88-404">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="a6a88-404">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="a6a88-405">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-405">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-406">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-406">AMS</span></span>
* <span data-ttu-id="a6a88-407">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-407">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="a6a88-408">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-408">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-409">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-409">Appservice</span></span>
* <span data-ttu-id="a6a88-410">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-410">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="a6a88-411">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-411">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="a6a88-412">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="a6a88-412">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-413">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-413">Container</span></span>
* <span data-ttu-id="a6a88-414">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-414">Added `container start` command</span></span>
* <span data-ttu-id="a6a88-415">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-415">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6a88-416">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="a6a88-416">EventGrid</span></span>
* <span data-ttu-id="a6a88-417">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-417">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="a6a88-418">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-418">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="a6a88-419">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="a6a88-419">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="a6a88-420">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="a6a88-420">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="a6a88-421">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a6a88-421">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6a88-422">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6a88-422">HDInsight</span></span>
* <span data-ttu-id="a6a88-423">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-423">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="a6a88-424">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-424">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="a6a88-425">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-425">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="a6a88-426">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="a6a88-426">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="a6a88-427">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-427">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="a6a88-428">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-428">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-429">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-429">IoT</span></span>
* <span data-ttu-id="a6a88-430">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="a6a88-430">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="a6a88-431">Kusto</span><span class="sxs-lookup"><span data-stu-id="a6a88-431">Kusto</span></span>
* <span data-ttu-id="a6a88-432">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a6a88-432">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-433">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-433">Monitor</span></span>
* <span data-ttu-id="a6a88-434">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a6a88-434">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-435">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-435">Profile</span></span>
* <span data-ttu-id="a6a88-436">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-436">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-437">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-437">Network</span></span>
* <span data-ttu-id="a6a88-438">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-438">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="a6a88-439">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="a6a88-439">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-440">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-440">Resource</span></span>
* <span data-ttu-id="a6a88-441">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-441">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="a6a88-442">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-442">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="a6a88-443">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-443">SQL Virtual Machine</span></span>
* <span data-ttu-id="a6a88-444">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a6a88-444">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-445">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-445">Storage</span></span>
* <span data-ttu-id="a6a88-446">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="a6a88-446">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="a6a88-447">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="a6a88-447">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-448">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-448">VM</span></span>
* <span data-ttu-id="a6a88-449">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-449">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="a6a88-450">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-450">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="a6a88-451">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-451">January 15, 2019</span></span>

<span data-ttu-id="a6a88-452">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="a6a88-452">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-453">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-453">ACR</span></span>
* <span data-ttu-id="a6a88-454">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="a6a88-454">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="a6a88-455">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="a6a88-455">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="a6a88-456">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="a6a88-456">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="a6a88-457">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-457">ACS</span></span>
* <span data-ttu-id="a6a88-458">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-458">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-459">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-459">Appservice</span></span>
* <span data-ttu-id="a6a88-460">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-460">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="a6a88-461">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="a6a88-461">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="a6a88-462">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="a6a88-462">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="a6a88-463">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-463">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="a6a88-464">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-464">Botservice</span></span>
* <span data-ttu-id="a6a88-465">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-465">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="a6a88-466">Настройка</span><span class="sxs-lookup"><span data-stu-id="a6a88-466">Configure</span></span>
* <span data-ttu-id="a6a88-467">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-467">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-468">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-468">CosmosDB</span></span>
* <span data-ttu-id="a6a88-469">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="a6a88-469">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6a88-470">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6a88-470">HDInsight</span></span>
* <span data-ttu-id="a6a88-471">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="a6a88-471">Added commands for managing applications</span></span>
* <span data-ttu-id="a6a88-472">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-472">Added commands for managing script actions</span></span>
* <span data-ttu-id="a6a88-473">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="a6a88-473">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="a6a88-474">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-474">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="a6a88-475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-475">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-476">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-476">Network</span></span>
* <span data-ttu-id="a6a88-477">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-477">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="a6a88-478">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="a6a88-478">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="a6a88-479">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-479">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="a6a88-480">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-480">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-481">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-481">Role</span></span>
* <span data-ttu-id="a6a88-482">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-482">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="a6a88-483">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-483">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="a6a88-484">Безопасность</span><span class="sxs-lookup"><span data-stu-id="a6a88-484">Security</span></span>
* <span data-ttu-id="a6a88-485">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-485">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-486">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-486">Storage</span></span>
* <span data-ttu-id="a6a88-487">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="a6a88-487">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="a6a88-488">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-488">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="a6a88-489">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-489">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="a6a88-490">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-490">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="a6a88-491">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-491">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-492">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-492">VM</span></span>
* <span data-ttu-id="a6a88-493">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-493">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="a6a88-494">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-494">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6a88-495">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-495">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="a6a88-496">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-496">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="a6a88-497">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-497">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="a6a88-498">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-498">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="a6a88-499">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-499">December 20, 2018</span></span>

<span data-ttu-id="a6a88-500">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="a6a88-500">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="a6a88-501">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-501">Appservice</span></span>
* <span data-ttu-id="a6a88-502">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="a6a88-502">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="a6a88-503">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-503">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="a6a88-504">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-504">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a6a88-505">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6a88-505">IoTCentral</span></span>
* <span data-ttu-id="a6a88-506">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-506">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-507">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-507">Role</span></span>
* <span data-ttu-id="a6a88-508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-508">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-509">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-509">SQL</span></span>
* <span data-ttu-id="a6a88-510">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-510">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-511">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-511">VM</span></span>
* <span data-ttu-id="a6a88-512">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-512">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="a6a88-513">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-513">December 18, 2018</span></span>

<span data-ttu-id="a6a88-514">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="a6a88-514">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="a6a88-515">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-515">ACR</span></span>
* <span data-ttu-id="a6a88-516">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-516">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="a6a88-517">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="a6a88-517">Condensed the table layout for task list</span></span>
* <span data-ttu-id="a6a88-518">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="a6a88-518">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-519">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-519">ACS</span></span>
* <span data-ttu-id="a6a88-520">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-520">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a6a88-521">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="a6a88-521">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="a6a88-522">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a6a88-522">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="a6a88-523">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-523">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="a6a88-524">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-524">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="a6a88-525">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-525">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-526">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-526">Appservice</span></span>
* <span data-ttu-id="a6a88-527">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-527">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="a6a88-528">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-528">Botservice</span></span>
* <span data-ttu-id="a6a88-529">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-529">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="a6a88-530">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="a6a88-530">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="a6a88-531">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="a6a88-531">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="a6a88-532">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="a6a88-532">Reduced Kudu network calls</span></span>
* <span data-ttu-id="a6a88-533">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-533">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-534">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-534">Consumption</span></span>
* <span data-ttu-id="a6a88-535">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-535">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-536">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-536">CosmosDB</span></span>
* <span data-ttu-id="a6a88-537">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="a6a88-537">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="a6a88-538">Карты</span><span class="sxs-lookup"><span data-stu-id="a6a88-538">Maps</span></span>
* <span data-ttu-id="a6a88-539">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="a6a88-539">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-540">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-540">Network</span></span>
* <span data-ttu-id="a6a88-541">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-541">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="a6a88-542">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="a6a88-542">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-543">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-543">Resource</span></span>
* <span data-ttu-id="a6a88-544">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-544">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="a6a88-545">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-545">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-546">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-546">Storage</span></span>
*  <span data-ttu-id="a6a88-547">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="a6a88-547">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-548">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-548">VM</span></span>
* <span data-ttu-id="a6a88-549">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-549">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="a6a88-550">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-550">December 4, 2018</span></span>

<span data-ttu-id="a6a88-551">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="a6a88-551">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="a6a88-552">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-552">Core</span></span>
* <span data-ttu-id="a6a88-553">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-553">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="a6a88-554">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="a6a88-554">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-555">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-555">Appservice</span></span>
* <span data-ttu-id="a6a88-556">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-556">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="a6a88-557">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="a6a88-557">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-558">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-558">Network</span></span>
* <span data-ttu-id="a6a88-559">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="a6a88-559">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-560">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-560">Role</span></span>
* <span data-ttu-id="a6a88-561">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-561">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="a6a88-562">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-562">VM</span></span>
* <span data-ttu-id="a6a88-563">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-563">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="a6a88-564">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="a6a88-564">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="a6a88-565">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="a6a88-565">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="a6a88-566">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-566">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="a6a88-567">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-567">November 20, 2018</span></span>

<span data-ttu-id="a6a88-568">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="a6a88-568">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="a6a88-569">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-569">Core</span></span>
* <span data-ttu-id="a6a88-570">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="a6a88-570">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-571">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-571">ACR</span></span>
* <span data-ttu-id="a6a88-572">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="a6a88-572">Added context token to task step</span></span>
* <span data-ttu-id="a6a88-573">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-573">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="a6a88-574">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-574">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-575">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-575">Appservice</span></span>
* <span data-ttu-id="a6a88-576">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-576">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="a6a88-577">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-577">Updated the default `node_version`.</span></span> <span data-ttu-id="a6a88-578">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-578">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="a6a88-579">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="a6a88-579">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="a6a88-580">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="a6a88-580">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a6a88-581">IotCentral</span><span class="sxs-lookup"><span data-stu-id="a6a88-581">IotCentral</span></span>
* <span data-ttu-id="a6a88-582">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="a6a88-582">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-583">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-583">KeyVault</span></span>
* <span data-ttu-id="a6a88-584">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="a6a88-584">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-585">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-585">Network</span></span>
* <span data-ttu-id="a6a88-586">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-586">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="a6a88-587">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-587">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="a6a88-588">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="a6a88-588">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="a6a88-589">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-589">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-590">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6a88-590">Rdbms</span></span>
* <span data-ttu-id="a6a88-591">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="a6a88-591">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="a6a88-592">RBAC:</span><span class="sxs-lookup"><span data-stu-id="a6a88-592">Rbac</span></span>
* <span data-ttu-id="a6a88-593">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-593">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="a6a88-594">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="a6a88-594">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="a6a88-595">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-595">Storage</span></span>
* <span data-ttu-id="a6a88-596">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="a6a88-596">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="a6a88-597">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-597">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="a6a88-598">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="a6a88-598">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="a6a88-599">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-599">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-600">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-600">VM</span></span>
* <span data-ttu-id="a6a88-601">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="a6a88-601">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="a6a88-602">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-602">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="a6a88-603">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-603">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="a6a88-604">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="a6a88-604">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="a6a88-605">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-605">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="a6a88-606">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-606">Added `snapshot wait` command</span></span>
* <span data-ttu-id="a6a88-607">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-607">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="a6a88-608">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-608">November 6, 2018</span></span>

<span data-ttu-id="a6a88-609">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="a6a88-609">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-610">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-610">Core</span></span>
* <span data-ttu-id="a6a88-611">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="a6a88-611">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-612">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-612">ACR</span></span>
* <span data-ttu-id="a6a88-613">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-613">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="a6a88-614">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="a6a88-614">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-615">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-615">ACS</span></span>
* <span data-ttu-id="a6a88-616">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-616">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="a6a88-617">Помощник</span><span class="sxs-lookup"><span data-stu-id="a6a88-617">Advisor</span></span>
* <span data-ttu-id="a6a88-618">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="a6a88-618">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-619">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-619">AMS</span></span>
* <span data-ttu-id="a6a88-620">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="a6a88-620">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="a6a88-621">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="a6a88-621">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="a6a88-622">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-622">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="a6a88-623">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-623">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="a6a88-624">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-624">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="a6a88-625">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-625">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="a6a88-626">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-626">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="a6a88-627">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-627">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="a6a88-628">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-628">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="a6a88-629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-629">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="a6a88-630">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-630">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="a6a88-631">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-631">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="a6a88-632">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="a6a88-632">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="a6a88-633">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="a6a88-633">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="a6a88-634">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-634">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="a6a88-635">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="a6a88-635">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="a6a88-636">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="a6a88-636">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-637">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-637">AppService</span></span>
* <span data-ttu-id="a6a88-638">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-638">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="a6a88-639">Настройка</span><span class="sxs-lookup"><span data-stu-id="a6a88-639">Configure</span></span>
* <span data-ttu-id="a6a88-640">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-640">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-641">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-641">Container</span></span>
* <span data-ttu-id="a6a88-642">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="a6a88-642">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="a6a88-643">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="a6a88-643">EventHub</span></span>
* <span data-ttu-id="a6a88-644">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-644">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-645">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-645">Interactive</span></span>
* <span data-ttu-id="a6a88-646">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="a6a88-646">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-647">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-647">Monitor</span></span>
* <span data-ttu-id="a6a88-648">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-648">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-649">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-649">Network</span></span>
* <span data-ttu-id="a6a88-650">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-650">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="a6a88-651">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a6a88-651">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="a6a88-652">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-652">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="a6a88-653">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-653">Profile</span></span>
* <span data-ttu-id="a6a88-654">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-654">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-655">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-655">RDBMS</span></span>
* <span data-ttu-id="a6a88-656">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-656">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-657">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-657">Resource</span></span>
* <span data-ttu-id="a6a88-658">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-658">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-659">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-659">Role</span></span>
* <span data-ttu-id="a6a88-660">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-660">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="a6a88-661">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-661">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="a6a88-662">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="a6a88-662">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-663">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-663">Storage</span></span>
* <span data-ttu-id="a6a88-664">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-664">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-665">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-665">VM</span></span>
* <span data-ttu-id="a6a88-666">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-666">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="a6a88-667">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="a6a88-667">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="a6a88-668">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="a6a88-668">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="a6a88-669">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="a6a88-669">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="a6a88-670">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-670">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="a6a88-671">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-671">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="a6a88-672">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-672">October 23, 2018</span></span>

<span data-ttu-id="a6a88-673">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="a6a88-673">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-674">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-674">Core</span></span>
* <span data-ttu-id="a6a88-675">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-675">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="a6a88-676">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-676">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-677">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-677">ACR</span></span>
* <span data-ttu-id="a6a88-678">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-678">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-679">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-679">CDN</span></span>
* <span data-ttu-id="a6a88-680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-680">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a6a88-681">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="a6a88-681">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-682">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-682">Container</span></span>
* <span data-ttu-id="a6a88-683">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="a6a88-683">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="a6a88-684">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-684">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="a6a88-685">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-685">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="a6a88-686">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-686">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="a6a88-687">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-687">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="a6a88-688">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-688">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="a6a88-689">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-689">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-690">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-690">CosmosDB</span></span>
* <span data-ttu-id="a6a88-691">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-691">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-692">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-692">Interactive</span></span>
* <span data-ttu-id="a6a88-693">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-693">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6a88-694">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6a88-694">IoT Central</span></span>
* <span data-ttu-id="a6a88-695">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="a6a88-695">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="a6a88-696">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="a6a88-696">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-697">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-697">Monitor</span></span>
* <span data-ttu-id="a6a88-698">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="a6a88-698">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="a6a88-699">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-699">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="a6a88-700">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-700">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a6a88-701">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-701">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="a6a88-702">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-702">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="a6a88-703">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="a6a88-703">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="a6a88-704">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="a6a88-704">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="a6a88-705">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-705">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a6a88-706">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-706">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="a6a88-707">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-707">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-708">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-708">Network</span></span>
* <span data-ttu-id="a6a88-709">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-709">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="a6a88-710">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-710">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="a6a88-711">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="a6a88-711">ServiceBus</span></span>
* <span data-ttu-id="a6a88-712">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="a6a88-712">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-713">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-713">SQL</span></span>
* <span data-ttu-id="a6a88-714">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="a6a88-714">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-715">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-715">Storage</span></span>
* <span data-ttu-id="a6a88-716">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-716">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="a6a88-717">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="a6a88-717">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-718">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-718">VM</span></span>
* <span data-ttu-id="a6a88-719">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-719">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6a88-720">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="a6a88-720">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="a6a88-721">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="a6a88-721">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="a6a88-722">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-722">October 16, 2018</span></span>

<span data-ttu-id="a6a88-723">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="a6a88-723">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-724">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-724">VM</span></span>
* <span data-ttu-id="a6a88-725">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-725">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="a6a88-726">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-726">October 9, 2018</span></span>

<span data-ttu-id="a6a88-727">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="a6a88-727">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-728">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-728">Core</span></span>
* <span data-ttu-id="a6a88-729">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="a6a88-729">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-730">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-730">ACR</span></span>
* <span data-ttu-id="a6a88-731">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="a6a88-731">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-732">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-732">ACS</span></span>
* <span data-ttu-id="a6a88-733">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="a6a88-733">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="a6a88-734">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="a6a88-734">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="a6a88-735">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-735">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="a6a88-736">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-736">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-737">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-737">Container</span></span>
* <span data-ttu-id="a6a88-738">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-738">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="a6a88-739">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-739">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="a6a88-740">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="a6a88-740">Event Hub</span></span>
* <span data-ttu-id="a6a88-741">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-741">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="a6a88-742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="a6a88-742">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="a6a88-743">расширения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-743">Extensions</span></span>
* <span data-ttu-id="a6a88-744">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="a6a88-744">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a6a88-745">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a6a88-745">HDInsight</span></span>
* <span data-ttu-id="a6a88-746">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-746">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-747">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-747">IoT</span></span>
* <span data-ttu-id="a6a88-748">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-748">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-749">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-749">KeyVault</span></span>
* <span data-ttu-id="a6a88-750">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="a6a88-750">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-751">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-751">Network</span></span>
* <span data-ttu-id="a6a88-752">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-752">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="a6a88-753">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="a6a88-753">See #6052</span></span>
* <span data-ttu-id="a6a88-754">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-754">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="a6a88-755">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a6a88-755">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="a6a88-756">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-756">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="a6a88-757">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-757">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="a6a88-758">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-758">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="a6a88-759">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-759">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-760">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-760">Role</span></span>
* <span data-ttu-id="a6a88-761">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-761">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="a6a88-762">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-762">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="a6a88-763">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-763">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="a6a88-764">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="a6a88-764">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6a88-765">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-765">Service Bus</span></span>
* <span data-ttu-id="a6a88-766">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="a6a88-766">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-767">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-767">VM</span></span>
* <span data-ttu-id="a6a88-768">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-768">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="a6a88-769">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-769">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="a6a88-770">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-770">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="a6a88-771">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-771">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="a6a88-772">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-772">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="a6a88-773">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="a6a88-773">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="a6a88-774">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-774">September 21, 2018</span></span>

<span data-ttu-id="a6a88-775">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="a6a88-775">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-776">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-776">ACR</span></span>
* <span data-ttu-id="a6a88-777">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-777">Added ACR Task commands</span></span>
* <span data-ttu-id="a6a88-778">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="a6a88-778">Added quick run command</span></span>
* <span data-ttu-id="a6a88-779">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-779">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="a6a88-780">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-780">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="a6a88-781">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-781">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="a6a88-782">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-782">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-783">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-783">ACS</span></span>
* <span data-ttu-id="a6a88-784">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-784">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="a6a88-785">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-785">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-786">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-786">AppService</span></span>

* <span data-ttu-id="a6a88-787">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="a6a88-787">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="a6a88-788">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="a6a88-788">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="a6a88-789">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-789">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="a6a88-790">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-790">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-791">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-791">Batch</span></span>
* <span data-ttu-id="a6a88-792">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="a6a88-792">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="a6a88-793">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-793">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="a6a88-794">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-794">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="a6a88-795">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="a6a88-795">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6a88-796">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-796">Batch AI</span></span> 
* <span data-ttu-id="a6a88-797">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-797">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6a88-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6a88-798">Cognitive Services</span></span>
* <span data-ttu-id="a6a88-799">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-799">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="a6a88-800">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-800">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="a6a88-801">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-801">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="a6a88-802">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-802">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="a6a88-803">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="a6a88-803">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="a6a88-804">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-804">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-805">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-805">Container</span></span>
* <span data-ttu-id="a6a88-806">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-806">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="a6a88-807">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="a6a88-807">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="a6a88-808">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-808">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="a6a88-809">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-809">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="a6a88-810">Data Lake</span><span class="sxs-lookup"><span data-stu-id="a6a88-810">Datalake</span></span>
* <span data-ttu-id="a6a88-811">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-811">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="a6a88-812">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="a6a88-812">Interactive Shell</span></span>
* <span data-ttu-id="a6a88-813">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-813">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="a6a88-814">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-814">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-815">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-815">IoT</span></span>
* <span data-ttu-id="a6a88-816">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-816">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6a88-817">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a6a88-817">Key Vault</span></span>
* <span data-ttu-id="a6a88-818">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="a6a88-818">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-819">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-819">Network</span></span>
* <span data-ttu-id="a6a88-820">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-820">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="a6a88-821">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-821">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="a6a88-822">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="a6a88-822">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="a6a88-823">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-823">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="a6a88-824">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-824">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="a6a88-825">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-825">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="a6a88-826">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-826">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="a6a88-827">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-827">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="a6a88-828">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-828">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="a6a88-829">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-829">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="a6a88-830">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-830">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="a6a88-831">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-831">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="a6a88-832">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-832">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="a6a88-833">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="a6a88-833">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="a6a88-834">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-834">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="a6a88-835">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-835">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="a6a88-836">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="a6a88-836">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="a6a88-837">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a6a88-837">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-838">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-838">RDBMS</span></span>
* <span data-ttu-id="a6a88-839">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="a6a88-839">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="a6a88-840">резервирование.</span><span class="sxs-lookup"><span data-stu-id="a6a88-840">Reservation</span></span>
* <span data-ttu-id="a6a88-841">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-841">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="a6a88-842">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="a6a88-842">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="a6a88-843">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="a6a88-843">Manage App</span></span>
* <span data-ttu-id="a6a88-844">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="a6a88-844">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="a6a88-845">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="a6a88-845">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-846">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-846">Role</span></span>
* <span data-ttu-id="a6a88-847">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-847">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="a6a88-848">SignalR</span><span class="sxs-lookup"><span data-stu-id="a6a88-848">SignalR</span></span>
* <span data-ttu-id="a6a88-849">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-849">First release</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-850">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-850">Storage</span></span>
* <span data-ttu-id="a6a88-851">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="a6a88-851">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="a6a88-852">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="a6a88-852">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-853">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-853">VM</span></span>
* <span data-ttu-id="a6a88-854">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="a6a88-854">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="a6a88-855">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-855">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="a6a88-856">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-856">August 28, 2018</span></span>

<span data-ttu-id="a6a88-857">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a6a88-857">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-858">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-858">Core</span></span>

* <span data-ttu-id="a6a88-859">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-859">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a6a88-860">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6a88-860">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-861">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-861">ACR</span></span>

* <span data-ttu-id="a6a88-862">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="a6a88-862">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a6a88-863">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-863">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-864">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-864">ACS</span></span>

* <span data-ttu-id="a6a88-865">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-865">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a6a88-866">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-866">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-867">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-867">AppService</span></span>

* <span data-ttu-id="a6a88-868">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="a6a88-868">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a6a88-869">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-869">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a6a88-870">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-870">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a6a88-871">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a6a88-871">Backup</span></span>

* <span data-ttu-id="a6a88-872">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-872">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a6a88-873">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="a6a88-873">Bot Service</span></span>

* <span data-ttu-id="a6a88-874">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="a6a88-874">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6a88-875">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6a88-875">Cognitive Services</span></span>

* <span data-ttu-id="a6a88-876">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="a6a88-876">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-877">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-877">IoT</span></span>

* <span data-ttu-id="a6a88-878">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-878">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-879">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-879">Monitor</span></span>

* <span data-ttu-id="a6a88-880">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-880">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a6a88-881">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-881">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-882">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-882">Network</span></span>

* <span data-ttu-id="a6a88-883">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-883">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-884">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-884">Resource</span></span>

* <span data-ttu-id="a6a88-885">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-885">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-886">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-886">Storage</span></span>

* <span data-ttu-id="a6a88-887">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-887">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-888">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-888">VM</span></span>

* <span data-ttu-id="a6a88-889">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a6a88-889">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a6a88-890">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-890">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="a6a88-891">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-891">Auguest 14, 2018</span></span>

<span data-ttu-id="a6a88-892">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a6a88-892">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-893">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-893">Core</span></span>

* <span data-ttu-id="a6a88-894">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-894">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a6a88-895">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="a6a88-895">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a6a88-896">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="a6a88-896">Telemetry</span></span>

* <span data-ttu-id="a6a88-897">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-897">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-898">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-898">ACR</span></span>

* <span data-ttu-id="a6a88-899">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-899">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a6a88-900">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-900">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-901">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-901">ACS</span></span>

* <span data-ttu-id="a6a88-902">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-902">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a6a88-903">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-903">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a6a88-904">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="a6a88-904">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a6a88-905">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="a6a88-905">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a6a88-906">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-906">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a6a88-907">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-907">AppService</span></span>

* <span data-ttu-id="a6a88-908">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-908">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a6a88-909">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="a6a88-909">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a6a88-910">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6a88-910">BatchAI</span></span>

* <span data-ttu-id="a6a88-911">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="a6a88-911">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a6a88-912">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-912">Container</span></span>

* <span data-ttu-id="a6a88-913">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="a6a88-913">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a6a88-914">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-914">IoT</span></span>

* <span data-ttu-id="a6a88-915">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-915">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a6a88-916">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-916">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a6a88-917">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6a88-917">Iot Central</span></span>

* <span data-ttu-id="a6a88-918">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="a6a88-918">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-919">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-919">KeyVault</span></span>


* <span data-ttu-id="a6a88-920">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-920">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a6a88-921">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-921">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a6a88-922">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="a6a88-922">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a6a88-923">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-923">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a6a88-924">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-924">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a6a88-925">Передача</span><span class="sxs-lookup"><span data-stu-id="a6a88-925">Relay</span></span>

* <span data-ttu-id="a6a88-926">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-926">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-927">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-927">Sql</span></span>

* <span data-ttu-id="a6a88-928">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-928">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-929">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-929">Storage</span></span>

* <span data-ttu-id="a6a88-930">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="a6a88-930">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a6a88-931">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="a6a88-931">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a6a88-932">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-932">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a6a88-933">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-933">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a6a88-934">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-934">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-935">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-935">VM</span></span>

* <span data-ttu-id="a6a88-936">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-936">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a6a88-937">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-937">July 31, 2018</span></span>

<span data-ttu-id="a6a88-938">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a6a88-938">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-939">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-939">ACR</span></span>

* <span data-ttu-id="a6a88-940">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-940">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a6a88-941">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-941">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-942">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-942">ACS</span></span>

* <span data-ttu-id="a6a88-943">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="a6a88-943">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-944">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-944">Batch</span></span>

* <span data-ttu-id="a6a88-945">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="a6a88-945">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-946">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-946">Container</span></span>

* <span data-ttu-id="a6a88-947">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-947">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-948">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-948">Network</span></span>

* <span data-ttu-id="a6a88-949">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-949">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a6a88-950">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-950">Resource</span></span>

* <span data-ttu-id="a6a88-951">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-951">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a6a88-952">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="a6a88-952">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-953">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-953">Role</span></span>

* <span data-ttu-id="a6a88-954">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6a88-954">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a6a88-955">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="a6a88-955">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a6a88-956">поиска</span><span class="sxs-lookup"><span data-stu-id="a6a88-956">Search</span></span>

* <span data-ttu-id="a6a88-957">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="a6a88-957">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6a88-958">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-958">Service Bus</span></span>

* <span data-ttu-id="a6a88-959">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="a6a88-959">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a6a88-960">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="a6a88-960">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="a6a88-961">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="a6a88-961">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="a6a88-962">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-962">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-963">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-963">Storage</span></span>

* <span data-ttu-id="a6a88-964">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-964">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a6a88-965">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="a6a88-965">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-966">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-966">VM</span></span>

* <span data-ttu-id="a6a88-967">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="a6a88-967">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a6a88-968">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-968">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="a6a88-969">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a6a88-969">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a6a88-970">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="a6a88-970">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a6a88-971">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-971">July 18, 2018</span></span>

<span data-ttu-id="a6a88-972">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a6a88-972">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-973">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-973">Core</span></span>

* <span data-ttu-id="a6a88-974">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-974">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a6a88-975">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-975">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a6a88-976">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-976">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-977">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-977">ACR</span></span>

* <span data-ttu-id="a6a88-978">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-978">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a6a88-979">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-979">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a6a88-980">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-980">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a6a88-981">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-981">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-982">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-982">ACS</span></span>

* <span data-ttu-id="a6a88-983">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="a6a88-983">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-984">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-984">AppService</span></span>

* <span data-ttu-id="a6a88-985">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-985">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-986">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-986">Batch</span></span>

* <span data-ttu-id="a6a88-987">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a6a88-987">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a6a88-988">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-988">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6a88-989">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-989">Batch AI</span></span>

* <span data-ttu-id="a6a88-990">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-990">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-991">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-991">Container</span></span>

* <span data-ttu-id="a6a88-992">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="a6a88-992">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a6a88-993">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="a6a88-993">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-994">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-994">Network</span></span>

* <span data-ttu-id="a6a88-995">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-995">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="a6a88-996">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-996">Added `network nic wait`</span></span>
* <span data-ttu-id="a6a88-997">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="a6a88-997">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="a6a88-998">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="a6a88-998">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="a6a88-999">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-999">Resource</span></span>

* <span data-ttu-id="a6a88-1000">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1000">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="a6a88-1001">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1001">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="a6a88-1002">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1002">Added `deployment wait` command</span></span>
* <span data-ttu-id="a6a88-1003">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1003">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1004">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1004">SQL</span></span>

* <span data-ttu-id="a6a88-1005">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1005">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a6a88-1006">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1006">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="a6a88-1007">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1007">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1008">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1008">Storage</span></span>

* <span data-ttu-id="a6a88-1009">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1009">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1010">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1010">VM</span></span>

* <span data-ttu-id="a6a88-1011">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1011">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a6a88-1012">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1012">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="a6a88-1013">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1013">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a6a88-1014">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1014">July 3, 2018</span></span>

<span data-ttu-id="a6a88-1015">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a6a88-1015">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a6a88-1016">AKS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1016">AKS</span></span>

* <span data-ttu-id="a6a88-1017">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1017">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a6a88-1018">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1018">July 3, 2018</span></span>

<span data-ttu-id="a6a88-1019">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a6a88-1019">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1020">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1020">Core</span></span>

* <span data-ttu-id="a6a88-1021">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1021">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1022">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1022">ACR</span></span>

* <span data-ttu-id="a6a88-1023">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1023">Added polling build status</span></span>
* <span data-ttu-id="a6a88-1024">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1024">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a6a88-1025">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1025">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1026">ACS</span></span>

* <span data-ttu-id="a6a88-1027">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1027">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a6a88-1028">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1028">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a6a88-1029">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1029">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a6a88-1030">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1030">Added `--listen-port` support</span></span>
* <span data-ttu-id="a6a88-1031">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1031">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a6a88-1032">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1032">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a6a88-1033">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1033">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1034">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-1034">AppService</span></span>

* <span data-ttu-id="a6a88-1035">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1035">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="a6a88-1036">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1036">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a6a88-1037">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a6a88-1037">Backup</span></span>

* <span data-ttu-id="a6a88-1038">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1038">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a6a88-1039">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6a88-1039">BatchAI</span></span>

* <span data-ttu-id="a6a88-1040">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1040">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a6a88-1041">Облако</span><span class="sxs-lookup"><span data-stu-id="a6a88-1041">Cloud</span></span>

* <span data-ttu-id="a6a88-1042">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1042">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1043">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1043">Container</span></span>

* <span data-ttu-id="a6a88-1044">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1044">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a6a88-1045">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1045">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="a6a88-1046">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1046">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1047">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1047">Extension</span></span>

* <span data-ttu-id="a6a88-1048">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1048">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1049">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1049">Network</span></span>

* <span data-ttu-id="a6a88-1050">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1050">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-1051">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a6a88-1051">Rdbms</span></span>

* <span data-ttu-id="a6a88-1052">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1052">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1053">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1053">Resource</span></span>

* <span data-ttu-id="a6a88-1054">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1054">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1055">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1055">VM</span></span>

* <span data-ttu-id="a6a88-1056">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1056">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a6a88-1057">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1057">June 25, 2018</span></span>

<span data-ttu-id="a6a88-1058">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a6a88-1058">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a6a88-1059">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="a6a88-1059">CLI</span></span>

* <span data-ttu-id="a6a88-1060">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1060">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a6a88-1061">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1061">June 19, 2018</span></span>

<span data-ttu-id="a6a88-1062">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a6a88-1062">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1063">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1063">Core</span></span>

* <span data-ttu-id="a6a88-1064">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1064">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1065">ACR</span></span>

* <span data-ttu-id="a6a88-1066">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1066">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a6a88-1067">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1067">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1068">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1068">ACS</span></span>

* <span data-ttu-id="a6a88-1069">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1069">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a6a88-1070">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1070">Added `--update` support</span></span>
* <span data-ttu-id="a6a88-1071">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1071">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="a6a88-1072">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1072">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a6a88-1073">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1073">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a6a88-1074">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1074">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="a6a88-1075">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1075">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="a6a88-1076">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1076">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1077">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-1077">AppService</span></span>

* <span data-ttu-id="a6a88-1078">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1078">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a6a88-1079">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1079">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-1080">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1080">Batch</span></span>

* <span data-ttu-id="a6a88-1081">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1081">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6a88-1082">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-1082">Batch AI</span></span>

* <span data-ttu-id="a6a88-1083">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1083">Added support for workspaces.</span></span> <span data-ttu-id="a6a88-1084">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1084">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a6a88-1085">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1085">Added support for experiments.</span></span> <span data-ttu-id="a6a88-1086">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1086">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a6a88-1087">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1087">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a6a88-1088">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1088">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a6a88-1089">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1089">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a6a88-1090">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1090">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a6a88-1091">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1091">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a6a88-1092">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1092">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a6a88-1093">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1093">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a6a88-1094">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1094">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a6a88-1095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1095">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a6a88-1096">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1096">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a6a88-1097">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1097">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a6a88-1098">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1098">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a6a88-1099">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1099">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a6a88-1100">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1100">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="a6a88-1101">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="a6a88-1101">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="a6a88-1102">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="a6a88-1102">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a6a88-1103">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="a6a88-1103">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a6a88-1104">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="a6a88-1104">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a6a88-1105">Карты</span><span class="sxs-lookup"><span data-stu-id="a6a88-1105">Maps</span></span>

* <span data-ttu-id="a6a88-1106">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1106">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1107">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1107">Network</span></span>

* <span data-ttu-id="a6a88-1108">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1108">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a6a88-1109">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1109">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a6a88-1110">#6502</span><span class="sxs-lookup"><span data-stu-id="a6a88-1110">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a6a88-1111">Резервирование</span><span class="sxs-lookup"><span data-stu-id="a6a88-1111">Reservations</span></span>

* <span data-ttu-id="a6a88-1112">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1112">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="a6a88-1113">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1113">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="a6a88-1114">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1114">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="a6a88-1115">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1115">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="a6a88-1116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1116">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="a6a88-1117">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1117">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1118">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1118">Role</span></span>

* <span data-ttu-id="a6a88-1119">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1119">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1120">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1120">SQL</span></span>

* <span data-ttu-id="a6a88-1121">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1121">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1122">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1122">Storage</span></span>

* <span data-ttu-id="a6a88-1123">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1123">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1124">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1124">VM</span></span>

* <span data-ttu-id="a6a88-1125">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1125">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="a6a88-1126">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1126">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="a6a88-1127">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1127">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a6a88-1128">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1128">June 13, 2018</span></span>

<span data-ttu-id="a6a88-1129">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a6a88-1129">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1130">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1130">Core</span></span>

* <span data-ttu-id="a6a88-1131">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1131">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a6a88-1132">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1132">June 13, 2018</span></span>

<span data-ttu-id="a6a88-1133">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a6a88-1133">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a6a88-1134">AKS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1134">AKS</span></span>

* <span data-ttu-id="a6a88-1135">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1135">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a6a88-1136">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1136">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a6a88-1137">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1137">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a6a88-1138">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1138">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a6a88-1139">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1139">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-1140">AppService</span></span>

* <span data-ttu-id="a6a88-1141">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1141">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a6a88-1142">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1142">June 5, 2018</span></span>

<span data-ttu-id="a6a88-1143">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a6a88-1143">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1144">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1144">Interactive</span></span>

* <span data-ttu-id="a6a88-1145">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1145">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a6a88-1146">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1146">June 5, 2018</span></span>

<span data-ttu-id="a6a88-1147">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a6a88-1147">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1148">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1148">Core</span></span>

* <span data-ttu-id="a6a88-1149">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1149">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a6a88-1150">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1150">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1151">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1151">ACR</span></span>

* <span data-ttu-id="a6a88-1152">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1152">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a6a88-1153">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1153">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a6a88-1154">AKS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1154">AKS</span></span>

* <span data-ttu-id="a6a88-1155">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1155">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-1156">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1156">Batch</span></span>

* <span data-ttu-id="a6a88-1157">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a6a88-1157">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-1158">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1158">IOT</span></span>

* <span data-ttu-id="a6a88-1159">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1159">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1160">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1160">Network</span></span>

* <span data-ttu-id="a6a88-1161">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1161">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a6a88-1162">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a6a88-1162">Policy Insights</span></span>

* <span data-ttu-id="a6a88-1163">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-1163">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a6a88-1164">ARM</span><span class="sxs-lookup"><span data-stu-id="a6a88-1164">ARM</span></span>

* <span data-ttu-id="a6a88-1165">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1165">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1166">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1166">SQL</span></span>

* <span data-ttu-id="a6a88-1167">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1167">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a6a88-1168">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1168">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a6a88-1169">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1169">Storage</span></span>

* <span data-ttu-id="a6a88-1170">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1170">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1171">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1171">VM</span></span>

* <span data-ttu-id="a6a88-1172">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1172">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a6a88-1173">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1173">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a6a88-1174">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1174">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a6a88-1175">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1175">May 22, 2018</span></span>

<span data-ttu-id="a6a88-1176">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a6a88-1176">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1177">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1177">Core</span></span>

* <span data-ttu-id="a6a88-1178">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1178">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1179">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1179">ACS</span></span>

* <span data-ttu-id="a6a88-1180">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1180">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a6a88-1181">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1181">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1182">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-1182">AppService</span></span>

* <span data-ttu-id="a6a88-1183">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1183">Improved generic update commands</span></span>
* <span data-ttu-id="a6a88-1184">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1184">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1185">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1185">Container</span></span>

* <span data-ttu-id="a6a88-1186">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1186">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a6a88-1187">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1187">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1188">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1188">Extension</span></span>

* <span data-ttu-id="a6a88-1189">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1189">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1190">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1190">Interactive</span></span>

* <span data-ttu-id="a6a88-1191">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1191">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a6a88-1192">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1192">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-1193">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1193">KeyVault</span></span>

* <span data-ttu-id="a6a88-1194">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1194">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1195">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1195">Network</span></span>

* <span data-ttu-id="a6a88-1196">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a6a88-1196">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a6a88-1197">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a6a88-1197">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1198">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1198">SQL</span></span>

* <span data-ttu-id="a6a88-1199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1199">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a6a88-1200">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1200">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a6a88-1201">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1201">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a6a88-1202">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1202">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a6a88-1203">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1203">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a6a88-1204">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1204">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a6a88-1205">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1205">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a6a88-1206">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1206">`edition`.</span></span> <span data-ttu-id="a6a88-1207">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1207">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a6a88-1208">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1208">`elasticPoolName`.</span></span> <span data-ttu-id="a6a88-1209">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1209">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a6a88-1210">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1210">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a6a88-1211">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1211">`edition`.</span></span> <span data-ttu-id="a6a88-1212">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1212">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a6a88-1213">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1213">`dtu`.</span></span> <span data-ttu-id="a6a88-1214">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1214">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a6a88-1215">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1215">`databaseDtuMin`.</span></span> <span data-ttu-id="a6a88-1216">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1216">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a6a88-1217">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1217">`databaseDtuMax`.</span></span> <span data-ttu-id="a6a88-1218">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1218">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a6a88-1219">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1219">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a6a88-1220">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1220">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1221">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1221">Storage</span></span>

* <span data-ttu-id="a6a88-1222">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1222">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a6a88-1223">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1223">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1224">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1224">VM</span></span>

* <span data-ttu-id="a6a88-1225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1225">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a6a88-1226">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1226">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a6a88-1227">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1227">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a6a88-1228">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1228">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a6a88-1229">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1229">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a6a88-1230">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1230">May 7, 2018</span></span>

<span data-ttu-id="a6a88-1231">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a6a88-1231">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1232">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1232">Core</span></span>

* <span data-ttu-id="a6a88-1233">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1233">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a6a88-1234">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1234">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a6a88-1235">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1235">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a6a88-1236">#5591</span><span class="sxs-lookup"><span data-stu-id="a6a88-1236">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a6a88-1237">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1237">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a6a88-1238">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1238">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a6a88-1239">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1239">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a6a88-1240">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1240">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a6a88-1241">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1241">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1242">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1242">ACR</span></span>

* <span data-ttu-id="a6a88-1243">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1243">Added ACR Build commands</span></span>
* <span data-ttu-id="a6a88-1244">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1244">Improved resource not found error messages</span></span>
* <span data-ttu-id="a6a88-1245">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1245">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a6a88-1246">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1246">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a6a88-1247">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1247">Improved repository commands error messages</span></span>
* <span data-ttu-id="a6a88-1248">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1248">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1249">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1249">ACS</span></span>

* <span data-ttu-id="a6a88-1250">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1250">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a6a88-1251">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1251">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a6a88-1252">AMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1252">AMS</span></span>

* <span data-ttu-id="a6a88-1253">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1253">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1254">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1254">Appservice</span></span>

* <span data-ttu-id="a6a88-1255">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1255">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a6a88-1256">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1256">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a6a88-1257">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1257">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a6a88-1258">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1258">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a6a88-1259">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-1259">Batch AI</span></span>

* <span data-ttu-id="a6a88-1260">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1260">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6a88-1261">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6a88-1261">Cognitive Services</span></span>

* <span data-ttu-id="a6a88-1262">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1262">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-1263">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-1263">Consumption</span></span>

* <span data-ttu-id="a6a88-1264">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1264">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1265">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1265">Container</span></span>

* <span data-ttu-id="a6a88-1266">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1266">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a6a88-1267">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="a6a88-1267">Cosmos DB</span></span>

* <span data-ttu-id="a6a88-1268">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-1268">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a6a88-1269">DMS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1269">DMS</span></span>

* <span data-ttu-id="a6a88-1270">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1270">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1271">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1271">Extension</span></span>

* <span data-ttu-id="a6a88-1272">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1272">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1273">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1273">Interactive</span></span>

* <span data-ttu-id="a6a88-1274">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1274">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a6a88-1275">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1275">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a6a88-1276">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1276">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a6a88-1277">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1277">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a6a88-1278">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a6a88-1278">Lab</span></span>

* <span data-ttu-id="a6a88-1279">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1279">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1280">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1280">Network</span></span>

* <span data-ttu-id="a6a88-1281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1281">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a6a88-1282">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1282">Profile</span></span>

* <span data-ttu-id="a6a88-1283">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1283">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a6a88-1284">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1284">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a6a88-1285">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1285">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a6a88-1286">Redis</span><span class="sxs-lookup"><span data-stu-id="a6a88-1286">Redis</span></span>

* <span data-ttu-id="a6a88-1287">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1287">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a6a88-1288">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1288">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a6a88-1289">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1289">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a6a88-1290">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1290">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a6a88-1291">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1291">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1292">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1292">Role</span></span>

* <span data-ttu-id="a6a88-1293">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1293">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1294">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1294">Storage</span></span>

* <span data-ttu-id="a6a88-1295">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1295">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a6a88-1296">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1296">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a6a88-1297">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1297">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a6a88-1298">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1298">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a6a88-1299">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1299">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1300">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1300">VM</span></span>

* <span data-ttu-id="a6a88-1301">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1301">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a6a88-1302">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1302">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a6a88-1303">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1303">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a6a88-1304">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1304">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a6a88-1305">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1305">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a6a88-1306">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1306">Added write accelerator support</span></span>
* <span data-ttu-id="a6a88-1307">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1307">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a6a88-1308">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1308">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a6a88-1309">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1309">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a6a88-1310">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1310">April 10, 2018</span></span>

<span data-ttu-id="a6a88-1311">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a6a88-1311">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1312">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1312">ACR</span></span>

* <span data-ttu-id="a6a88-1313">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1313">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1314">ACS</span></span>

* <span data-ttu-id="a6a88-1315">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1315">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1316">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1316">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a6a88-1318">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1318">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a6a88-1319">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a6a88-1319">BatchAI</span></span>

* <span data-ttu-id="a6a88-1320">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1320">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="a6a88-1321">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1321">Job level mounting</span></span>
  - <span data-ttu-id="a6a88-1322">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1322">Environment variables with secret values</span></span>
  - <span data-ttu-id="a6a88-1323">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="a6a88-1323">Performance counters settings</span></span>
  - <span data-ttu-id="a6a88-1324">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1324">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="a6a88-1325">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1325">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="a6a88-1326">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1326">Usage and limits reporting</span></span>
  - <span data-ttu-id="a6a88-1327">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1327">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="a6a88-1328">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1328">Support for custom images</span></span>
  - <span data-ttu-id="a6a88-1329">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1329">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a6a88-1330">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1330">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a6a88-1331">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1331">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a6a88-1332">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1332">National clouds are supported</span></span>
* <span data-ttu-id="a6a88-1333">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1333">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a6a88-1334">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1334">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a6a88-1335">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1335">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a6a88-1336">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1336">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a6a88-1337">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1337">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a6a88-1338">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1338">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a6a88-1339">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1339">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a6a88-1340">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1340">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a6a88-1341">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1341">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a6a88-1342">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1342">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a6a88-1343">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1343">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a6a88-1344">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1344">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a6a88-1345">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1345">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a6a88-1346">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="a6a88-1346">Billing</span></span>

* <span data-ttu-id="a6a88-1347">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1347">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-1348">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-1348">Consumption</span></span>

* <span data-ttu-id="a6a88-1349">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1349">Added `marketplace` commands</span></span>
* <span data-ttu-id="a6a88-1350">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1350">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a6a88-1351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1351">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a6a88-1352">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1352">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a6a88-1353">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1353">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a6a88-1354">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1354">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1355">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1355">Container</span></span>

* <span data-ttu-id="a6a88-1356">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1356">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a6a88-1357">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1357">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1358">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1358">Extension</span></span>

* <span data-ttu-id="a6a88-1359">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1359">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1360">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1360">Interactive</span></span>

* <span data-ttu-id="a6a88-1361">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1361">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a6a88-1362">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1362">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a6a88-1363">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1363">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1364">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1364">Network</span></span>

* <span data-ttu-id="a6a88-1365">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1365">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a6a88-1366">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1366">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="a6a88-1367">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1367">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="a6a88-1368">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1368">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a6a88-1369">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1369">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a6a88-1370">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1370">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a6a88-1371">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1371">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a6a88-1372">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1372">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1373">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1373">Profile</span></span>

* <span data-ttu-id="a6a88-1374">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1374">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a6a88-1375">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1375">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-1376">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-1376">RDBMS</span></span>

* <span data-ttu-id="a6a88-1377">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1377">Added `georestore` command</span></span>
* <span data-ttu-id="a6a88-1378">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1378">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1379">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1379">Resource</span></span>

* <span data-ttu-id="a6a88-1380">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1380">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a6a88-1381">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1381">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1382">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1382">SQL</span></span>

* <span data-ttu-id="a6a88-1383">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1383">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1384">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1384">Storage</span></span>

* <span data-ttu-id="a6a88-1385">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1385">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1386">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1386">VM</span></span>

* <span data-ttu-id="a6a88-1387">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1387">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a6a88-1388">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1388">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a6a88-1390">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1390">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a6a88-1391">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1391">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="a6a88-1392">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1392">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="a6a88-1393">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1393">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a6a88-1394">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1394">March 27, 2018</span></span>

<span data-ttu-id="a6a88-1395">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a6a88-1395">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1396">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1396">Core</span></span>

* <span data-ttu-id="a6a88-1397">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1397">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1398">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1398">ACS</span></span>

* <span data-ttu-id="a6a88-1399">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1399">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1400">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1400">Appservice</span></span>

* <span data-ttu-id="a6a88-1401">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1401">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a6a88-1402">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1402">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a6a88-1403">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a6a88-1403">Backup</span></span>

* <span data-ttu-id="a6a88-1404">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1404">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a6a88-1405">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1405">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a6a88-1406">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1406">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a6a88-1407">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1407">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1408">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1408">Container</span></span>

* <span data-ttu-id="a6a88-1409">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1409">Added `container exec` command.</span></span> <span data-ttu-id="a6a88-1410">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1410">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a6a88-1411">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1411">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1412">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1412">Extension</span></span>

* <span data-ttu-id="a6a88-1413">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1413">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a6a88-1414">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1414">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a6a88-1415">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1415">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1416">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1416">Interactive</span></span>

* <span data-ttu-id="a6a88-1417">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1417">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a6a88-1418">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1418">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a6a88-1419">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1419">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a6a88-1420">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1420">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a6a88-1421">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a6a88-1421">Lab</span></span>

* <span data-ttu-id="a6a88-1422">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1422">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1423">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1423">Monitor</span></span>

* <span data-ttu-id="a6a88-1424">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1424">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a6a88-1425">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1425">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a6a88-1426">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1426">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1427">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1427">Network</span></span>

* <span data-ttu-id="a6a88-1428">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1428">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1429">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1429">Profile</span></span>

* <span data-ttu-id="a6a88-1430">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1430">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-1431">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-1431">RDBMS</span></span>

* <span data-ttu-id="a6a88-1432">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1432">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1433">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1433">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a6a88-1435">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1435">Role</span></span>

* <span data-ttu-id="a6a88-1436">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1436">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a6a88-1437">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1437">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a6a88-1438">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1438">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a6a88-1439">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1439">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a6a88-1440">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1440">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1441">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1441">Storage</span></span>

* <span data-ttu-id="a6a88-1442">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1442">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a6a88-1443">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1443">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1444">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1444">VM</span></span>

* <span data-ttu-id="a6a88-1445">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1445">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a6a88-1446">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1446">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a6a88-1447">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1447">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a6a88-1448">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1448">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a6a88-1449">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1449">March 13, 2018</span></span>

<span data-ttu-id="a6a88-1450">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a6a88-1450">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1451">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1451">ACR</span></span>

* <span data-ttu-id="a6a88-1452">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1452">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a6a88-1453">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1453">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a6a88-1454">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1454">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1455">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1455">ACS</span></span>

* <span data-ttu-id="a6a88-1456">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1456">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a6a88-1457">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1457">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a6a88-1458">Помощник</span><span class="sxs-lookup"><span data-stu-id="a6a88-1458">Advisor</span></span>

* <span data-ttu-id="a6a88-1459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1459">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a6a88-1460">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1460">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a6a88-1461">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1461">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="a6a88-1462">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1462">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a6a88-1463">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1463">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1464">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1464">Appservice</span></span>

* <span data-ttu-id="a6a88-1465">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1465">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a6a88-1466">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1466">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a6a88-1467">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="a6a88-1467">Eventhubs</span></span>

* <span data-ttu-id="a6a88-1468">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-1468">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1469">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1469">Extension</span></span>

* <span data-ttu-id="a6a88-1470">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1470">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1471">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1471">Interactive</span></span>

* <span data-ttu-id="a6a88-1472">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1472">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a6a88-1473">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1473">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a6a88-1474">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1474">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a6a88-1475">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1475">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1476">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1476">Monitor</span></span>

* <span data-ttu-id="a6a88-1477">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1477">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a6a88-1478">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1478">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a6a88-1479">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1479">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a6a88-1480">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1480">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1481">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1481">Network</span></span>

* <span data-ttu-id="a6a88-1482">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1482">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a6a88-1483">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1483">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a6a88-1484">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1484">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a6a88-1485">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1485">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1486">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1486">Profile</span></span>

* <span data-ttu-id="a6a88-1487">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1487">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a6a88-1488">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1488">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-1489">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-1489">RDBMS</span></span>

* <span data-ttu-id="a6a88-1490">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1490">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a6a88-1491">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1491">Service Bus</span></span>

* <span data-ttu-id="a6a88-1492">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-1492">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1493">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1493">Storage</span></span>

* <span data-ttu-id="a6a88-1494">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1494">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a6a88-1495">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1495">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1496">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1496">VM</span></span>

* <span data-ttu-id="a6a88-1497">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1497">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a6a88-1498">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1498">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a6a88-1499">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1499">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a6a88-1500">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1500">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a6a88-1501">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="a6a88-1501">February 27, 2018</span></span>

<span data-ttu-id="a6a88-1502">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a6a88-1502">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1503">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1503">Core</span></span>

* <span data-ttu-id="a6a88-1504">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1504">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a6a88-1505">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1505">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a6a88-1506">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1506">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1507">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1507">ACS</span></span>

* <span data-ttu-id="a6a88-1508">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1508">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a6a88-1509">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1509">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a6a88-1510">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1510">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a6a88-1511">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1511">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1512">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1512">Appservice</span></span>

* <span data-ttu-id="a6a88-1513">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a6a88-1513">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a6a88-1514">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1514">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a6a88-1515">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a6a88-1515">Cognitive Services</span></span>

* <span data-ttu-id="a6a88-1516">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1516">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-1517">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-1517">Consumption</span></span>

* <span data-ttu-id="a6a88-1518">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1518">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a6a88-1519">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1519">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1520">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1520">Container</span></span>

* <span data-ttu-id="a6a88-1521">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1521">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1522">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1522">Network</span></span>

* <span data-ttu-id="a6a88-1523">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1523">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1524">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1524">Resource</span></span>

* <span data-ttu-id="a6a88-1525">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1525">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1526">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1526">Role</span></span>

* <span data-ttu-id="a6a88-1527">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1527">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1528">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1528">SQL</span></span>

* <span data-ttu-id="a6a88-1529">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1529">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1530">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1530">Storage</span></span>

* <span data-ttu-id="a6a88-1531">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1531">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1532">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1532">VM</span></span>

* <span data-ttu-id="a6a88-1533">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1533">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a6a88-1534">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1534">February 13, 2018</span></span>

<span data-ttu-id="a6a88-1535">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a6a88-1535">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1536">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1536">Core</span></span>

* <span data-ttu-id="a6a88-1537">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1537">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1538">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1538">ACS</span></span>

* <span data-ttu-id="a6a88-1539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1539">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a6a88-1540">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1540">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a6a88-1541">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1541">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a6a88-1542">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1542">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a6a88-1543">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1543">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a6a88-1544">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1544">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a6a88-1545">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1545">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a6a88-1546">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1546">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1547">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1547">Appservice</span></span>

* <span data-ttu-id="a6a88-1548">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1548">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a6a88-1549">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1549">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-1550">CDN</span></span>

* <span data-ttu-id="a6a88-1551">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1551">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1552">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1552">Container</span></span>

* <span data-ttu-id="a6a88-1553">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1553">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a6a88-1554">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1554">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-1555">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-1555">CosmosDB</span></span>

* <span data-ttu-id="a6a88-1556">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1556">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1557">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1557">Extension</span></span>

* <span data-ttu-id="a6a88-1558">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1558">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a6a88-1559">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1559">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a6a88-1560">Отзыв</span><span class="sxs-lookup"><span data-stu-id="a6a88-1560">Feedback</span></span>

* <span data-ttu-id="a6a88-1561">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1561">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1562">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1562">Interactive</span></span>

* <span data-ttu-id="a6a88-1563">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1563">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a6a88-1564">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1564">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-1565">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1565">IoT</span></span>

* <span data-ttu-id="a6a88-1566">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1566">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a6a88-1567">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1567">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a6a88-1568">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1568">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a6a88-1569">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1569">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1570">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1570">Monitor</span></span>

* <span data-ttu-id="a6a88-1571">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1571">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1572">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1572">Network</span></span>

* <span data-ttu-id="a6a88-1573">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1573">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a6a88-1574">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1574">Profile</span></span>

* <span data-ttu-id="a6a88-1575">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1575">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1576">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1576">Resource</span></span>

* <span data-ttu-id="a6a88-1577">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1577">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1578">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1578">Role</span></span>

* <span data-ttu-id="a6a88-1579">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1579">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1580">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1580">SQL</span></span>

* <span data-ttu-id="a6a88-1581">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1581">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a6a88-1582">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1582">Added `sql db rename`</span></span>
* <span data-ttu-id="a6a88-1583">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1583">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1584">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1584">Storage</span></span>

* <span data-ttu-id="a6a88-1585">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1585">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1586">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1586">VM</span></span>

* <span data-ttu-id="a6a88-1587">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1587">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a6a88-1588">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1588">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a6a88-1589">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1589">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a6a88-1590">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1590">January 31, 2018</span></span>

<span data-ttu-id="a6a88-1591">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a6a88-1591">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1592">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1592">Core</span></span>

* <span data-ttu-id="a6a88-1593">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1593">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a6a88-1594">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1594">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a6a88-1595">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1595">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a6a88-1596">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1596">Use `--verbose` to see</span></span>
* <span data-ttu-id="a6a88-1597">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1597">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1598">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1598">ACS</span></span>

* <span data-ttu-id="a6a88-1599">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1599">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a6a88-1600">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1600">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1601">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1601">Appservice</span></span>

* <span data-ttu-id="a6a88-1602">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1602">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a6a88-1603">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1603">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-1604">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-1604">CDN</span></span>

* <span data-ttu-id="a6a88-1605">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1605">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-1606">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-1606">CosmosDB</span></span>

* <span data-ttu-id="a6a88-1607">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1607">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1608">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1608">Interactive</span></span>

* <span data-ttu-id="a6a88-1609">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1609">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1610">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1610">Network</span></span>

* <span data-ttu-id="a6a88-1611">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1611">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a6a88-1612">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1612">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a6a88-1613">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1613">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a6a88-1614">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1614">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a6a88-1615">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1615">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a6a88-1616">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="a6a88-1616">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a6a88-1617">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1617">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a6a88-1618">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1618">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a6a88-1619">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1619">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="a6a88-1620">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1620">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1621">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1621">Profile</span></span>

* <span data-ttu-id="a6a88-1622">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1622">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1623">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1623">Resource</span></span>

* <span data-ttu-id="a6a88-1624">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1624">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1625">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1625">Storage</span></span>

* <span data-ttu-id="a6a88-1626">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1626">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a6a88-1627">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1627">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a6a88-1628">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1628">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="a6a88-1629">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1629">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a6a88-1630">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1630">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1631">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1631">VM</span></span>

* <span data-ttu-id="a6a88-1632">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1632">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a6a88-1633">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1633">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a6a88-1634">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1634">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a6a88-1635">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1635">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a6a88-1636">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1636">January 17, 2018</span></span>

<span data-ttu-id="a6a88-1637">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a6a88-1637">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1638">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1638">ACR</span></span>

* <span data-ttu-id="a6a88-1639">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1639">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a6a88-1640">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1640">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1641">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1641">ACS</span></span>

* <span data-ttu-id="a6a88-1642">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1642">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a6a88-1643">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1643">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1644">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1644">Appservice</span></span>

* <span data-ttu-id="a6a88-1645">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1645">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a6a88-1646">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1646">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a6a88-1647">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1647">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a6a88-1648">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a6a88-1648">Backup</span></span>

* <span data-ttu-id="a6a88-1649">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1649">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a6a88-1650">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1650">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a6a88-1651">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1651">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a6a88-1652">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1652">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a6a88-1653">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1653">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-1654">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1654">Batch</span></span>

* <span data-ttu-id="a6a88-1655">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1655">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a6a88-1656">Облако</span><span class="sxs-lookup"><span data-stu-id="a6a88-1656">Cloud</span></span>

* <span data-ttu-id="a6a88-1657">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1657">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-1658">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-1658">Consumption</span></span>

* <span data-ttu-id="a6a88-1659">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1659">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6a88-1660">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1660">Event Grid</span></span>

* <span data-ttu-id="a6a88-1661">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1661">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a6a88-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1662">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a6a88-1663">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1663">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a6a88-1664">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1664">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a6a88-1665">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1665">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a6a88-1666">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1666">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a6a88-1667">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1667">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a6a88-1668">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1668">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-1669">Interactive</span><span class="sxs-lookup"><span data-stu-id="a6a88-1669">Interactive</span></span>

* <span data-ttu-id="a6a88-1670">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1670">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a6a88-1671">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1671">Fixed errors on startup</span></span>
* <span data-ttu-id="a6a88-1672">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1672">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-1673">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1673">IoT</span></span>

* <span data-ttu-id="a6a88-1674">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1674">Added support for device provisioning service</span></span>
* <span data-ttu-id="a6a88-1675">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1675">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a6a88-1676">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1676">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1677">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1677">Monitor</span></span>

* <span data-ttu-id="a6a88-1678">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1678">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a6a88-1679">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1679">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a6a88-1680">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1680">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1681">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1681">Network</span></span>

* <span data-ttu-id="a6a88-1682">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1682">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a6a88-1683">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1683">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1684">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1684">Profile</span></span>

* <span data-ttu-id="a6a88-1685">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1685">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1686">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1686">Role</span></span>

* <span data-ttu-id="a6a88-1687">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1687">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6a88-1688">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6a88-1688">Service Fabric</span></span>

* <span data-ttu-id="a6a88-1689">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1689">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a6a88-1690">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1690">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1691">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1691">VM</span></span>

* <span data-ttu-id="a6a88-1692">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1692">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a6a88-1693">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="a6a88-1693">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a6a88-1694">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1694">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a6a88-1695">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1695">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a6a88-1696">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1696">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a6a88-1697">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1697">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6a88-1698">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1698">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6a88-1699">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1699">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a6a88-1700">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1700">December 19, 2017</span></span>

<span data-ttu-id="a6a88-1701">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a6a88-1701">Version 2.0.23</span></span>

* <span data-ttu-id="a6a88-1702">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1702">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1703">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1703">Container</span></span>

* <span data-ttu-id="a6a88-1704">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1704">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1705">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1705">Network</span></span>

* <span data-ttu-id="a6a88-1706">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1706">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a6a88-1707">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1707">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1708">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1708">Storage</span></span>

* <span data-ttu-id="a6a88-1709">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1709">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1710">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1710">VM</span></span>

* <span data-ttu-id="a6a88-1711">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1711">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a6a88-1712">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1712">December 5, 2017</span></span>

<span data-ttu-id="a6a88-1713">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a6a88-1713">Version 2.0.22</span></span>

* <span data-ttu-id="a6a88-1714">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1714">Removed `az component` commands.</span></span> <span data-ttu-id="a6a88-1715">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1715">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1716">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1716">Core</span></span>
* <span data-ttu-id="a6a88-1717">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1717">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a6a88-1718">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1718">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1719">ACS</span></span>

* <span data-ttu-id="a6a88-1720">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1720">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a6a88-1721">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1721">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a6a88-1722">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1722">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a6a88-1723">Помощник</span><span class="sxs-lookup"><span data-stu-id="a6a88-1723">Advisor</span></span>

* <span data-ttu-id="a6a88-1724">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-1724">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1725">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1725">Appservice</span></span>

* <span data-ttu-id="a6a88-1726">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1726">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a6a88-1727">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1727">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a6a88-1728">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1728">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a6a88-1729">Потребление</span><span class="sxs-lookup"><span data-stu-id="a6a88-1729">Consumption</span></span>

* <span data-ttu-id="a6a88-1730">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1730">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1731">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1731">Container</span></span>

* <span data-ttu-id="a6a88-1732">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1732">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1733">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1733">Monitor</span></span>

* <span data-ttu-id="a6a88-1734">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1734">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1735">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1735">Resource</span></span>

* <span data-ttu-id="a6a88-1736">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1736">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-1737">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1737">Role</span></span>

* <span data-ttu-id="a6a88-1738">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1738">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a6a88-1739">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1739">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a6a88-1740">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1740">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1741">SQL</span></span>

* <span data-ttu-id="a6a88-1742">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1742">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a6a88-1743">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1743">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1744">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1744">VM</span></span>

* <span data-ttu-id="a6a88-1745">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1745">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a6a88-1746">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1746">November 14, 2017</span></span>

<span data-ttu-id="a6a88-1747">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a6a88-1747">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1748">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1748">ACR</span></span>

* <span data-ttu-id="a6a88-1749">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1749">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a6a88-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1750">ACS</span></span>

* <span data-ttu-id="a6a88-1751">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1751">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a6a88-1752">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1752">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a6a88-1753">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1753">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a6a88-1754">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1754">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a6a88-1755">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1755">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1756">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1756">Appservice</span></span>

* <span data-ttu-id="a6a88-1757">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1757">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a6a88-1758">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1758">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a6a88-1759">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1759">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a6a88-1760">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1760">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a6a88-1761">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="a6a88-1761">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a6a88-1762">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1762">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-1763">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1763">Batch</span></span>

* <span data-ttu-id="a6a88-1764">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1764">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a6a88-1765">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-1765">Batchai</span></span>

* <span data-ttu-id="a6a88-1766">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1766">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a6a88-1767">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1767">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a6a88-1768">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1768">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a6a88-1769">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1769">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a6a88-1770">Облако</span><span class="sxs-lookup"><span data-stu-id="a6a88-1770">Cloud</span></span>

* <span data-ttu-id="a6a88-1771">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1771">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-1772">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1772">Container</span></span>

* <span data-ttu-id="a6a88-1773">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1773">Added support to open multiple ports</span></span>
* <span data-ttu-id="a6a88-1774">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1774">Added container group restart policy</span></span>
* <span data-ttu-id="a6a88-1775">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1775">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a6a88-1776">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1776">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6a88-1777">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6a88-1777">Data Lake Analytics</span></span>

* <span data-ttu-id="a6a88-1778">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1778">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6a88-1779">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6a88-1779">Data Lake Store</span></span>

* <span data-ttu-id="a6a88-1780">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1780">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1781">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1781">Extension</span></span>

* <span data-ttu-id="a6a88-1782">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1782">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a6a88-1783">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1783">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-1784">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1784">IoT</span></span>

* <span data-ttu-id="a6a88-1785">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1785">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1786">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1786">Monitor</span></span>

* <span data-ttu-id="a6a88-1787">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1787">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1788">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1788">Network</span></span>

* <span data-ttu-id="a6a88-1789">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1789">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a6a88-1790">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1790">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a6a88-1791">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1791">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a6a88-1792">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1792">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a6a88-1793">Резервирование</span><span class="sxs-lookup"><span data-stu-id="a6a88-1793">Reservations</span></span>

* <span data-ttu-id="a6a88-1794">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="a6a88-1794">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1795">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1795">Resource</span></span>

* <span data-ttu-id="a6a88-1796">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1796">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1797">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1797">SQL</span></span>

* <span data-ttu-id="a6a88-1798">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1798">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1799">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1799">Storage</span></span>

* <span data-ttu-id="a6a88-1800">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1800">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a6a88-1801">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1801">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a6a88-1802">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1802">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a6a88-1803">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1803">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a6a88-1804">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1804">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a6a88-1805">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1805">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a6a88-1806">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1806">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1807">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1807">VM</span></span>

* <span data-ttu-id="a6a88-1808">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1808">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a6a88-1809">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1809">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a6a88-1810">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1810">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a6a88-1811">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1811">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a6a88-1812">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1812">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a6a88-1813">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1813">October 24, 2017</span></span>

<span data-ttu-id="a6a88-1814">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a6a88-1814">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1815">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1815">Core</span></span>

* <span data-ttu-id="a6a88-1816">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1816">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-1817">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-1817">ACR</span></span>

* <span data-ttu-id="a6a88-1818">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1818">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a6a88-1819">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="a6a88-1819">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a6a88-1820">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="a6a88-1820">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1821">ACS</span></span>

* <span data-ttu-id="a6a88-1822">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1822">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a6a88-1823">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1823">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1824">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1824">Appservice</span></span>

* <span data-ttu-id="a6a88-1825">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1825">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a6a88-1826">Компонент</span><span class="sxs-lookup"><span data-stu-id="a6a88-1826">Component</span></span>

* <span data-ttu-id="a6a88-1827">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="a6a88-1827">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-1828">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-1828">Monitor</span></span>

* <span data-ttu-id="a6a88-1829">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1829">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1830">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1830">Resource</span></span>

* <span data-ttu-id="a6a88-1831">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1831">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a6a88-1832">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="a6a88-1832">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1833">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1833">VM</span></span>

* <span data-ttu-id="a6a88-1834">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1834">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a6a88-1835">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1835">October 9, 2017</span></span>

<span data-ttu-id="a6a88-1836">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a6a88-1836">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1837">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1837">Core</span></span>

* <span data-ttu-id="a6a88-1838">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1838">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1839">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1839">Appservice</span></span>

* <span data-ttu-id="a6a88-1840">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1840">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-1841">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-1841">Batch</span></span>

* <span data-ttu-id="a6a88-1842">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a6a88-1842">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a6a88-1843">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1843">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a6a88-1844">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1844">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a6a88-1845">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1845">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a6a88-1846">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-1846">Batchai</span></span>

* <span data-ttu-id="a6a88-1847">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a6a88-1847">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-1848">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1848">Keyvault</span></span>

* <span data-ttu-id="a6a88-1849">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1849">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a6a88-1850">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a6a88-1850">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a6a88-1851">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1851">Network</span></span>

* <span data-ttu-id="a6a88-1852">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1852">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a6a88-1853">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1853">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1854">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1854">Resource</span></span>

* <span data-ttu-id="a6a88-1855">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1855">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a6a88-1856">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1856">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a6a88-1857">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1857">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a6a88-1858">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1858">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1859">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1859">Sql</span></span>

* <span data-ttu-id="a6a88-1860">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1860">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a6a88-1861">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1861">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a6a88-1862">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1862">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1863">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1863">Storage</span></span>

* <span data-ttu-id="a6a88-1864">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1864">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1865">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="a6a88-1865">Vm</span></span>

* <span data-ttu-id="a6a88-1866">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1866">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a6a88-1867">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1867">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a6a88-1868">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1868">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a6a88-1869">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1869">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a6a88-1870">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1870">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a6a88-1871">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1871">September 22, 2017</span></span>

<span data-ttu-id="a6a88-1872">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a6a88-1872">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1873">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1873">Resource</span></span>

* <span data-ttu-id="a6a88-1874">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="a6a88-1874">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a6a88-1875">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="a6a88-1875">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a6a88-1876">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1876">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a6a88-1877">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1877">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1878">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1878">Network</span></span>

* <span data-ttu-id="a6a88-1879">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1879">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a6a88-1880">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1880">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a6a88-1881">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1881">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a6a88-1882">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1882">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a6a88-1883">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1883">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a6a88-1884">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1884">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a6a88-1885">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1885">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1886">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1886">Storage</span></span>

* <span data-ttu-id="a6a88-1887">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="a6a88-1887">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a6a88-1888">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="a6a88-1888">Eventgrid</span></span>

* <span data-ttu-id="a6a88-1889">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="a6a88-1889">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1890">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1890">SQL</span></span>

* <span data-ttu-id="a6a88-1891">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1891">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a6a88-1892">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="a6a88-1892">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a6a88-1893">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1893">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-1894">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1894">Keyvault</span></span>

* <span data-ttu-id="a6a88-1895">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="a6a88-1895">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1896">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1896">VM</span></span>

* <span data-ttu-id="a6a88-1897">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1897">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a6a88-1898">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="a6a88-1898">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a6a88-1899">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1899">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a6a88-1900">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1900">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a6a88-1901">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1901">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a6a88-1902">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1902">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1903">ACS</span></span>

* <span data-ttu-id="a6a88-1904">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a6a88-1904">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1905">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1905">Appservice</span></span>

* <span data-ttu-id="a6a88-1906">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a6a88-1906">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a6a88-1907">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a6a88-1907">Backup</span></span>

* <span data-ttu-id="a6a88-1908">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1908">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a6a88-1909">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1909">September 11, 2017</span></span>

<span data-ttu-id="a6a88-1910">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a6a88-1910">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a6a88-1911">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-1911">Core</span></span>

* <span data-ttu-id="a6a88-1912">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1912">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a6a88-1913">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1913">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1914">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1914">Acs</span></span>

* <span data-ttu-id="a6a88-1915">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1915">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a6a88-1916">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1916">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1917">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1917">Appservice</span></span>

* <span data-ttu-id="a6a88-1918">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1918">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-1919">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-1919">CDN</span></span>

* <span data-ttu-id="a6a88-1920">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1920">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a6a88-1921">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a6a88-1921">Extension</span></span>

* <span data-ttu-id="a6a88-1922">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-1922">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-1923">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1923">Keyvault</span></span>

* <span data-ttu-id="a6a88-1924">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1924">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1925">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1925">Network</span></span>

* <span data-ttu-id="a6a88-1926">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1926">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a6a88-1927">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1927">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a6a88-1928">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1928">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a6a88-1929">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1929">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a6a88-1930">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1930">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-1931">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-1931">Resource</span></span>

* <span data-ttu-id="a6a88-1932">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1932">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a6a88-1933">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1933">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a6a88-1934">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1934">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a6a88-1935">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1935">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-1936">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-1936">SQL</span></span>

* <span data-ttu-id="a6a88-1937">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1937">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1938">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1938">VM</span></span>

* <span data-ttu-id="a6a88-1939">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1939">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a6a88-1940">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1940">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a6a88-1941">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1941">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a6a88-1942">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1942">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a6a88-1943">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1943">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a6a88-1944">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1944">August 31, 2017</span></span>

<span data-ttu-id="a6a88-1945">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a6a88-1945">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-1946">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1946">Keyvault</span></span>

* <span data-ttu-id="a6a88-1947">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1947">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a6a88-1948">Sf</span><span class="sxs-lookup"><span data-stu-id="a6a88-1948">Sf</span></span>

* <span data-ttu-id="a6a88-1949">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="a6a88-1949">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1950">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1950">Storage</span></span>

* <span data-ttu-id="a6a88-1951">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1951">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a6a88-1952">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1952">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a6a88-1953">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1953">August 28, 2017</span></span>

<span data-ttu-id="a6a88-1954">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a6a88-1954">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a6a88-1955">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="a6a88-1955">CLI</span></span>

* <span data-ttu-id="a6a88-1956">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1956">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1957">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1957">ACS</span></span>

* <span data-ttu-id="a6a88-1958">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1958">Corrected preview regions</span></span>
* <span data-ttu-id="a6a88-1959">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1959">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a6a88-1960">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1960">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-1961">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-1961">Appservice</span></span>

* <span data-ttu-id="a6a88-1962">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1962">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a6a88-1963">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1963">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a6a88-1964">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1964">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a6a88-1965">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1965">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a6a88-1966">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1966">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-1967">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-1967">IoT</span></span>

* <span data-ttu-id="a6a88-1968">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1968">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-1969">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-1969">Network</span></span>

* <span data-ttu-id="a6a88-1970">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1970">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a6a88-1971">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1971">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a6a88-1972">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1972">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a6a88-1973">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1973">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a6a88-1974">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1974">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-1975">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-1975">Profile</span></span>

* <span data-ttu-id="a6a88-1976">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1976">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6a88-1977">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6a88-1977">Service Fabric</span></span>

* <span data-ttu-id="a6a88-1978">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1978">Preview release</span></span>
* <span data-ttu-id="a6a88-1979">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1979">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a6a88-1980">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1980">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a6a88-1981">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1981">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-1982">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-1982">Storage</span></span>

* <span data-ttu-id="a6a88-1983">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1983">Enabled setting blob tier</span></span>
* <span data-ttu-id="a6a88-1984">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1984">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a6a88-1985">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1985">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a6a88-1986">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1986">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a6a88-1987">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1987">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a6a88-1988">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1988">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-1989">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-1989">VM</span></span>

* <span data-ttu-id="a6a88-1990">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1990">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a6a88-1991">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1991">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a6a88-1992">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1992">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a6a88-1993">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1993">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a6a88-1994">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1994">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a6a88-1995">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1995">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a6a88-1996">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1996">August 15, 2017</span></span>

<span data-ttu-id="a6a88-1997">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a6a88-1997">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-1998">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-1998">ACS</span></span>

* <span data-ttu-id="a6a88-1999">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a6a88-1999">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-2000">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-2000">Appservice</span></span>

* <span data-ttu-id="a6a88-2001">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2001">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6a88-2002">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-2002">Event Grid</span></span>

* <span data-ttu-id="a6a88-2003">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2003">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a6a88-2004">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2004">August 11, 2017</span></span>

<span data-ttu-id="a6a88-2005">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a6a88-2005">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-2006">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-2006">ACS</span></span>

* <span data-ttu-id="a6a88-2007">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2007">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-2008">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-2008">Batch</span></span>

* <span data-ttu-id="a6a88-2009">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2009">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a6a88-2010">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2010">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a6a88-2011">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2011">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a6a88-2012">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2012">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a6a88-2013">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2013">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a6a88-2014">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2014">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a6a88-2015">Компонент</span><span class="sxs-lookup"><span data-stu-id="a6a88-2015">Component</span></span>

* <span data-ttu-id="a6a88-2016">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2016">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a6a88-2017">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a6a88-2017">Container</span></span>

* <span data-ttu-id="a6a88-2018">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2018">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a6a88-2019">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6a88-2019">Data Lake Store</span></span>

* <span data-ttu-id="a6a88-2020">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2020">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a6a88-2021">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-2021">Event Grid</span></span>

* <span data-ttu-id="a6a88-2022">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a6a88-2022">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-2023">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-2023">Network</span></span>

* <span data-ttu-id="a6a88-2024">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2024">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a6a88-2025">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2025">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a6a88-2026">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2026">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a6a88-2027">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2027">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-2028">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-2028">Profile</span></span>

* <span data-ttu-id="a6a88-2029">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2029">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-2030">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-2030">Storage</span></span>

* <span data-ttu-id="a6a88-2031">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2031">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-2032">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-2032">VM</span></span>

* <span data-ttu-id="a6a88-2033">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2033">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a6a88-2034">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2034">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a6a88-2035">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2035">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a6a88-2036">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2036">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a6a88-2037">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2037">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a6a88-2038">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2038">July 28, 2017</span></span>

<span data-ttu-id="a6a88-2039">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a6a88-2039">Version 2.0.12</span></span>

* <span data-ttu-id="a6a88-2040">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2040">Added container commands</span></span>
* <span data-ttu-id="a6a88-2041">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2041">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a6a88-2042">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-2042">Core</span></span>

* <span data-ttu-id="a6a88-2043">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2043">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a6a88-2044">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2044">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a6a88-2045">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2045">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a6a88-2046">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2046">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a6a88-2047">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2047">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a6a88-2048">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2048">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a6a88-2049">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2049">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a6a88-2050">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2050">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a6a88-2051">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2051">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a6a88-2052">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2052">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a6a88-2053">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2053">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a6a88-2054">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2054">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a6a88-2055">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2055">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a6a88-2056">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2056">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a6a88-2057">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2057">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a6a88-2058">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2058">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a6a88-2059">ACR</span><span class="sxs-lookup"><span data-stu-id="a6a88-2059">ACR</span></span>

* <span data-ttu-id="a6a88-2060">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2060">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a6a88-2061">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2061">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a6a88-2062">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2062">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a6a88-2063">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2063">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a6a88-2064">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2064">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a6a88-2065">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2065">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-2066">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-2066">ACS</span></span>

* <span data-ttu-id="a6a88-2067">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2067">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-2068">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a6a88-2068">Appservice</span></span>

* <span data-ttu-id="a6a88-2069">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2069">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a6a88-2070">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2070">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a6a88-2071">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2071">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a6a88-2072">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2072">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a6a88-2073">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2073">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a6a88-2074">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2074">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a6a88-2075">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2075">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a6a88-2076">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2076">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a6a88-2077">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2077">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a6a88-2078">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2078">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a6a88-2079">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a6a88-2079">Batch</span></span>

* <span data-ttu-id="a6a88-2080">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2080">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a6a88-2081">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2081">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a6a88-2082">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2082">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a6a88-2083">CDN</span><span class="sxs-lookup"><span data-stu-id="a6a88-2083">CDN</span></span>

* <span data-ttu-id="a6a88-2084">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2084">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a6a88-2085">Облако</span><span class="sxs-lookup"><span data-stu-id="a6a88-2085">Cloud</span></span>

* <span data-ttu-id="a6a88-2086">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2086">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a6a88-2087">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2087">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a6a88-2088">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2088">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a6a88-2089">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2089">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a6a88-2090">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2090">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-2091">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-2091">CosmosDB</span></span>

* <span data-ttu-id="a6a88-2092">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2092">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a6a88-2093">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2093">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6a88-2094">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6a88-2094">Data Lake Analytics</span></span>

* <span data-ttu-id="a6a88-2095">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2095">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a6a88-2096">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2096">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a6a88-2097">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2097">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6a88-2098">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6a88-2098">Data Lake Store</span></span>

* <span data-ttu-id="a6a88-2099">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2099">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a6a88-2100">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2100">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a6a88-2101">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2101">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a6a88-2102">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2102">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a6a88-2103">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="a6a88-2103">Interactive</span></span>

* <span data-ttu-id="a6a88-2104">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2104">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a6a88-2105">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2105">Increased test coverage</span></span>
* <span data-ttu-id="a6a88-2106">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2106">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a6a88-2107">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2107">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a6a88-2108">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2108">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a6a88-2109">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2109">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a6a88-2110">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2110">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a6a88-2111">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2111">Added `--progress` flag</span></span>
* <span data-ttu-id="a6a88-2112">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2112">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a6a88-2113">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2113">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a6a88-2114">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a6a88-2114">IoT</span></span>

* <span data-ttu-id="a6a88-2115">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="a6a88-2115">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a6a88-2116">(3934).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2116">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a6a88-2117">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-2117">Key vault</span></span>

* <span data-ttu-id="a6a88-2118">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="a6a88-2118">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a6a88-2119">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2119">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a6a88-2120">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2120">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a6a88-2121">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2121">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a6a88-2122">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2122">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a6a88-2123">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2123">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a6a88-2124">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="a6a88-2124">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a6a88-2125">(3307).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2125">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a6a88-2126">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a6a88-2126">Lab</span></span>

* <span data-ttu-id="a6a88-2127">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2127">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a6a88-2128">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2128">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-2129">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-2129">Monitor</span></span>

* <span data-ttu-id="a6a88-2130">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2130">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a6a88-2131">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2131">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a6a88-2132">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2132">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a6a88-2133">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2133">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a6a88-2134">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2134">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a6a88-2135">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="a6a88-2135">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a6a88-2136">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2136">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a6a88-2137">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2137">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a6a88-2138">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2138">`location` no longer required</span></span>
  * <span data-ttu-id="a6a88-2139">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2139">Add name and ID support for target</span></span>
  * <span data-ttu-id="a6a88-2140">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2140">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a6a88-2141">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2141">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a6a88-2142">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2142">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a6a88-2143">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2143">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a6a88-2144">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2144">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a6a88-2145">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2145">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-2146">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-2146">Network</span></span>

* <span data-ttu-id="a6a88-2147">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2147">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a6a88-2148">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2148">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a6a88-2149">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2149">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a6a88-2150">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2150">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a6a88-2151">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2151">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a6a88-2152">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2152">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a6a88-2153">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2153">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a6a88-2154">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2154">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a6a88-2155">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2155">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a6a88-2156">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2156">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a6a88-2157">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2157">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a6a88-2158">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2158">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a6a88-2159">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2159">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a6a88-2160">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2160">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a6a88-2161">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2161">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a6a88-2162">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2162">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a6a88-2163">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2163">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a6a88-2164">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2164">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a6a88-2165">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2165">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a6a88-2166">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2166">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a6a88-2167">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2167">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a6a88-2168">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2168">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a6a88-2169">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2169">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a6a88-2170">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2170">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a6a88-2171">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2171">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a6a88-2172">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2172">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a6a88-2173">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2173">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-2174">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-2174">Profile</span></span>

* <span data-ttu-id="a6a88-2175">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2175">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a6a88-2176">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2176">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a6a88-2177">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2177">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a6a88-2178">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2178">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a6a88-2179">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2179">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a6a88-2180">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a6a88-2180">RDBMS</span></span>

* <span data-ttu-id="a6a88-2181">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2181">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a6a88-2182">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2182">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a6a88-2183">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2183">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a6a88-2184">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2184">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-2185">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-2185">Resource</span></span>

* <span data-ttu-id="a6a88-2186">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2186">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a6a88-2187">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2187">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a6a88-2188">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2188">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a6a88-2189">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2189">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a6a88-2190">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2190">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a6a88-2191">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2191">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a6a88-2192">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2192">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a6a88-2193">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2193">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-2194">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-2194">Role</span></span>

* <span data-ttu-id="a6a88-2195">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2195">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a6a88-2196">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2196">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a6a88-2197">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2197">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a6a88-2198">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2198">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a6a88-2199">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2199">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a6a88-2200">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a6a88-2200">Service Fabric</span></span>
* <span data-ttu-id="a6a88-2201">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2201">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a6a88-2202">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2202">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a6a88-2203">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2203">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-2204">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-2204">SQL</span></span>

* <span data-ttu-id="a6a88-2205">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2205">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a6a88-2206">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2206">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a6a88-2207">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2207">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-2208">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-2208">Storage</span></span>

* <span data-ttu-id="a6a88-2209">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2209">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a6a88-2210">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2210">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a6a88-2211">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2211">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a6a88-2212">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="a6a88-2212">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a6a88-2213">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2213">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a6a88-2214">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2214">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-2215">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-2215">VM</span></span>

* <span data-ttu-id="a6a88-2216">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2216">Support configuring nsg</span></span>
* <span data-ttu-id="a6a88-2217">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2217">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a6a88-2218">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2218">Support managed service identities</span></span>
* <span data-ttu-id="a6a88-2219">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2219">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a6a88-2220">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2220">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a6a88-2221">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2221">May 10, 2017</span></span>

<span data-ttu-id="a6a88-2222">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a6a88-2222">Version 2.0.6</span></span>

* <span data-ttu-id="a6a88-2223">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2223">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a6a88-2224">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2224">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a6a88-2225">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2225">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a6a88-2226">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2226">Include Cognitive Services module</span></span>
* <span data-ttu-id="a6a88-2227">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2227">Include Service Fabric module</span></span>
* <span data-ttu-id="a6a88-2228">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2228">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a6a88-2229">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2229">Add support for CDN commands</span></span>
* <span data-ttu-id="a6a88-2230">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2230">Remove Container module</span></span>
* <span data-ttu-id="a6a88-2231">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2231">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a6a88-2232">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2232">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a6a88-2233">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-2233">Core</span></span>

* <span data-ttu-id="a6a88-2234">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2234">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a6a88-2235">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2235">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a6a88-2236">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2236">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a6a88-2237">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2237">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a6a88-2238">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2238">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a6a88-2239">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2239">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a6a88-2240">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2240">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a6a88-2241">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2241">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a6a88-2242">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2242">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a6a88-2243">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2243">core: Improved performance</span></span>
* <span data-ttu-id="a6a88-2244">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2244">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a6a88-2245">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2245">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-2246">ACS</span></span>

* <span data-ttu-id="a6a88-2247">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2247">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a6a88-2248">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2248">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a6a88-2249">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2249">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a6a88-2250">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2250">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-2251">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-2251">AppService</span></span>

* <span data-ttu-id="a6a88-2252">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2252">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a6a88-2253">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2253">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a6a88-2254">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2254">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a6a88-2255">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2255">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a6a88-2256">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2256">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a6a88-2257">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2257">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a6a88-2258">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2258">support slot swap with preview</span></span>
* <span data-ttu-id="a6a88-2259">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2259">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a6a88-2260">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2260">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a6a88-2261">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a6a88-2261">CosmosDB</span></span>

* <span data-ttu-id="a6a88-2262">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2262">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a6a88-2263">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2263">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a6a88-2264">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2264">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a6a88-2265">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2265">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a6a88-2266">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a6a88-2266">Data Lake Analytics</span></span>

* <span data-ttu-id="a6a88-2267">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2267">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a6a88-2268">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2268">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a6a88-2269">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2269">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a6a88-2270">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="a6a88-2270">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a6a88-2271">Таблица</span><span class="sxs-lookup"><span data-stu-id="a6a88-2271">Table</span></span>
  * <span data-ttu-id="a6a88-2272">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="a6a88-2272">Table valued function</span></span>
  * <span data-ttu-id="a6a88-2273">Просмотр</span><span class="sxs-lookup"><span data-stu-id="a6a88-2273">View</span></span>
  * <span data-ttu-id="a6a88-2274">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2274">Table Statistics.</span></span> <span data-ttu-id="a6a88-2275">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2275">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a6a88-2276">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a6a88-2276">Data Lake Store</span></span>

* <span data-ttu-id="a6a88-2277">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2277">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a6a88-2278">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2278">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a6a88-2279">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2279">missed help for access show.</span></span> <span data-ttu-id="a6a88-2280">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2280">adding it.</span></span> <span data-ttu-id="a6a88-2281">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a6a88-2281">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a6a88-2282">Поиск</span><span class="sxs-lookup"><span data-stu-id="a6a88-2282">Find</span></span>

* <span data-ttu-id="a6a88-2283">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2283">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a6a88-2284">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a6a88-2284">KeyVault</span></span>

* <span data-ttu-id="a6a88-2285">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2285">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a6a88-2286">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2286">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a6a88-2287">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2287">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a6a88-2288">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2288">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a6a88-2289">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2289">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a6a88-2290">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a6a88-2290">Lab</span></span>

* <span data-ttu-id="a6a88-2291">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2291">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a6a88-2292">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2292">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a6a88-2293">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2293">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a6a88-2294">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2294">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a6a88-2295">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2295">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a6a88-2296">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a6a88-2296">Monitor</span></span>

* <span data-ttu-id="a6a88-2297">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2297">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a6a88-2298">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2298">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a6a88-2299">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-2299">Network</span></span>

* <span data-ttu-id="a6a88-2300">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2300">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a6a88-2301">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2301">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a6a88-2302">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2302">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a6a88-2303">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2303">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a6a88-2304">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2304">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a6a88-2305">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2305">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a6a88-2306">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2306">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a6a88-2307">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2307">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a6a88-2308">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2308">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a6a88-2309">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="a6a88-2309">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a6a88-2310">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2310">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a6a88-2311">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2311">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a6a88-2312">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2312">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a6a88-2313">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2313">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a6a88-2314">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2314">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a6a88-2315">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2315">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a6a88-2316">Профиль</span><span class="sxs-lookup"><span data-stu-id="a6a88-2316">Profile</span></span>

* <span data-ttu-id="a6a88-2317">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2317">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a6a88-2318">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2318">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a6a88-2319">Redis</span><span class="sxs-lookup"><span data-stu-id="a6a88-2319">Redis</span></span>

* <span data-ttu-id="a6a88-2320">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2320">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a6a88-2321">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2321">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a6a88-2322">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a6a88-2322">Resource</span></span>

* <span data-ttu-id="a6a88-2323">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2323">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a6a88-2324">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2324">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a6a88-2325">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2325">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a6a88-2326">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2326">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a6a88-2327">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a6a88-2327">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a6a88-2328">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2328">Add docs for az lock update.</span></span> <span data-ttu-id="a6a88-2329">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a6a88-2329">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a6a88-2330">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2330">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a6a88-2331">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a6a88-2331">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a6a88-2332">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2332">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a6a88-2333">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a6a88-2333">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a6a88-2334">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2334">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a6a88-2335">Роль</span><span class="sxs-lookup"><span data-stu-id="a6a88-2335">Role</span></span>

* <span data-ttu-id="a6a88-2336">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2336">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a6a88-2337">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2337">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a6a88-2338">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2338">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a6a88-2339">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2339">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a6a88-2340">SQL</span><span class="sxs-lookup"><span data-stu-id="a6a88-2340">SQL</span></span>

* <span data-ttu-id="a6a88-2341">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2341">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a6a88-2342">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2342">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a6a88-2343">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-2343">Storage</span></span>

* <span data-ttu-id="a6a88-2344">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2344">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a6a88-2345">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2345">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a6a88-2346">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2346">Add support for large block blob upload</span></span>
* <span data-ttu-id="a6a88-2347">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2347">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-2348">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-2348">VM</span></span>

* <span data-ttu-id="a6a88-2349">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2349">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a6a88-2350">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="a6a88-2350">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a6a88-2351">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a6a88-2351">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a6a88-2352">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a6a88-2352">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a6a88-2353">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2353">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a6a88-2354">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2354">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a6a88-2355">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2355">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a6a88-2356">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2356">April 3, 2017</span></span>

<span data-ttu-id="a6a88-2357">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a6a88-2357">Version 2.0.2</span></span>

<span data-ttu-id="a6a88-2358">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2358">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a6a88-2359">Core</span><span class="sxs-lookup"><span data-stu-id="a6a88-2359">Core</span></span>

* <span data-ttu-id="a6a88-2360">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2360">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a6a88-2361">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2361">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a6a88-2362">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2362">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a6a88-2363">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2363">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a6a88-2364">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2364">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a6a88-2365">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="a6a88-2365">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a6a88-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2366">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a6a88-2367">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2367">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a6a88-2368">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2368">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a6a88-2369">ACS</span><span class="sxs-lookup"><span data-stu-id="a6a88-2369">ACS</span></span>

* <span data-ttu-id="a6a88-2370">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2370">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a6a88-2371">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="a6a88-2371">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a6a88-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2372">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a6a88-2373">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="a6a88-2373">Add support for windows clusters.</span></span> <span data-ttu-id="a6a88-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2374">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a6a88-2375">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="a6a88-2375">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a6a88-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2376">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a6a88-2377">AppService</span><span class="sxs-lookup"><span data-stu-id="a6a88-2377">AppService</span></span>

* <span data-ttu-id="a6a88-2378">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2378">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a6a88-2379">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2379">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a6a88-2380">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2380">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a6a88-2381">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2381">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a6a88-2382">Data Lake</span><span class="sxs-lookup"><span data-stu-id="a6a88-2382">DataLake</span></span>

* <span data-ttu-id="a6a88-2383">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2383">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a6a88-2384">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2384">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a6a88-2385">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a6a88-2385">DocuemntDB</span></span>

* <span data-ttu-id="a6a88-2386">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2386">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a6a88-2387">ВМ</span><span class="sxs-lookup"><span data-stu-id="a6a88-2387">VM</span></span>

* <span data-ttu-id="a6a88-2388">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2388">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a6a88-2389">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2389">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a6a88-2390">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2390">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a6a88-2391">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2391">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a6a88-2392">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2392">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a6a88-2393">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2393">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="a6a88-2394">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2394">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a6a88-2395">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2395">February 27, 2017</span></span>

<span data-ttu-id="a6a88-2396">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a6a88-2396">Version 2.0.0</span></span>

<span data-ttu-id="a6a88-2397">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="a6a88-2397">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a6a88-2398">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="a6a88-2398">Container Service (acs)</span></span>
- <span data-ttu-id="a6a88-2399">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="a6a88-2399">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a6a88-2400">Сеть</span><span class="sxs-lookup"><span data-stu-id="a6a88-2400">Networking</span></span>
- <span data-ttu-id="a6a88-2401">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a6a88-2401">Storage</span></span>

<span data-ttu-id="a6a88-2402">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2402">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a6a88-2403">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2403">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a6a88-2404">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2404">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a6a88-2405">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2405">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a6a88-2406">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a6a88-2406">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a6a88-2407">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="a6a88-2407">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a6a88-2408">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="a6a88-2408">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a6a88-2409">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="a6a88-2409">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a6a88-2410">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a6a88-2410">Provide feedback from the command line with the `az feedback` command</span></span>

