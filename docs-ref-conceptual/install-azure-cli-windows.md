---
title: "Установка Azure CLI для Windows"
description: "Как установить Azure CLI 2.0 в Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: df1c2b33589c160525710845cc81d076082a9ecc
ms.sourcegitcommit: def1a07bfccf26a4178ba6dd836764a1df205929
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Установка Azure CLI 2.0 в Windows

В Windows двоичный файл Azure CLI устанавливается с помощью установщика MSI, который предоставляет доступ к CLI через командную строку Windows (CMD) или PowerShell.
При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для вашего дистрибутива. Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).

## <a name="install-or-update"></a>Установка или обновление

Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)

Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".

Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell. PowerShell предоставляет несколько функций заполнения нажатием клавиши TAB, которые недоступны в CMD.

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)
