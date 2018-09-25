---
title: Начало работы с Azure CLI 2.0
description: Начните работу с Azure CLI 2.0, изучив базовые команды.
keywords: Azure CLI, CLI help, Azure help, query, automation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 00cfca8d55f0b404cae32ba9b4ce464dfa8afa08
ms.sourcegitcommit: 8318ce761c279afa4cd45a81a58d83fc38c616bc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2018
ms.locfileid: "45561581"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="c3224-104">Начало работы с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c3224-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="c3224-105">Добро пожаловать в Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="c3224-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="c3224-106">CLI — это средство, предназначенное для быстрой и эффективной работы со службами Azure с возможностью автоматизации.</span><span class="sxs-lookup"><span data-stu-id="c3224-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="c3224-107">В этой статье рассматриваются возможности CLI и приводятся ссылки на связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="c3224-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="c3224-108">Установка или запуск в Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="c3224-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="c3224-109">Самый простой способ приступить к работе с Azure CLI —запустить CLI в среде Azure Cloud Shell через браузер.</span><span class="sxs-lookup"><span data-stu-id="c3224-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="c3224-110">Дополнительные сведения о Cloud Shell см. в [кратком руководстве по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="c3224-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="c3224-111">Сведения об установке CLI см. в разделе [Установка Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c3224-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="c3224-112">Вход</span><span class="sxs-lookup"><span data-stu-id="c3224-112">Sign in</span></span>

<span data-ttu-id="c3224-113">Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="c3224-113">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="c3224-114">Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c3224-114">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="c3224-115">Стандартные команды</span><span class="sxs-lookup"><span data-stu-id="c3224-115">Common commands</span></span>

<span data-ttu-id="c3224-116">В таблице приведены некоторые распространенные команды CLI и ссылки на справочную документацию.</span><span class="sxs-lookup"><span data-stu-id="c3224-116">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="c3224-117">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="c3224-117">Resource type</span></span> | <span data-ttu-id="c3224-118">Группа команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c3224-118">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="c3224-119">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="c3224-119">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="c3224-120">az group</span><span class="sxs-lookup"><span data-stu-id="c3224-120">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="c3224-121">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="c3224-121">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="c3224-122">az vm</span><span class="sxs-lookup"><span data-stu-id="c3224-122">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="c3224-123">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="c3224-123">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="c3224-124">az storage account</span><span class="sxs-lookup"><span data-stu-id="c3224-124">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="c3224-125">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="c3224-125">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="c3224-126">az keyvault</span><span class="sxs-lookup"><span data-stu-id="c3224-126">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="c3224-127">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="c3224-127">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="c3224-128">az webapp</span><span class="sxs-lookup"><span data-stu-id="c3224-128">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="c3224-129">Базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="c3224-129">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="c3224-130">az sql server</span><span class="sxs-lookup"><span data-stu-id="c3224-130">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="c3224-131">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c3224-131">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="c3224-132">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="c3224-132">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="c3224-133">Поиск команд</span><span class="sxs-lookup"><span data-stu-id="c3224-133">Finding commands</span></span>

<span data-ttu-id="c3224-134">Команды CLI организованы в виде _групп_ _команд_.</span><span class="sxs-lookup"><span data-stu-id="c3224-134">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="c3224-135">Каждая группа представляет службу Azure, с которой работают эти команды.</span><span class="sxs-lookup"><span data-stu-id="c3224-135">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="c3224-136">Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="c3224-136">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="c3224-137">Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="c3224-137">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="c3224-138">Аргумент `--help` позволяет получить полный список команд и подгрупп в группе.</span><span class="sxs-lookup"><span data-stu-id="c3224-138">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="c3224-139">Например, вот как можно найти команды CLI для работы с группами безопасности сети (NSG):</span><span class="sxs-lookup"><span data-stu-id="c3224-139">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="c3224-140">В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.</span><span class="sxs-lookup"><span data-stu-id="c3224-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="c3224-141">Глобально доступные аргументы</span><span class="sxs-lookup"><span data-stu-id="c3224-141">Globally available arguments</span></span>

<span data-ttu-id="c3224-142">Для каждой команды есть ряд аргументов.</span><span class="sxs-lookup"><span data-stu-id="c3224-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="c3224-143">`--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.</span><span class="sxs-lookup"><span data-stu-id="c3224-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="c3224-144">`--output` изменяет формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="c3224-144">`--output` changes the output format.</span></span> <span data-ttu-id="c3224-145">Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции) и `table` (понятные таблицы ASCII).</span><span class="sxs-lookup"><span data-stu-id="c3224-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="c3224-146">По умолчанию CLI выводит формат `json`.</span><span class="sxs-lookup"><span data-stu-id="c3224-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="c3224-147">См. дополнительные сведения о [форматах выходных данных для Azure CLI 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c3224-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="c3224-148">`--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure.</span><span class="sxs-lookup"><span data-stu-id="c3224-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="c3224-149">См. дополнительные сведения о [создании запросов о результатах команд в Azure CLI 2.0](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="c3224-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="c3224-150">`--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="c3224-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="c3224-151">`--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки.</span><span class="sxs-lookup"><span data-stu-id="c3224-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="c3224-152">Если вы обнаружили ошибку, включите выходные данные, полученные с помощью флага `--debug`, в отправляемый отчет об ошибке.</span><span class="sxs-lookup"><span data-stu-id="c3224-152">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="c3224-153">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="c3224-153">Interactive mode</span></span>

<span data-ttu-id="c3224-154">CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд.</span><span class="sxs-lookup"><span data-stu-id="c3224-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="c3224-155">Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="c3224-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="c3224-156">См. дополнительные сведения об [интерактивном режиме Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c3224-156">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="c3224-157">Также доступно [расширение для Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), которое предлагает интерактивный интерфейс с функциями автозавершения и отображения документации при наведении курсора.</span><span class="sxs-lookup"><span data-stu-id="c3224-157">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="c3224-158">Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах</span><span class="sxs-lookup"><span data-stu-id="c3224-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="c3224-159">Чтобы приступить к работе с Azure CLI 2.0, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для запроса ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="c3224-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="c3224-160">Создание виртуальных машин с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c3224-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="c3224-161">Также доступны краткие руководства по работе с другими популярными службами.</span><span class="sxs-lookup"><span data-stu-id="c3224-161">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="c3224-162">Создание учетной записи хранения с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c3224-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="c3224-163">Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="c3224-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="c3224-164">Создание отдельной базы данных SQL Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c3224-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="c3224-165">Создание базы данных Azure для сервера MySQL с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="c3224-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="c3224-166">[Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="c3224-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="c3224-167">Создание веб-приложения Python в Azure</span><span class="sxs-lookup"><span data-stu-id="c3224-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="c3224-168">Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров</span><span class="sxs-lookup"><span data-stu-id="c3224-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="c3224-169">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="c3224-169">Give feedback</span></span>

<span data-ttu-id="c3224-170">Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки.</span><span class="sxs-lookup"><span data-stu-id="c3224-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="c3224-171">Вы можете [опубликовать описание проблемы на Github](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="c3224-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
