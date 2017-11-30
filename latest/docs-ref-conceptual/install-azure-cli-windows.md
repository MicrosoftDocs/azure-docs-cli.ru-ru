---
title: "Установка Azure CLI для Windows"
description: "Как установить Azure CLI 2.0 в Windows"
keywords: Azure CLI,Install Azure CLI,azure install windows, azure cli windows, azure windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 96a123575226f281accf125cb5bb29ee7d14ef2a
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-windows"></a>Установка Azure CLI 2.0 в Windows

В Windows вы можете установить собственный двоичный файл из MSI-файла, который затем можно использовать с помощью командной строки Windows и PowerShell. При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для используемого вами дистрибутива. Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).

## <a name="install-or-update-with-msi"></a>Установка или обновление с помощью MSI-файла

Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows. Вы можете [скачать установщик MSI](https://aka.ms/InstallAzureCliWindows) и запустить его для установки или обновления.

Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".

Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.

## <a name="uninstall-with-msi"></a>Удаление с помощью MSI-файла

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить". Вы можете [скачать установщик MSI](https://aka.ms/InstallAzureCliWindows), если у вас его нет.
