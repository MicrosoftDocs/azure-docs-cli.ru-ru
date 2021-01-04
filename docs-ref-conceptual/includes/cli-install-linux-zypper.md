---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d80970432a116656a33a3dc6c0d4909b4b92f312
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744643"
---
## <a name="overview"></a>Обзор

Для дистрибутивов Linux, использующих `zypper`, например openSUSE или SLES, доступен пакет Azure CLI. Этот пакет протестирован с openSUSE Leap 15.1 и SLES 15.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a>Установка

1. Установите `curl`:

   ```bash
   sudo zypper install -y curl
   ```

2. Импортируйте ключ репозитория Майкрософт:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Создайте сведения о локальном репозитории `azure-cli`:

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. Обновите индекс пакета `zypper` и выполните установку:

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```

   Используйте вход 2 чтобы продолжить установку, игнорируя некоторые зависимости.

Запустите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы при установке с помощью `zypper`. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="notimplementederror-on-opensuse-15-vm"></a>Ошибка NotImplementedError в виртуальной машине OpenSUSE 15
Виртуальная машина OpenSUSE 15 поставляется с предварительно установленной версией Azure CLI `2.0.45`, которая устарела и имеет проблемы с `az login`. Удалите ее вместе с зависимостями, прежде чем переходить к [инструкции по установке](#install), чтобы добавить последнюю версию Azure CLI:

```bash
sudo zypper rm -y --clean-deps azure-cli
```

Если вы обновили Azure CLI без удаления зависимостей версии `2.0.45`, старые зависимости могут повлиять на работу последней версии Azure CLI. Необходимо вернуть старую версию, чтобы связать ее с зависимостями, а затем удалить `azure-cli` вместе с зависимостями:

```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a>Установка в SLES 12 или других системах без Python 3.6

В SLES 12 пакет `python3` по умолчанию теперь имеет версию `3.4` и не поддерживается в Azure CLI. Вы можете сначала выполнить шаги 1–3 [инструкции по установке](#install), чтобы добавить репозиторий `azure-cli`. Затем выполните сборку более поздней версии `python3` из источника. Наконец, можно скачать пакет Azure CLI и установить его без зависимости.

Для установки Azure CLI можно использовать следующую команду (помните, что существующая версия Python 3 будет переопределена версией Python 3.6):

```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

Кроме того, это можно сделать пошагово:

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a>Прокси-сервер блокирует подключения

[!INCLUDE[configure-proxy](configure-proxy.md)]

Вы также можете явным образом настроить `zypper` (через `yast2`), чтобы использовать этот прокси-сервер все время. Чтобы сделать это, выполните команду `yast2 proxy` как суперпользователь и заполните форму. Если в системе установлен диспетчер окон, можно также использовать панель `Network Services > Proxy` в `YaST Control Center`.

Дополнительные сведения о расширенной конфигурации см. в [документации по конфигурации прокси-сервера OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).

Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a>Проблема с сертификатом SSL

Если сертификат на компьютере поврежден или устарел, может поступить сообщение об ошибке, указывающее на то, что произошел сбой при проверке подлинности сервера, из-за чего не удалось установить безопасное подключение.  Обновите сертификат, чтобы устранить проблему.  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a>Update

[!INCLUDE [az-upgrade](az-upgrade.md)]

Вы также можете обновить пакет с помощью команды `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Удалите пакет из системы.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания (Майкрософт).

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
