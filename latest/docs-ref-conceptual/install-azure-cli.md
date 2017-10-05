---
title: "Установка Azure CLI 2.0"
description: "Справочная документация по установке Azure CLI 2.0"
keywords: Azure CLI, Install Azure CLI, Azure Python CLI, Azure CLI Reference
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 935814d56d0a6be00f626da860dc643adbf14804
ms.sourcegitcommit: 9f38efbb7efd800ee5cab80d6641770d268c5a68
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2017
---
# <a name="install-azure-cli-20"></a>Установка Azure CLI 2.0

Установите новую версию интерфейса командной строки Azure прямо сейчас!
Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.
Его можно использовать в Windows, Linux и macOS.
Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).

> [!NOTE]
> Если вам нужна предыдущая версия Azure CLI, см. руководство по [установке Azure CLI 1.0](/azure/cli-install-nodejs).

## <a name="a-namemacosinstall-on-macos"></a><a name="macOS"/>Установка в macOS

В macOS установку можно выполнить с помощью [Homebrew](https://brew.sh/) или вручную.

### <a name="install-with-homebrew"></a>Установка с помощью Homebrew

1. Если у вас нет этой программы, выполните [инструкции по установке Homebrew](https://docs.brew.sh/Installation.html).

2. Если CLI устанавливался вручную, следуйте инструкциям по [удалению вручную](#UninstallManually).

3. Обновите свои локальные репозитории Homebrew.

   ```bash
   brew update
   ```

4. Установите пакет `azure-cli`.

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> Если вы ранее установили Azure CLI 1.0 с помощью Homebrew, вместо установки пакета можно получить CLI 2.0 при регулярном обновлении Homebrew.
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a>Установка вручную

1. Установите Azure CLI 2.0 с помощью команды `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.

   ```bash
   exec -l $SHELL
   ```
   
3. Запустите CLI из командной строки с помощью команды `az`.

## <a name="install-on-windows"></a>Установка в Windows

### <a name="install-with-msi-for-the-windows-command-line"></a>Установка с помощью MSI-файла для командной строки Windows 

Чтобы установить CLI в Windows и использовать его в окне командной строки Windows, скачайте и запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows).

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a>Установка с помощью apt-get для Bash на платформе Ubuntu в Windows

1. Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).

2. Откройте оболочку Bash.

3. Измените список источников.

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. Выполните следующие команды sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  Запустите CLI из командной строки с помощью команды `az`.

## <a name="install-on-debianubuntu-with-apt-get"></a>Установка на Debian или Ubuntu с помощью apt-get

В системах на базе Debian и Ubuntu можно установить Azure CLI 2.0 с помощью `apt-get`.

1. Измените список источников.
 
   - 32-разрядная система:

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - 64-разрядная система:

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Выполните следующие команды sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  Запустите CLI из командной строки с помощью команды `az`.

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a>Установка в RHEL, Fedora и CentOS с помощью yum

Для любого дистрибутива на базе RedHat, который содержит диспетчер пакетов `yum`, Azure CLI 2.0 можно установить с помощью `yum`.

1. Импортируйте ключ репозитория Майкрософт:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Создайте сведения о локальном репозитории `azure-cli`:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Обновите индекс пакета `yum` и выполните установку:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. Запустите CLI из командной строки с помощью команды `az`.

## <a name="install-on-opensuse-and-sle-with-zypper"></a>Установка в openSUSE и SLE с помощью zypper

1. Импортируйте ключ репозитория Майкрософт:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Создайте сведения о локальном репозитории `azure-cli`:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. Обновите индекс пакета `zypper` и выполните установку:

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. Запустите CLI из командной строки с помощью команды `az`.

## <a name="install-with-docker"></a>Установка с помощью Docker

Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI 2.0.

Установите CLI с помощью команды `docker run`.

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.

> [!NOTE]
> Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><a name="Linux"/>Установка в Linux без использования apt-get

Рекомендуется по возможности устанавливать CLI с помощью диспетчера пакетов (если вы знаете, как это сделать). Для дистрибутивов, для которых диспетчер пакетов не предоставляется, CLI можно установить вручную.

1. Установите необходимые компоненты с учетом дистрибутива Linux.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

Если дистрибутив не указан в списке выше, вам нужно установить [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) и [OpenSSL](https://www.openssl.org/source/).

2. Установите CLI с помощью команды `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.

   ```bash
   exec -l $SHELL
   ```

4. Запустите CLI из командной строки с помощью команды `az`.

## <a name="troubleshooting"></a>Устранение неполадок

Если при установке CLI возникла проблема, ознакомьтесь с этим разделом, чтобы найти описание своего случая. Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="curl-object-moved-error"></a>Ошибка "Объект перемещен" при выполнении команды curl

Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Команда `az` не найдена

Попробуйте очистить кэш хэша команд оболочки. Выполните это

```bash
hash -r
```

и посмотрите, будет ли устранена проблема.

## <a name="uninstall-cli-1x-versions"></a>Удаление версий CLI 1.x

Если в системе установлена более ранняя версия CLI 1.x, вы можете удалить ее с учетом примененного типа установки.

### <a name="uninstall-with-npm"></a>Удаление с помощью npm

Удалите устаревшую версию CLI с помощью команды `npm uninstall`.

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a>Удаление с помощью распространяемых компонентов

Если установка выполнялась с использованием [установщика Azure CLI (MSI)](http://aka.ms/webpi-azure-cli) или [пакета macOS](http://aka.ms/mac-azure-cli), используйте то же средство для удаления файлов установки.

### <a name="uninstall-with-docker"></a>Удаление с помощью Docker

Если вы установили образ Docker, чтобы использовать более раннюю версию CLI, удалите этот образ и все связанные контейнеры. Позже вы сможете повторно создать контейнеры, установив новый образ Docker, как описано в инструкциях по установке.

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a>Обновление интерфейса командной строки

Чтобы обновить Azure CLI, используйте тот же метод, что и для установки.

### <a name="update-with-homebrew"></a>Обновление с помощью Homebrew

1. Если установка выполнялась вручную, следуйте инструкциям по [установке с помощью Homebrew](#macOS).

2. Обновите свои данные в локальном репозитории Homebrew.

   ```bash
   brew update
   ```

3. Обновите установленные пакеты.

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a>Обновление с помощью MSI-файла

Запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows) еще раз.

### <a name="update-with-apt-get"></a>Обновление с помощью apt-get

Используйте `apt-get upgrade`, чтобы обновить пакет CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.
> Чтобы обновить только CLI, используйте команду `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a>Обновление с помощью Docker

1. Обновите локальный образ с помощью команды `docker pull`.

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. Получите данные о контейнерах, которые используют образ CLI.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.

3. Остановите и заново создайте контейнеры.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a>Обновление вручную

Следуйте инструкциям по установке вручную для обновления в [macOS](#macOS) или [Linux](#Linux).

## <a name="uninstall"></a>Удаление

Нам будет очень жаль, если вы решите удалить CLI. Чтобы удалить CLI, используйте тот же метод, что и для установки.

### <a name="uninstall-with-homebrew"></a>Удаление с помощью Homebrew

Удалите пакет `azure-cli`.

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a>Удаление с помощью MSI-файла

Запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".

### <a name="uninstall-with-apt-get"></a>Удаление с помощью apt-get

Выполните удаление с помощью `apt-get remove`.

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a>Удаление с помощью Docker

Если вы установили образ Docker, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.

1. Получите данные о контейнерах, на которых запущен образ azure-cli.

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. Удалите все контейнеры с образом CLI.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Удалите локально установленный образ CLI.

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><a name="UninstallManually"/>Удаление вручную

Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.

1. Удалите установленные файлы.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.

> [!Note]
> Расположение установки по умолчанию — `/Users/<username>`.

## <a name="report-cli-issues-and-feedback"></a>Создание отчетов о проблемах CLI и обратная связь

Если при работе со средством возникают ошибки, сообщите об этом в разделе репозитория GitHub, посвященном [проблемам](https://github.com/Azure/azure-cli/issues).
Чтобы отправить отзыв из командной строки, используйте команду `az feedback`.
