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
ms.openlocfilehash: 165da295d187edf7dbc19a332670fd49d8f8bdd5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388564"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="da744-104">Начало работы с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="da744-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="da744-105">Добро пожаловать в Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="da744-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="da744-106">CLI — это средство, предназначенное для быстрой и эффективной работы со службами Azure с возможностью автоматизации.</span><span class="sxs-lookup"><span data-stu-id="da744-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="da744-107">В этой статье рассматриваются возможности CLI и приводятся ссылки на связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="da744-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="da744-108">Установка и вход</span><span class="sxs-lookup"><span data-stu-id="da744-108">Install and sign in</span></span>

<span data-ttu-id="da744-109">Вы можете [установить CLI](install-azure-cli.md) или попробовать поработать с [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="da744-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="da744-110">Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="da744-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="da744-111">Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="da744-111">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="da744-112">Стандартные команды</span><span class="sxs-lookup"><span data-stu-id="da744-112">Common commands</span></span>

<span data-ttu-id="da744-113">В таблице приведены некоторые распространенные команды CLI и ссылки на справочную документацию.</span><span class="sxs-lookup"><span data-stu-id="da744-113">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="da744-114">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="da744-114">Resource type</span></span> | <span data-ttu-id="da744-115">Группа команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="da744-115">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="da744-116">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="da744-116">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="da744-117">az group</span><span class="sxs-lookup"><span data-stu-id="da744-117">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="da744-118">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="da744-118">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="da744-119">az vm</span><span class="sxs-lookup"><span data-stu-id="da744-119">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="da744-120">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="da744-120">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="da744-121">az storage account</span><span class="sxs-lookup"><span data-stu-id="da744-121">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="da744-122">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="da744-122">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="da744-123">az keyvault</span><span class="sxs-lookup"><span data-stu-id="da744-123">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="da744-124">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="da744-124">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="da744-125">az webapp</span><span class="sxs-lookup"><span data-stu-id="da744-125">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="da744-126">Базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="da744-126">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="da744-127">az sql server</span><span class="sxs-lookup"><span data-stu-id="da744-127">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="da744-128">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="da744-128">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="da744-129">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="da744-129">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="da744-130">Поиск команд</span><span class="sxs-lookup"><span data-stu-id="da744-130">Finding commands</span></span>

<span data-ttu-id="da744-131">Команды CLI организованы в виде _групп_ _команд_.</span><span class="sxs-lookup"><span data-stu-id="da744-131">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="da744-132">Каждая группа представляет службу Azure, с которой работают эти команды.</span><span class="sxs-lookup"><span data-stu-id="da744-132">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="da744-133">Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="da744-133">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="da744-134">Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="da744-134">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="da744-135">Аргумент `--help` позволяет получить полный список команд и подгрупп в группе.</span><span class="sxs-lookup"><span data-stu-id="da744-135">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="da744-136">Например, вот как можно найти команды CLI для работы с группами безопасности сети (NSG):</span><span class="sxs-lookup"><span data-stu-id="da744-136">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="da744-137">В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.</span><span class="sxs-lookup"><span data-stu-id="da744-137">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="da744-138">Глобально доступные аргументы</span><span class="sxs-lookup"><span data-stu-id="da744-138">Globally available arguments</span></span>

<span data-ttu-id="da744-139">Для каждой команды есть ряд аргументов.</span><span class="sxs-lookup"><span data-stu-id="da744-139">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="da744-140">`--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.</span><span class="sxs-lookup"><span data-stu-id="da744-140">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="da744-141">`--output` изменяет формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="da744-141">`--output` changes the output format.</span></span> <span data-ttu-id="da744-142">Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции) и `table` (понятные таблицы ASCII).</span><span class="sxs-lookup"><span data-stu-id="da744-142">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="da744-143">По умолчанию CLI выводит формат `json`.</span><span class="sxs-lookup"><span data-stu-id="da744-143">By default the CLI outputs `json`.</span></span> <span data-ttu-id="da744-144">См. дополнительные сведения о [форматах выходных данных для Azure CLI 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="da744-144">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="da744-145">`--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure.</span><span class="sxs-lookup"><span data-stu-id="da744-145">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="da744-146">См. дополнительные сведения о [создании запросов о результатах команд в Azure CLI 2.0](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="da744-146">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="da744-147">`--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="da744-147">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="da744-148">`--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки.</span><span class="sxs-lookup"><span data-stu-id="da744-148">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="da744-149">Если вы обнаружили ошибку, включите выходные данные, полученные с помощью флага `--debug`, в отправляемый отчет об ошибке.</span><span class="sxs-lookup"><span data-stu-id="da744-149">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="da744-150">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="da744-150">Interactive mode</span></span>

<span data-ttu-id="da744-151">CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд.</span><span class="sxs-lookup"><span data-stu-id="da744-151">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="da744-152">Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="da744-152">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="da744-153">См. дополнительные сведения об [интерактивном режиме Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="da744-153">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="da744-154">Также доступно [расширение для Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), которое предлагает интерактивный интерфейс с функциями автозавершения и отображения документации при наведении курсора.</span><span class="sxs-lookup"><span data-stu-id="da744-154">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="da744-155">Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах</span><span class="sxs-lookup"><span data-stu-id="da744-155">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="da744-156">Чтобы приступить к работе с Azure CLI 2.0, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для запроса ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="da744-156">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="da744-157">Создание виртуальных машин с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="da744-157">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="da744-158">Также доступны краткие руководства по работе с другими популярными службами.</span><span class="sxs-lookup"><span data-stu-id="da744-158">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="da744-159">Создание учетной записи хранения с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="da744-159">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="da744-160">Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="da744-160">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="da744-161">Создание отдельной базы данных SQL Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="da744-161">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="da744-162">Создание базы данных Azure для сервера MySQL с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="da744-162">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="da744-163">[Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="da744-163">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="da744-164">Создание веб-приложения Python в Azure</span><span class="sxs-lookup"><span data-stu-id="da744-164">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="da744-165">Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров</span><span class="sxs-lookup"><span data-stu-id="da744-165">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="da744-166">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="da744-166">Give feedback</span></span>

<span data-ttu-id="da744-167">Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки.</span><span class="sxs-lookup"><span data-stu-id="da744-167">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="da744-168">Вы можете [опубликовать описание проблемы на Github](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="da744-168">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
