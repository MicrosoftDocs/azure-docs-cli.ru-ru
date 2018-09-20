---
title: Общие сведения об Azure CLI 2.0
description: Общие сведения об Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388394"
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 — это кроссплатформенный интерфейс командной строки от Майкрософт для управления ресурсами Azure.
Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.

Начать работу с Azure CLI 2.0 очень просто. Этот инструмент лучше всего подходит для создания скриптов автоматизации, которые работают с Azure Resource Manager. С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Запуск или установка

CLI можно установить локально, запустить в контейнере Docker или браузере с помощью Azure Cloud Shell.

* Сведения о запуске Azure Cloud Shell в браузере см. в статье [Краткое руководство по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart) или [Краткое руководство по использованию PowerShell в Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Сведения об установке CLI см. в статье [Установка Azure CLI 2.0](install-azure-cli.md).
* Сведения о запуске в контейнере Docker см. в статье [Запуск Azure CLI 2.0 в контейнере Docker](run-azure-cli-docker.md).

## <a name="get-started"></a>Начало работы

Основные сведения о CLI см. в статье о [начале работы](get-started-with-azure-cli.md). В следующих примерах показаны некоторые из распространенных вариантов использования:

- [Виртуальные машины Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Виртуальные машины Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Веб-приложения](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [База данных SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI 2.0.

> [!NOTE]
> Если вы используете предыдущую версию интерфейса командной строки (Azure CLI 1.0), вы можете продолжать использовать ее.
> Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI 2.0.
> При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0.
