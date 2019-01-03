---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI в macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593172"
---
# <a name="install-azure-cli-on-macos"></a>Установка Azure CLI в macOS

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

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).

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

## <a name="other-installation-methods"></a>Другие методы установки

При невозможности использовать Homebrew для установки Azure CLI в своей среде можно воспользоваться инструкциями по ручной установке для Linux. Следует учесть, что этот процесс не является официально рекомендованным для macOS. Всегда предпочтительнее использовать менеджер пакетов, например Homebrew. Используйте метод ручной установки только при отсутствии других вариантов.

Инструкции по ручной установке Azure CLI в Linux см. в [соответствующей статье](install-azure-cli-linux.md).

## <a name="next-steps"></a>Дальнейшие действия

Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.

> [!div class="nextstepaction"]
> [Начало работы с Azure CLI](get-started-with-azure-cli.md)
