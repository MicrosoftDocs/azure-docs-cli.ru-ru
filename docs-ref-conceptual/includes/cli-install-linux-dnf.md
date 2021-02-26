---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: c0de92ff9aed581d192d72ca920fafea8bbd192b
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631023"
---
## <a name="overview"></a>Обзор

Для дистрибутивов Linux, использующих `dnf`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI. Этот пакет протестирован с RHEL 7.7 и 8, Fedora 24 и более поздних версий, а также CentOS 7 и 8.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> Если вы работаете с системами Linux, которые не поддерживаю диспетчер пакетов `dnf`, используйте диспетчер пакетов `yum`.

## <a name="install"></a>Установка

1. Импортируйте ключ репозитория Майкрософт.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Создайте сведения о локальном репозитории `azure-cli`.

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. Выполните установку с помощью команды `dnf install`.

   ```bash
   sudo dnf install azure-cli
   ```
 
Обновите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).


[!INCLUDE [interactive-login](interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы при установке с помощью `dnf`. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a>Установка в RHEL 7.6 или других системах без Python 3

По возможности обновите систему до версии с официальной поддержкой пакета `python 3.6+`. В противном случае необходимо сначала установить пакет `python3`, а затем установить Azure CLI без зависимости.

Для установки Azure CLI с `python 3.6` (сборка из источника), можно использовать следующую команду:

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

Кроме того, это можно сделать пошагово:

Azure CLI требуется `SSL 1.1+`, и вам нужно создать `openssl 1.1` из источника перед созданием `python3`:

```bash
$ sudo dnf install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
# build openssl from source
$ cd ~
$ wget https://www.openssl.org/source/openssl-1.1.1d.tar.gz
$ tar -xzf openssl-1.1.1d.tar.gz
$ cd openssl-1.1.1d
$ ./config --prefix=/usr/local/ssl --openssldir=/usr/local/ssl
$ make
$ sudo make install
# configure shared object lookup directory so that libssl.so.1.1 can be found
$ echo "/usr/local/ssl/lib" | sudo tee /etc/ld.so.conf.d/openssl-1.1.1d.conf
# reload config
$ sudo ldconfig -v
```

Затем выполните сборку Python 3 из источника:

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

Наконец, выполните шаги 1–2 [инструкции по установке](#install), чтобы добавить репозиторий Azure CLI. Затем можно скачать пакет и установить его без зависимости.

> [!NOTE]
>
> Если подключаемый модуль скачивания dnf не установлен, при выполнении приведенного ниже кода произойдет ошибка "Команда не найдена". Установите подключаемый модуль скачивания dnf с помощью команды `dnf install 'dnf-command(download)'`.

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

В качестве альтернативы можно также установить Python 3, используя [дополнительные репозитории](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/). Таким образом, если вы установили `python3`, но у вас по-прежнему возникает ошибка `python3: command not found` при попытке запустить CLI, необходимо включить его в путь.

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a>Прокси-сервер блокирует подключения

[!INCLUDE[configure-proxy](configure-proxy.md)]

Вы также можете явным образом настроить `dnf`, чтобы использовать этот прокси-сервер все время. Убедитесь, что следующие строки отображаются в разделе `[main]` в `/etc/dnf/dnf.conf`:

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Update

[!INCLUDE [az-upgrade](az-upgrade.md)]

Вы также можете обновить Azure CLI с помощью команды `dnf update`.

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Удалите пакет из системы.

   ```bash
   sudo dnf remove azure-cli
   ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
