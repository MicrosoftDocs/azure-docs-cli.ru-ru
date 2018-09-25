---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI 2.0 в macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1dab4d6aece78999e9d97ac5c8e3598c55a8a55d
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2018
ms.locfileid: "46469935"
---
# <a name="install-azure-cli-20-on-macos"></a>Установка Azure CLI 2.0 в macOS

На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](https://brew.sh). Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии. Пакет CLI протестирован с macOS 10.9 и более поздних версий.

## <a name="install"></a>Install

Homebrew — это самый простой способ управления установкой CLI. Это удобное средство установки, обновления и удаления,
Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.

Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:

```bash
brew update && brew install azure-cli
```

Запустите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Не удается найти Python или установленные пакеты

Во время установки с помощью homebrew может наблюдаться несовпадение дополнительного номера версии или другая проблема. CLI не использует виртуальное окружение Python и попытается обнаружить установленную версию Python. Возможное решение — установить зависимость `python3` и повторно создать на нее ссылку из Homebrew.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>Установлена версия CLI 1.x

Если установлена старая версия, это может произойти из-за устаревания кэша homebrew. Следуйте инструкциям по [обновлению](#Update).

## <a name="update"></a>Блокировка изменений

CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра. Новый выпуск выходит примерно раз в две недели. Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Для удаления пакета `azure-cli` воспользуйтесь homebrew.

```bash
brew uninstall azure-cli
```

## <a name="next-steps"></a>Дальнейшие действия

Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.

> [!div class="nextstepaction"]
> [Начало работы с Azure CLI](get-started-with-azure-cli.md)
