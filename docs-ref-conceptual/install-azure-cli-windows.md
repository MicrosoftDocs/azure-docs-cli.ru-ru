---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI 2.0 в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 30bdb327601c7d898b5e64a3a472a104dc5db3b4
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388462"
---
# <a name="install-azure-cli-20-on-windows"></a>Установка Azure CLI 2.0 в Windows

Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.
При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux. Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).

## <a name="install-or-update"></a>Установка или обновление

Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)

Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".

Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell. В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows. Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".

> [!div class="nextstepaction"]
> [Скачать установщик MSI](https://aka.ms/installazurecliwindows)
