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
ms.openlocfilehash: f45c3acfdb4edb82cde755472d240ae18d82aba2
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967747"
---
# <a name="get-started-with-azure-cli-20"></a>Начало работы с Azure CLI 2.0

Добро пожаловать в Azure CLI 2.0! CLI — это средство, предназначенное для быстрой и эффективной работы со службами Azure с возможностью автоматизации. В этой статье рассматриваются возможности CLI и приводятся ссылки на связанные ресурсы.

## <a name="install-and-sign-in"></a>Установка и вход

Вы можете [установить CLI](install-azure-cli.md) или попробовать поработать с [Azure Cloud Shell](/azure/cloud-shell/overview).

Прежде чем использовать команды CLI при локальной установке, необходимо войти с помощью команды [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Вы также можете войти в автономном режиме, как описано в руководстве по [входу с помощью Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="common-commands"></a>Стандартные команды

В этой таблице перечислены некоторые распространенные команды, которые описаны в соответствующей справочной документации (см. ссылки).
Описание всех подкоманд и связанную документацию можно просмотреть в электронных справочниках или получить с помощью аргумента `--help`.

| Тип ресурса | Группа команд Azure CLI |
|---------------|-------------------------|
| [Группа ресурсов](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Виртуальные машины](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Учетные записи хранения](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [хранилище ключей;](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Веб-приложения](/azure/app-service) | [az webapp](/cli/azure/webapp) |
| [Базы данных SQL](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [Cosmos DB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Поиск команд

Команды в CLI представлены в виде _подкоманд_, входящих в _группы_.
Каждая группа представляет службу, предоставляемую Azure, а подгруппы позволяют распределить команды для этих служб в логические группы.

Чтобы найти команды, используйте команду [az find](/cli/azure/reference-index#az-find). Например, чтобы найти команды, содержащие `secret`, используйте следующую команду:

```azurecli-interactive
az find -q secret
```

Если вы знаете, с какой группой команд вы хотите работать, используйте аргумент `--help`. Она выводит не только подробные сведения о команде, но (при использовании с группой) отображает все доступные подкоманды. Например, при работе с группами безопасности сети (NSG) можно найти доступные подгруппы и команды, связанные с NSG.

```azurecli-interactive
az network nsg --help
```

В CLI доступна функция заполнения нажатием клавиши TAB для команд в оболочке Bash.

## <a name="globally-available-arguments"></a>Глобально доступные аргументы

Для каждой команды есть ряд аргументов.

* `--help` выводит справочные сведения CLI о командах и их аргументах, а также перечисляет доступные подгруппы и команды.
* `--output` изменяет формат выходных данных. Доступные выходные форматы: `json`, `jsonc` (выделенные цветом данные JSON), `tsv` (значения с разделением знаками табуляции) и `table` (понятные таблицы ASCII). По умолчанию CLI выводит формат `json`. См. дополнительные сведения о [форматах выходных данных для Azure CLI 2.0](format-output-azure-cli.md).
* `--query` использует [язык запросов JMESPath](http://jmespath.org/) для фильтрации результатов, возвращенных от служб Azure. См. дополнительные сведения о [создании запросов о результатах команд в Azure CLI 2.0](query-azure-cli.md) и [работе с JMESPath](http://jmespath.org/tutorial.html).
* `--verbose` выводит сведения о ресурсах, созданных в Azure во время выполнения операции, а также другую полезную информацию.
* `--debug` выводит дополнительные сведения об операциях CLI, выполняемых для отладки. Если вы обнаружили ошибку, включите выходные данные с помощью флага `--debug` в отправляемый отчет об ошибке.

## <a name="interactive-mode"></a>Интерактивный режим

CLI можно использовать в интерактивном режиме для автоматического отображения справочных сведений и упрощения выбора подкоманд. Перейти в интерактивный режим можно с помощью команды [az interactive](/cli/azure/reference-index#az-interactive).

```azurecli-interactive
az interactive
```

См. дополнительные сведения об [интерактивном режиме Azure CLI 2.0](interactive-azure-cli.md).

Кроме того, доступен [подключаемый модуль Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), который предусматривает интерактивное взаимодействие для получения документации с помощью автозаполнения и указателя.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Дополнительные сведения о CLI, представляемые в кратких и подробных руководствах

Чтобы приступить к работе с Azure CLI 2.0, ознакомьтесь с подробным руководством по настройке виртуальных машин и использовании функций CLI для запроса ресурсов Azure.

> [!div class="nextstepaction"]
> [Создание виртуальных машин с помощью Azure CLI 2.0](azure-cli-vm-tutorial.yml)

Если вы хотите сосредоточиться на других службах, доступен ряд кратких руководств для соответствующих решений с поддержкой CLI.

* [Создание учетной записи хранения с помощью Azure CLI](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Передача объектов в хранилище BLOB-объектов Azure и обратно с помощью CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)
* [Создание отдельной базы данных SQL Azure с помощью Azure CLI](/azure/sql-database/sql-database-get-started-cli)
* [Создание базы данных Azure для сервера MySQL с помощью Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Create an Azure Database for PostgreSQL by using the Azure CLI](/azure/postgresql/quickstart-create-server-database-azure-cli) (Создание базы данных Azure для PostgreSQL с помощью Azure CLI)
* [Создание веб-приложения Python в Azure](/azure/app-service/app-service-web-get-started-python)
* [Использование пользовательского образа Docker Hub для Веб-приложений Azure для контейнеров](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Обратная связь

Мы рады вашим отзывам о CLI, которые помогают нам улучшать наш продукт и устранять ошибки. Вы можете [опубликовать описание проблемы на Github](https://github.com/azure/azure-cli/issues) или использовать встроенные функции CLI, чтобы оставить отзыв с помощью команды [az feedback](/cli/azure/reference-index#az-feedback).

```azurecli-interactive
az feedback
```
