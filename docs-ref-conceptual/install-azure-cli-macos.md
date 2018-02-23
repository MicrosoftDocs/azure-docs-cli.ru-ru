---
title: "Установка Azure CLI для macOS"
description: "Как установить Azure CLI 2.0 в macOS"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0295846abc2fe6091940824c6efc47b8fd64ce9f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-macos"></a>Установка Azure CLI 2.0 в macOS

На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](http://brew.sh). Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии. Пакет CLI протестирован с macOS 10.9 и более поздних версий.

## <a name="install"></a>Install

Homebrew — это самый простой способ управления установкой CLI. Это удобное средство установки, обновления и удаления,
Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.

Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:

```bash
brew update && brew install azure-cli
```

Запустите Azure CLI с помощью команды `az`.

## <a name="troubleshooting"></a>Устранение неполадок

Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок. Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Не удается найти Python или установленные пакеты

Если при установке не удается найти Python или установленные пакеты, причина может быть в незначительном несоответствии номера версии или в проблеме с установкой homebrew. Так как для CLI не используется виртуальное окружение Python, важно, чтобы была найдена правильная версия Python. Эти проблемы можно устранить, перенастроив установку Python.

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>Установлена версия CLI 1.x

Если установлена устаревшая версия, возможно, причиной является устаревший кэш homebrew. Следуйте инструкциям по [обновлению](#Update).

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
