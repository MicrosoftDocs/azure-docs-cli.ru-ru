---
title: "Установка Azure CLI 2.0"
description: "Справочная документация по Azure CLI 2.0"
keywords: "Azure CLI 2.0, справочник по Azure CLI 2.0, установка Azure CLI 2.0, Azure Python CLI, удаление Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a>Установка Azure CLI 2.0

Установите новую версию интерфейса командной строки Azure прямо сейчас!
Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.
Его можно использовать в Windows, Linux и macOS.
Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).

> [!NOTE]
> Если вам нужна предыдущая версия Azure CLI, см. статью [Установка Azure CLI 1.0](/azure/cli-install-nodejs).

## <a name="macos"></a>macOS

1. Azure CLI 2.0 можно установить с помощью одной команды `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.

   ```bash
   exec -l $SHELL
   ```
   
3. Запустите Azure CLI 2.0 из командной строки с помощью команды `az`.

> [!Note]
> При установке с помощью InstallAzureCli `az component update` не поддерживается.
> Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.
> 
> Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).

## <a name="windows"></a>Windows

Интерфейс командной строки можно установить с помощью MSI-файла и использовать его в командной строке Windows или установить его на платформе Ubuntu в Windows с помощью apt-get для Bash.

### <a name="msi-for-the-windows-command-line"></a>MSI-файл для командной строки Windows 

Чтобы установить интерфейс командной строки в Windows и использовать его в окне командной строке Windows, скачайте и запустите соответствующий [MSI](https://aka.ms/InstallAzureCliWindows)-файл.

> [!NOTE]
> При установке с помощью MSI-файла `az component` не поддерживается.
> Для обновления до последней версии интерфейса командной строки запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз.
> 
> Чтобы удалить интерфейс командной строки, запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a>apt-get для Bash на платформе Ubuntu в Windows

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

> [!NOTE]
> При установке с помощью apt-get `az component` не поддерживается.
> Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.
> 
> Для удаления выполните команду `sudo apt-get remove azure-cli`.

## <a name="linux"></a>Linux

1. В Linux может потребоваться установить определенные [необходимые компоненты](#linux-prerequisites).

2. Azure CLI 2.0 можно установить с помощью одной команды `curl`.

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.

   ```bash
   exec -l $SHELL
   ```

4. Запустите Azure CLI 2.0 из командной строки с помощью команды `az`.

> [!Note]
> При установке с помощью InstallAzureCli `az component update` не поддерживается.
> Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.
> 
> Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).

## <a name="docker"></a>Docker

Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI.

Установите Azure CLI с помощью `docker run`.

```bash
docker run azuresdk/azure-cli-python:<version>
```

См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).

> [!NOTE]
> Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> Образ Docker не поддерживает [ функцию `component`](/cli/azure/component).
> Чтобы обновить Azure CLI 2.0, используйте `docker run` для установки последней версии образа или выбранного вами определенного образа.

## <a name="apt-get"></a>apt-get

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

> [!NOTE]
> При установке с помощью apt-get `az component` не поддерживается.
> Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.
> 
> Для удаления выполните команду `sudo apt-get remove azure-cli`.

## <a name="linux-prerequisites"></a>Предварительные требования для Linux

1. Если у вас не установлен язык [Python](https://www.python.org/downloads), установите его.

2. В зависимости от дистрибутива Linux установите необходимые компоненты.

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

## <a name="troubleshooting"></a>Устранение неполадок

### <a name="errors-with-curl-redirection"></a>Ошибки, связанные с перенаправлением curl

Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса aka.ms:

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a>Удаление

Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.

1. Удалите установленные файлы.

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.

> [!Note]
> Расположение установки по умолчанию — `/Users/<username>`.

Если вы использовали apt-get, Docker или MSI-файл для установки интерфейса командной строки, используйте тот же инструмент для его удаления.

## <a name="reporting-issues-and-feedback"></a>Создание отчетов о проблемах и обратная связь

При появлении ошибок в средстве сообщите о проблеме в разделе [Проблемы](https://github.com/Azure/azure-cli/issues) репозитория GitHub.
Чтобы отправить отзыв из командной строки, попробуйте использовать команду `az feedback`.
