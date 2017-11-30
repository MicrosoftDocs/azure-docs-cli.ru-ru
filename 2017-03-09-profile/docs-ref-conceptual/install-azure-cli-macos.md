---
title: "Установка Azure CLI для macOS"
description: "Как установить Azure CLI 2.0 в macOS"
keywords: Azure CLI,Install Azure CLI,azure macos, azure install macos
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-on-macos"></a>Установка Azure CLI 2.0 в macOS

Для платформы macOS можно установить Azure CLI с помощью [диспетчера пакетов homebrew](http://brew.sh) или вручную. Использовать диспетчер пакетов homebrew предпочтительнее, так как это средство упрощает установку, обновление и удаление (при необходимости).

## <a name="use-homebrew-to-install"></a>Установка с помощью homebrew

Homebrew — это самый простой способ управления установкой CLI. Это удобное средство установки, обновления и удаления, как и другие аналогичные средства, включая `apt` или `yum`.
Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.

### <a name="install-with-homebrew"></a>Установка с помощью Homebrew

Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:

```bash
brew update && brew install azure-cli
```

Запустите Azure CLI с помощью команды `az`.

### <a name="update-with-homebrew"></a>Обновление с помощью homebrew

CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра. Новый выпуск выходит примерно раз в две недели. Вам нужно будет обновить сведения о локальном репозитории, а затем — обновить сам пакет CLI.

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a>Устранение неполадок

У вас возникли проблемы с установкой или обновлением CLI с помощью homebrew? Ниже описаны некоторые распространенные ошибки, а также способы их диагностики и устранения.

#### <a name="unable-to-find-python-or-installed-packages"></a>Не удается найти Python или установленные пакеты

Если при установке не удается найти Python или установленные пакеты, причина может быть в незначительном нессответствии номера версии или в проблеме с установкой homebrew. Так как CLI не использует virtualenv, важно, чтобы при установке с помощью homebrew была найдена правильная версия Python. Эти проблемы можно устранить, перенастроив установку Python:

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a>Версия CLI устарела

Если вы считаете, что установленная версия CLI могла устареть, последовательно выполните команды `brew update` и `brew upgrade azure-cli`. Если обновление CLI не произойдет, имейте в виду, что пакеты homebrew могут развертываться медленнее, чем общие выпуски. Если вам нужно установить самую последнюю версию CLI, выполните [установку вручную](#manage-the-cli-manually).

### <a name="uninstall-with-homebrew"></a>Удаление с помощью homebrew

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

Если установка выполнялась с помощью homebrew, это же средство следует использовать и для удаления.

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a>Установка CLI вручную

Если вы не можете или не хотите использовать homebrew, установить CLI можно вручную.

Выполните [инструкции по установке в Linux вручную](install-azure-cli-linux.md), чтобы установить CLI вручную в macOS. В macOS версии 10.9 и выше должны содержаться все необходимые зависимости.
