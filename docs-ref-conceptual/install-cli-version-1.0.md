---
title: Установка Azure CLI 1.0
description: Установка Azure CLI 1.0 на компьютерах Mac OS, Linux и Windows и начало работы со службами Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5f185e02217d6a3b54a9c252825c0f3fed3ab09e
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967679"
---
# <a name="install-the-azure-cli-10"></a>Установка Azure CLI 1.0

> [!IMPORTANT]
> В этом разделе описана установка Azure CLI 1.0. Это нерекомендуемый CLI, и его можно использовать только для поддержки с моделью управления службами Azure (ASM) с "классическими" ресурсами.
> Для развертываний Azure Resource Manager используйте [Azure CLI 2.0](/cli/azure).

Вы можете выполнить быструю установку интерфейса командной строки Azure (Azure CLI 1.0), чтобы использовать набор консольных команд с открытым кодом для управления ресурсами в среде Microsoft Azure. Существует несколько вариантов установки этих кроссплатформенных инструментов на компьютер.

* **Пакет npm**. Запустите npm (диспетчер пакетов для JavaScript), чтобы установить последнюю версию пакета для Azure CLI 1.0 в дистрибутиве или ОС Linux. На компьютере должны быть установлены node.js и npm.
* **Установщик**. Скачайте установщик, чтобы легко установить эти инструменты на компьютеры Mac или Windows.
* **Контейнер Docker**. Приступите к использованию последней версии интерфейса командной строки из готового контейнера Docker. На компьютере требуется наличие узла Docker.

Дополнительные сведения и варианты установки см. в репозитории проектов на сайте [GitHub](https://github.com/azure/azure-xplat-cli).

После установки Azure CLI 1.0 вы сможете [подключить его к своей подписке Azure](/cli/azure/authenticate-azure-cli) и работать с ресурсами Azure c помощью команд **azure** из интерфейса командной строки (Bash, терминала, командной строки и т. д.).

## <a name="option-1-install-an-npm-package"></a>Вариант 1. Установка пакета npm

Для установки интерфейса командной строки из пакета NPM в системе должна быть установлена [последняя версия Node.js и npm](https://nodejs.org/en/download/package-manager/). Затем запустите **npm install** для установки пакета azure-cli:

```bash
npm install -g azure-cli
```

В системах Linux для выполнения команды **npm** может потребоваться команда **sudo**:

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Если необходимо установить или обновить Node.js и npm в дистрибутиве или ОС Linux, рекомендуется установить последнюю версию Node.js LTS (4.x). Если вы используете более раннюю версию, возможны ошибки при установке.

Если хотите, скачайте последнюю версию [TAR-файла][linux-installer] пакета npm для Linux на локальный компьютер. Затем установите скачанный пакет npm, как описано ниже (для дистрибутивов Linux может потребоваться использовать **sudo**).

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Вариант 2. Использование установщика

При использовании компьютера Windows или Mac можно скачать следующие установщики интерфейса командной строки:

* [Установщик Mac OS X][mac-installer]
* [MSI-файл Windows][windows-installer]

> [!TIP]
> В Windows для установки интерфейса командной строки можно также скачать [установщик веб-платформы](https://go.microsoft.com/?linkid=9828653) . Этот установщик дает возможность установить дополнительный пакет SDK для Azure и программы командной строки после установки интерфейса командной строки.

## <a name="option-3-use-a-docker-container"></a>Вариант 3. Использование контейнера Docker

Если вы настроили компьютер в качестве узла [Docker](https://docs.docker.com/engine/understanding-docker/), то можете запустить последнюю версию Azure CLI 1.0 в контейнере Docker. Выполните следующую команду (в системах Linux для выполнения команды npm может потребоваться команда **sudo**):

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a>Выполнение команд Azure CLI 1.0

После установки Azure CLI 1.0 команду **azure** можно выполнить в любом пользовательском интерфейсе командной строки (Bash, терминале, командной строке и т. д.). Например, чтобы выполнить команду справки, введите следующее:

```azurecli
azure help
```

> [!NOTE]
> Для некоторых дистрибутивов Linux может появиться сообщение об ошибке `/usr/bin/env: ‘node’: No such file or directory`. Это связано с тем, что новые установки Node.js размещаются в папке /usr/bin/nodejs. Для устранения этой ошибки создайте символьную ссылку /usr/bin/node, выполнив следующую команду:

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Чтобы просмотреть версию установленного интерфейса Azure CLI 1.0, введите следующую команду.

```azurecli
azure --version
```

Теперь все готово к работе. Чтобы получить доступ ко всем командам интерфейса командной строки для работы с ресурсами, [подключитесь к подписке Azure из интерфейса командной строки Azure](/cli/azure/authenticate-azure-cli).

> [!NOTE]
> При первом использовании Azure CLI появится сообщение с вопросом, следует ли разрешить корпорации Майкрософт собирать сведения об использовании. Участие является добровольным. Если вы согласились участвовать в этой программе, сбор сведений можно остановить в любой момент, выполнив команду `azure telemetry --disable`. Чтобы включить участие в любой момент, выполните команду `azure telemetry --enable`.

## <a name="update-the-cli"></a>Обновление интерфейса командной строки

Корпорация Майкрософт часто выпускает обновленные версии Azure CLI. Переустановите интерфейс командной строки с помощью установщика для соответствующей операционной системы или запустите актуальную версию контейнера Docker. Если вы установили последние версии Node.js и NPM, введите следующую команду (в системах Linux может потребоваться использовать режим **sudo**).

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Включение выполнения нажатием клавиши TAB

Выполнение команд интерфейса командной строки нажатием клавиши TAB поддерживается на компьютерах MAC и Linux.

Чтобы включить эту функцию в zsh, выполните следующую команду:

```bash
echo '. <(azure --completion)' >> .zshrc
```

Чтобы включить эту функцию в bash, выполните следующую команду:

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a>Дополнительная информация

* [Подключитесь к подписке Azure из интерфейса командной строки](/cli/azure/authenticate-azure-cli) для создания ресурсов Azure и управления ими.
* Для того чтобы получить дополнительные сведения об интерфейсе командной строки Azure, скачать исходный код, сообщить о проблемах или принять участие в проекте, зайдите в [репозиторий GitHub для интерфейса командной строки Azure](https://github.com/azure/azure-xplat-cli).
* Если у вас возникли вопросы об использовании интерфейса командной строки Azure или платформы Azure, посетите [форумы Azure](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).

[mac-installer]: http://aka.ms/mac-azure-cli
[windows-installer]: http://aka.ms/webpi-azure-cli
[linux-installer]: http://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md
