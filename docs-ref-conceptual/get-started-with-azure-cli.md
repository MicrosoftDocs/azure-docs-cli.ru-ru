---
title: Начало работы с Azure CLI 2.0
description: Начните работу с Azure CLI 2.0, изучив базовые команды.
keywords: Azure CLI, CLI help, Azure help, query, automation,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dbb6233e8fed15b440282b8396d3b3bd056e80f7
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512943"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="367ac-104">Начало работы с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="367ac-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="367ac-105">Добро пожаловать в Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="367ac-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="367ac-106">CLI — это средство, предназначенное для быстрой и эффективной работы со службами Azure с возможностью автоматизации.</span><span class="sxs-lookup"><span data-stu-id="367ac-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="367ac-107">В этой статье рассматриваются возможности CLI и приводятся ссылки на связанные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="367ac-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-log-in"></a><span data-ttu-id="367ac-108">Установка и вход</span><span class="sxs-lookup"><span data-stu-id="367ac-108">Install and log in</span></span>

<span data-ttu-id="367ac-109">Вы можете [установить CLI](install-azure-cli.md) или попробовать поработать с [Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="367ac-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="367ac-110">Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="367ac-110">Before using any CLI commands with a local install, you need to log in with [az login](/cli/azure/reference-index#az-login).</span></span>

```azurecli
az login
```

<span data-ttu-id="367ac-111">Эта команда выводит приглашение на вход с использованием кода аутентификации через веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="367ac-111">This command prompts you to log in with an authentication code via a website.</span></span> <span data-ttu-id="367ac-112">Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="367ac-112">There are ways to log in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="367ac-113">Стандартные команды</span><span class="sxs-lookup"><span data-stu-id="367ac-113">Common commands</span></span>

<span data-ttu-id="367ac-114">В этой таблице перечислены некоторые распространенные команды, которые описаны в соответствующей справочной документации (см. ссылки).</span><span class="sxs-lookup"><span data-stu-id="367ac-114">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="367ac-115">Описание всех подкоманд и связанную документацию можно просмотреть в электронных справочниках или получить с помощью аргумента `--help`.</span><span class="sxs-lookup"><span data-stu-id="367ac-115">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="367ac-116">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="367ac-116">Resource type</span></span> | <span data-ttu-id="367ac-117">Группа команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="367ac-117">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="367ac-118">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="367ac-118">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="367ac-119">az group</span><span class="sxs-lookup"><span data-stu-id="367ac-119">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="367ac-120">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="367ac-120">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="367ac-121">az vm</span><span class="sxs-lookup"><span data-stu-id="367ac-121">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="367ac-122">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="367ac-122">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="367ac-123">az storage account</span><span class="sxs-lookup"><span data-stu-id="367ac-123">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="367ac-124">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="367ac-124">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="367ac-125">az keyvault</span><span class="sxs-lookup"><span data-stu-id="367ac-125">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="367ac-126">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="367ac-126">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="367ac-127">az webapp</span><span class="sxs-lookup"><span data-stu-id="367ac-127">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="367ac-128">Базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="367ac-128">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="367ac-129">az sql server</span><span class="sxs-lookup"><span data-stu-id="367ac-129">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="367ac-130">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="367ac-130">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="367ac-131">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="367ac-131">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="367ac-132">Поиск команд</span><span class="sxs-lookup"><span data-stu-id="367ac-132">Finding commands</span></span>

<span data-ttu-id="367ac-133">Команды в CLI представлены в виде _подкоманд_, входящих в _группы_.</span><span class="sxs-lookup"><span data-stu-id="367ac-133">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="367ac-134">Каждая группа представляет службу, предоставляемую Azure, а подгруппы позволяют распределить команды для этих служб в логические группы.</span><span class="sxs-lookup"><span data-stu-id="367ac-134">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="367ac-135">Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="367ac-135">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="367ac-136">Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="367ac-136">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="367ac-137">Если вы знаете, с какой группой команд вы хотите работать, используйте аргумент `--help`.</span><span class="sxs-lookup"><span data-stu-id="367ac-137">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="367ac-138">Она выводит не только подробные сведения о команде, но (при использовании с группой) отображает все доступные подкоманды.</span><span class="sxs-lookup"><span data-stu-id="367ac-138">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="367ac-139">Например, при работе с группами безопасности сети (NSG) можно найти доступные подгруппы и команды, связанные с NSG.</span><span class="sxs-lookup"><span data-stu-id="367ac-139">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="367ac-140">В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.</span><span class="sxs-lookup"><span data-stu-id="367ac-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="367ac-141">Глобально доступные аргументы</span><span class="sxs-lookup"><span data-stu-id="367ac-141">Globally available arguments</span></span>

<span data-ttu-id="367ac-142">Для каждой команды есть ряд аргументов.</span><span class="sxs-lookup"><span data-stu-id="367ac-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="367ac-143">`--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.</span><span class="sxs-lookup"><span data-stu-id="367ac-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="367ac-144">`--output` изменяет формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="367ac-144">`--output` changes the output format.</span></span> <span data-ttu-id="367ac-145">Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции) и `table` (понятные таблицы ASCII).</span><span class="sxs-lookup"><span data-stu-id="367ac-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="367ac-146">По умолчанию CLI выводит формат `json`.</span><span class="sxs-lookup"><span data-stu-id="367ac-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="367ac-147">См. дополнительные сведения о [форматах выходных данных для Azure CLI 2.0](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="367ac-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="367ac-148">`--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure.</span><span class="sxs-lookup"><span data-stu-id="367ac-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="367ac-149">См. дополнительные сведения о [создании запросов о результатах команд в Azure CLI 2.0](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="367ac-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="367ac-150">`--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="367ac-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="367ac-151">`--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки.</span><span class="sxs-lookup"><span data-stu-id="367ac-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="367ac-152">Если вы обнаружили ошибку, включите выходные данные с помощью флага `--debug` в отправляемый отчет об ошибке.</span><span class="sxs-lookup"><span data-stu-id="367ac-152">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="367ac-153">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="367ac-153">Interactive mode</span></span>

<span data-ttu-id="367ac-154">CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд.</span><span class="sxs-lookup"><span data-stu-id="367ac-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="367ac-155">Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="367ac-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="367ac-156">См. дополнительные сведения об [интерактивном режиме Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="367ac-156">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="367ac-157">Кроме того, доступен [подключаемый модуль Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), который предусматривает интерактивное взаимодействие для получения документации с помощью автозаполнения и указателя.</span><span class="sxs-lookup"><span data-stu-id="367ac-157">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="367ac-158">Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах</span><span class="sxs-lookup"><span data-stu-id="367ac-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="367ac-159">Чтобы приступить к работе с Azure CLI 2.0, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для запроса ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="367ac-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="367ac-160">Создание виртуальных машин с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="367ac-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="367ac-161">Если вы хотите сосредоточиться на других службах, доступен ряд кратких руководств для соответствующих решений с поддержкой CLI.</span><span class="sxs-lookup"><span data-stu-id="367ac-161">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="367ac-162">Создание учетной записи хранения с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="367ac-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="367ac-163">Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="367ac-163">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="367ac-164">Создание отдельной базы данных SQL Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="367ac-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="367ac-165">Создание базы данных Azure для сервера MySQL с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="367ac-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="367ac-166">[Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="367ac-166">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="367ac-167">Создание веб-приложения Python в Azure</span><span class="sxs-lookup"><span data-stu-id="367ac-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="367ac-168">Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров</span><span class="sxs-lookup"><span data-stu-id="367ac-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="367ac-169">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="367ac-169">Give feedback</span></span>

<span data-ttu-id="367ac-170">Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки.</span><span class="sxs-lookup"><span data-stu-id="367ac-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="367ac-171">Вы можете [опубликовать описание проблемы на Github](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="367ac-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```
