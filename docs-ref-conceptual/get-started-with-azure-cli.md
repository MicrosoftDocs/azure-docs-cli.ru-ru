---
title: Начало работы с Azure CLI
description: Начните работу с Azure CLI, изучив базовые команды.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: bc9b86db6fb9c5b3731550df9dda96debcbfba9f
ms.sourcegitcommit: 93d8137f37e974f7d314a0b1deb65ac563c2e2c5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "79990119"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="e5a23-103">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-103">Get started with Azure CLI</span></span>

<span data-ttu-id="e5a23-104">Добро пожаловать в Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="e5a23-104">Welcome to the Azure CLI!</span></span>  <span data-ttu-id="e5a23-105">В этой статье собрана информация об интерфейсе командной строки и выполнении стандартных задач.</span><span class="sxs-lookup"><span data-stu-id="e5a23-105">This article introduces the CLI and helps you complete common tasks.</span></span>

> [!NOTE]
>
> <span data-ttu-id="e5a23-106">В скриптах и на сайте документации Майкрософт примеры Azure CLI написаны для оболочки `bash`.</span><span class="sxs-lookup"><span data-stu-id="e5a23-106">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="e5a23-107">Однострочные примеры можно запускать на любой платформе.</span><span class="sxs-lookup"><span data-stu-id="e5a23-107">One-line examples will run on any platform.</span></span> <span data-ttu-id="e5a23-108">Более длинные примеры, включающие символы продолжения строки (`\`) или присвоение значения переменной, нужно изменить для использования в других оболочках, включая PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e5a23-108">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="e5a23-109">Установка или запуск в Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5a23-109">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="e5a23-110">Самый простой способ приступить к работе с Azure CLI —запустить CLI в среде Azure Cloud Shell через браузер.</span><span class="sxs-lookup"><span data-stu-id="e5a23-110">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="e5a23-111">Дополнительные сведения о Cloud Shell см. в [кратком руководстве по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="e5a23-111">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="e5a23-112">Сведения об установке CLI см. в разделе [Установка Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-112">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="e5a23-113">Установив CLI впервые, проверьте правильность установки и версии, выполнив команду `az --version`.</span><span class="sxs-lookup"><span data-stu-id="e5a23-113">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

> [!NOTE]
> <span data-ttu-id="e5a23-114">Если вы используете классическую модель развертывания Azure, [установите классический интерфейс командной строки Azure](install-classic-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-114">If you're using the Azure classic deployment model, [install the Azure classic CLI](install-classic-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="e5a23-115">Вход</span><span class="sxs-lookup"><span data-stu-id="e5a23-115">Sign in</span></span>

<span data-ttu-id="e5a23-116">Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="e5a23-116">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="e5a23-117">После входа в систему появится список подписок, связанных с учетной записью Azure.</span><span class="sxs-lookup"><span data-stu-id="e5a23-117">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="e5a23-118">В сведениях о подписке с `isDefault: true` указана текущая активная подписка, отображаемая после входа.</span><span class="sxs-lookup"><span data-stu-id="e5a23-118">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="e5a23-119">Чтобы выбрать другую подписку, укажите идентификатор подписки с помощью команды [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="e5a23-119">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="e5a23-120">См. дополнительные сведения о [выборе нужной подписки при использовании нескольких подписок Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-120">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="e5a23-121">Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-121">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="e5a23-122">Стандартные команды</span><span class="sxs-lookup"><span data-stu-id="e5a23-122">Common commands</span></span>

<span data-ttu-id="e5a23-123">В таблице приведены некоторые распространенные команды CLI и ссылки на справочную документацию.</span><span class="sxs-lookup"><span data-stu-id="e5a23-123">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="e5a23-124">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="e5a23-124">Resource type</span></span> | <span data-ttu-id="e5a23-125">Группа команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-125">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="e5a23-126">Группа ресурсов</span><span class="sxs-lookup"><span data-stu-id="e5a23-126">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="e5a23-127">az group</span><span class="sxs-lookup"><span data-stu-id="e5a23-127">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="e5a23-128">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="e5a23-128">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="e5a23-129">az vm</span><span class="sxs-lookup"><span data-stu-id="e5a23-129">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="e5a23-130">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="e5a23-130">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="e5a23-131">az storage account</span><span class="sxs-lookup"><span data-stu-id="e5a23-131">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="e5a23-132">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="e5a23-132">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="e5a23-133">az keyvault</span><span class="sxs-lookup"><span data-stu-id="e5a23-133">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="e5a23-134">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="e5a23-134">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="e5a23-135">az webapp</span><span class="sxs-lookup"><span data-stu-id="e5a23-135">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="e5a23-136">Базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="e5a23-136">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="e5a23-137">az sql server</span><span class="sxs-lookup"><span data-stu-id="e5a23-137">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="e5a23-138">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5a23-138">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="e5a23-139">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e5a23-139">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="e5a23-140">Поиск команд</span><span class="sxs-lookup"><span data-stu-id="e5a23-140">Finding commands</span></span>

<span data-ttu-id="e5a23-141">Команды CLI организованы в виде _групп_ _команд_.</span><span class="sxs-lookup"><span data-stu-id="e5a23-141">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="e5a23-142">Каждая группа представляет службу Azure, с которой работают эти команды.</span><span class="sxs-lookup"><span data-stu-id="e5a23-142">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="e5a23-143">Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="e5a23-143">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="e5a23-144">Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="e5a23-144">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="e5a23-145">Аргумент `--help` позволяет получить полный список команд и подгрупп в группе.</span><span class="sxs-lookup"><span data-stu-id="e5a23-145">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="e5a23-146">Например, вот как можно найти команды CLI для работы с группами безопасности сети (NSG):</span><span class="sxs-lookup"><span data-stu-id="e5a23-146">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="e5a23-147">В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.</span><span class="sxs-lookup"><span data-stu-id="e5a23-147">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="e5a23-148">Глобально доступные аргументы</span><span class="sxs-lookup"><span data-stu-id="e5a23-148">Globally available arguments</span></span>

<span data-ttu-id="e5a23-149">Для каждой команды есть ряд аргументов.</span><span class="sxs-lookup"><span data-stu-id="e5a23-149">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="e5a23-150">`--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.</span><span class="sxs-lookup"><span data-stu-id="e5a23-150">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="e5a23-151">`--output` изменяет формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="e5a23-151">`--output` changes the output format.</span></span> <span data-ttu-id="e5a23-152">Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции), `table` (понятные таблицы ASCII) и `yaml`.</span><span class="sxs-lookup"><span data-stu-id="e5a23-152">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="e5a23-153">По умолчанию CLI выводит формат `json`.</span><span class="sxs-lookup"><span data-stu-id="e5a23-153">By default the CLI outputs `json`.</span></span> <span data-ttu-id="e5a23-154">См. дополнительные сведения о [форматах выходных данных для Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-154">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="e5a23-155">`--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure.</span><span class="sxs-lookup"><span data-stu-id="e5a23-155">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="e5a23-156">См. дополнительные сведения о [создании запросов к результатам выполнения команд в Azure CLI](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="e5a23-156">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="e5a23-157">`--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.</span><span class="sxs-lookup"><span data-stu-id="e5a23-157">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="e5a23-158">`--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки.</span><span class="sxs-lookup"><span data-stu-id="e5a23-158">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="e5a23-159">Если вы обнаружили ошибку, включите выходные данные, полученные с помощью флага `--debug`, в отправляемый отчет об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e5a23-159">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="e5a23-160">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="e5a23-160">Interactive mode</span></span>

<span data-ttu-id="e5a23-161">CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд.</span><span class="sxs-lookup"><span data-stu-id="e5a23-161">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="e5a23-162">Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).</span><span class="sxs-lookup"><span data-stu-id="e5a23-162">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="e5a23-163">См. дополнительные сведения об [интерактивном режиме Azure CLI](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5a23-163">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="e5a23-164">Также доступно [расширение для Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), которое предлагает интерактивный интерфейс с функциями автозавершения и отображения документации при наведении курсора.</span><span class="sxs-lookup"><span data-stu-id="e5a23-164">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="e5a23-165">Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах</span><span class="sxs-lookup"><span data-stu-id="e5a23-165">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="e5a23-166">Чтобы приступить к работе с Azure CLI, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для выполнения запросов к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="e5a23-166">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="e5a23-167">Руководство по созданию виртуальных машин с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-167">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="e5a23-168">Также доступны краткие руководства по работе с другими популярными службами.</span><span class="sxs-lookup"><span data-stu-id="e5a23-168">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="e5a23-169">Создание учетной записи хранения с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-169">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [<span data-ttu-id="e5a23-170">Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-170">Transfer objects to/from Azure Blob storage using the CLI</span></span>](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [<span data-ttu-id="e5a23-171">Создание отдельной базы данных SQL Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-171">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="e5a23-172">Создание базы данных Azure для сервера MySQL с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-172">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* <span data-ttu-id="e5a23-173">[Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="e5a23-173">[Create an Azure Database for PostgreSQL using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)</span></span>
* [<span data-ttu-id="e5a23-174">Создание веб-приложения Python в Azure</span><span class="sxs-lookup"><span data-stu-id="e5a23-174">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="e5a23-175">Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров</span><span class="sxs-lookup"><span data-stu-id="e5a23-175">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="e5a23-176">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="e5a23-176">Give feedback</span></span>

<span data-ttu-id="e5a23-177">Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки.</span><span class="sxs-lookup"><span data-stu-id="e5a23-177">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="e5a23-178">Вы можете [опубликовать описание проблемы на GitHub](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).</span><span class="sxs-lookup"><span data-stu-id="e5a23-178">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

## <a name="see-also"></a><span data-ttu-id="e5a23-179">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="e5a23-179">See also</span></span>

* [<span data-ttu-id="e5a23-180">Службы, которыми можно управлять с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-180">Services the Azure CLI can manage</span></span>](azure-services-the-azure-cli-can-manage.md)
* [<span data-ttu-id="e5a23-181">Полный список справочников по командам Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-181">Full command reference list for the Azure CLI</span></span>](/cli/azure/reference-index)
* [<span data-ttu-id="e5a23-182">Популярные статьи по использованию Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e5a23-182">Popular articles on using the Azure CLI</span></span>](popular-articles-using-the-azure-cli.md)
