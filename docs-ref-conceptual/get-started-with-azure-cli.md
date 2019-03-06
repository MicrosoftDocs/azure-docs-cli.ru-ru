---
title: Начало работы с Azure CLI
description: Начните работу с Azure CLI, изучив базовые команды.
keywords: Azure CLI, CLI help, Azure help, query, automation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ddee71f39500b63065a3f71d01b3bed1a7311a52
ms.sourcegitcommit: 943598f8bf05ee058593ca0d72aec507aa26c242
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2019
ms.locfileid: "56963465"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="5c929-104">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-104">Get started with Azure CLI</span></span>

<span data-ttu-id="5c929-105">Добро пожаловать в Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="5c929-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="5c929-106">CLI — это средство, предназначенное для быстрой и эффективной работы со службами Azure с возможностью автоматизации.</span><span class="sxs-lookup"><span data-stu-id="5c929-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="5c929-107">В этой статье рассматриваются возможности CLI и приводятся ссылки на связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="5c929-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="5c929-108">Установка или запуск в Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5c929-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="5c929-109">Самый простой способ приступить к работе с Azure CLI —запустить CLI в среде Azure Cloud Shell через браузер.</span><span class="sxs-lookup"><span data-stu-id="5c929-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="5c929-110">Дополнительные сведения о Cloud Shell см. в [кратком руководстве по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="5c929-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="5c929-111">Сведения об установке CLI см. в разделе [Установка Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c929-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="5c929-112">Установив CLI впервые, проверьте правильность установки и версии, выполнив команду `az --version`.</span><span class="sxs-lookup"><span data-stu-id="5c929-112">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

## <a name="sign-in"></a><span data-ttu-id="5c929-113">Вход</span><span class="sxs-lookup"><span data-stu-id="5c929-113">Sign in</span></span>

<span data-ttu-id="5c929-114">Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5c929-114">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5c929-115">После входа в систему появится список подписок, связанных с учетной записью Azure.</span><span class="sxs-lookup"><span data-stu-id="5c929-115">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="5c929-116">В сведениях о подписке с `isDefault: true` указана текущая активная подписка, отображаемая после входа.</span><span class="sxs-lookup"><span data-stu-id="5c929-116">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="5c929-117">Чтобы выбрать другую подписку, укажите идентификатор подписки с помощью команды [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="5c929-117">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="5c929-118">См. дополнительные сведения о [выборе нужной подписки при использовании нескольких подписок Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c929-118">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="5c929-119">Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c929-119">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="5c929-120">Стандартные команды</span><span class="sxs-lookup"><span data-stu-id="5c929-120">Common commands</span></span>

<span data-ttu-id="5c929-121">В таблице приведены некоторые распространенные команды CLI и ссылки на справочную документацию.</span><span class="sxs-lookup"><span data-stu-id="5c929-121">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="5c929-122">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="5c929-122">Resource type</span></span> | <span data-ttu-id="5c929-123">Группа команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-123">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="5c929-124">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="5c929-124">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="5c929-125">az group</span><span class="sxs-lookup"><span data-stu-id="5c929-125">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="5c929-126">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="5c929-126">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="5c929-127">az vm</span><span class="sxs-lookup"><span data-stu-id="5c929-127">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="5c929-128">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="5c929-128">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="5c929-129">az storage account</span><span class="sxs-lookup"><span data-stu-id="5c929-129">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="5c929-130">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="5c929-130">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="5c929-131">az keyvault</span><span class="sxs-lookup"><span data-stu-id="5c929-131">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="5c929-132">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="5c929-132">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="5c929-133">az webapp</span><span class="sxs-lookup"><span data-stu-id="5c929-133">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="5c929-134">Базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="5c929-134">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="5c929-135">az sql server</span><span class="sxs-lookup"><span data-stu-id="5c929-135">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="5c929-136">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5c929-136">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="5c929-137">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="5c929-137">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="5c929-138">Поиск команд</span><span class="sxs-lookup"><span data-stu-id="5c929-138">Finding commands</span></span>

<span data-ttu-id="5c929-139">Команды CLI организованы в виде _групп_ _команд_.</span><span class="sxs-lookup"><span data-stu-id="5c929-139">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="5c929-140">Каждая группа представляет службу Azure, с которой работают эти команды.</span><span class="sxs-lookup"><span data-stu-id="5c929-140">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="5c929-141">Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="5c929-141">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="5c929-142">Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="5c929-142">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="5c929-143">Аргумент `--help` позволяет получить полный список команд и подгрупп в группе.</span><span class="sxs-lookup"><span data-stu-id="5c929-143">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="5c929-144">Например, вот как можно найти команды CLI для работы с группами безопасности сети (NSG):</span><span class="sxs-lookup"><span data-stu-id="5c929-144">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="5c929-145">В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.</span><span class="sxs-lookup"><span data-stu-id="5c929-145">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="5c929-146">Глобально доступные аргументы</span><span class="sxs-lookup"><span data-stu-id="5c929-146">Globally available arguments</span></span>

<span data-ttu-id="5c929-147">Для каждой команды есть ряд аргументов.</span><span class="sxs-lookup"><span data-stu-id="5c929-147">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="5c929-148">`--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.</span><span class="sxs-lookup"><span data-stu-id="5c929-148">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="5c929-149">`--output` изменяет формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5c929-149">`--output` changes the output format.</span></span> <span data-ttu-id="5c929-150">Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции), `table` (понятные таблицы ASCII) и `yaml`.</span><span class="sxs-lookup"><span data-stu-id="5c929-150">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="5c929-151">По умолчанию CLI выводит формат `json`.</span><span class="sxs-lookup"><span data-stu-id="5c929-151">By default the CLI outputs `json`.</span></span> <span data-ttu-id="5c929-152">См. дополнительные сведения о [форматах выходных данных для Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c929-152">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="5c929-153">`--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure.</span><span class="sxs-lookup"><span data-stu-id="5c929-153">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="5c929-154">См. дополнительные сведения о [создании запросов к результатам выполнения команд в Azure CLI](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="5c929-154">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="5c929-155">`--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="5c929-155">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="5c929-156">`--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки.</span><span class="sxs-lookup"><span data-stu-id="5c929-156">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="5c929-157">Если вы обнаружили ошибку, включите выходные данные, полученные с помощью флага `--debug`, в отправляемый отчет об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5c929-157">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="5c929-158">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="5c929-158">Interactive mode</span></span>

<span data-ttu-id="5c929-159">CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд.</span><span class="sxs-lookup"><span data-stu-id="5c929-159">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="5c929-160">Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="5c929-160">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="5c929-161">См. дополнительные сведения об [интерактивном режиме Azure CLI](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5c929-161">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="5c929-162">Также доступно [расширение для Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), которое предлагает интерактивный интерфейс с функциями автозавершения и отображения документации при наведении курсора.</span><span class="sxs-lookup"><span data-stu-id="5c929-162">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="5c929-163">Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах</span><span class="sxs-lookup"><span data-stu-id="5c929-163">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="5c929-164">Чтобы приступить к работе с Azure CLI, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для выполнения запросов к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="5c929-164">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5c929-165">Руководство по созданию виртуальных машин с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-165">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="5c929-166">Также доступны краткие руководства по работе с другими популярными службами.</span><span class="sxs-lookup"><span data-stu-id="5c929-166">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="5c929-167">Создание учетной записи хранения с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-167">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="5c929-168">Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-168">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="5c929-169">Создание отдельной базы данных SQL Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-169">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="5c929-170">Создание базы данных Azure для сервера MySQL с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c929-170">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="5c929-171">[Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="5c929-171">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="5c929-172">Создание веб-приложения Python в Azure</span><span class="sxs-lookup"><span data-stu-id="5c929-172">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="5c929-173">Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров</span><span class="sxs-lookup"><span data-stu-id="5c929-173">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="5c929-174">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="5c929-174">Give feedback</span></span>

<span data-ttu-id="5c929-175">Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки.</span><span class="sxs-lookup"><span data-stu-id="5c929-175">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="5c929-176">Вы можете [опубликовать описание проблемы на GitHub](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="5c929-176">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
