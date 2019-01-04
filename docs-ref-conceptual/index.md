---
title: Общие сведения об Azure CLI
description: Общие сведения об интерфейсе командной строки Azure (CLI).
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 285567b00d8c303af3e78a01dc80946a08e4e8f8
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805913"
---
# <a name="azure-command-line-interface-cli"></a>Интерфейс командной строки Azure (CLI)

Azure CLI — это кроссплатформенный интерфейс командной строки от Майкрософт для управления ресурсами Azure.
Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.

Начать работу с Azure CLI очень просто. Этот инструмент лучше всего подходит для создания скриптов автоматизации, которые работают с Azure Resource Manager.
С помощью Azure CLI можно легко создавать виртуальные машины в Azure простым вводом следующей команды:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> В скриптах и на сайте документации Майкрософт примеры Azure CLI написаны для оболочки `bash`. Однострочные примеры можно запускать на любой платформе. Более длинные примеры, включающие символы продолжения строки (`\`) или присвоение значения переменной, нужно изменить для использования в других оболочках, включая PowerShell.

## <a name="run-or-install"></a>Запуск или установка

CLI можно установить локально, запустить в контейнере Docker или браузере с помощью Azure Cloud Shell.

* Сведения о запуске Azure Cloud Shell в браузере см. в статье [Краткое руководство по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart) или [Краткое руководство по использованию PowerShell в Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Сведения об установке CLI см. в статье [Установка Azure CLI 2.0](install-azure-cli.md).
* Сведения о запуске в контейнере Docker см. в статье [Запуск Azure CLI в контейнере Docker](run-azure-cli-docker.md).

## <a name="build-your-skills-with-microsoft-learn"></a>Развитие навыков с помощью Microsoft Learn

- [Управление виртуальными машинами с помощью Azure CLI](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [Управление службами Azure с помощью CLI](/learn/modules/control-azure-services-with-cli/)
- [Другие интерактивные руководства](/learn/browse/?products=azure-clis)

## <a name="get-started"></a>Начало работы

Основные сведения о CLI см. в статье о [начале работы](get-started-with-azure-cli.md). В следующих примерах показаны некоторые из распространенных вариантов использования:

- [Виртуальные машины Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Виртуальные машины Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Веб-приложения](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [База данных SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI.

> [!NOTE]
> Если вы используете предыдущую версию интерфейса командной строки (классический интерфейс командной строки Azure), вы можете продолжать использовать ее.
> Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI.
> Если вы используете обе версии CLI, следует помнить, что команда `azure` вызывает классический интерфейс командной строки, а `az` — последнюю версию CLI.
