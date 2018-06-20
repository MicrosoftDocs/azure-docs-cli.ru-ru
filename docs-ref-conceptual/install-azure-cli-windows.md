---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI 2.0 в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c3ed3585b601ee55b267ea6cfc43ce41c54f084a
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2018
ms.locfileid: "33815982"
---
# <a name="install-azure-cli-20-on-windows"></a>Установка Azure CLI 2.0 в Windows

В Windows двоичный файл Azure CLI устанавливается с помощью установщика MSI, который предоставляет доступ к CLI через командную строку Windows (CMD) или PowerShell.
При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для вашего дистрибутива. Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).

## <a name="install-or-update"></a>Установка или обновление

Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)

Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".

Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell. В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows. Для входа выполните команду `az login`.

```azurecli
az login
```

Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)
