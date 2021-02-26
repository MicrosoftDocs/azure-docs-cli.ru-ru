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
## <a name="overview"></a><span data-ttu-id="bad5b-101">Обзор</span><span class="sxs-lookup"><span data-stu-id="bad5b-101">Overview</span></span>

<span data-ttu-id="bad5b-102">Для дистрибутивов Linux, использующих `dnf`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="bad5b-102">For Linux distributions with `dnf` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="bad5b-103">Этот пакет протестирован с RHEL 7.7 и 8, Fedora 24 и более поздних версий, а также CentOS 7 и 8.</span><span class="sxs-lookup"><span data-stu-id="bad5b-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> <span data-ttu-id="bad5b-104">Если вы работаете с системами Linux, которые не поддерживаю диспетчер пакетов `dnf`, используйте диспетчер пакетов `yum`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-104">Use `yum` package manager if you are using Linux systems that don't support `dnf` package manager.</span></span>

## <a name="install"></a><span data-ttu-id="bad5b-105">Установка</span><span class="sxs-lookup"><span data-stu-id="bad5b-105">Install</span></span>

1. <span data-ttu-id="bad5b-106">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bad5b-106">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="bad5b-107">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-107">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="bad5b-108">Выполните установку с помощью команды `dnf install`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-108">Install with the `dnf install` command.</span></span>

   ```bash
   sudo dnf install azure-cli
   ```
 
<span data-ttu-id="bad5b-109">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-109">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="bad5b-110">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="bad5b-110">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>


[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="bad5b-111">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bad5b-111">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="bad5b-112">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="bad5b-112">Troubleshooting</span></span>

<span data-ttu-id="bad5b-113">Ниже описаны некоторые распространенные проблемы при установке с помощью `dnf`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-113">Here are some common problems seen when installing with `dnf`.</span></span> <span data-ttu-id="bad5b-114">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="bad5b-114">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="bad5b-115">Установка в RHEL 7.6 или других системах без Python 3</span><span class="sxs-lookup"><span data-stu-id="bad5b-115">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="bad5b-116">По возможности обновите систему до версии с официальной поддержкой пакета `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-116">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="bad5b-117">В противном случае необходимо сначала установить пакет `python3`, а затем установить Azure CLI без зависимости.</span><span class="sxs-lookup"><span data-stu-id="bad5b-117">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="bad5b-118">Для установки Azure CLI с `python 3.6` (сборка из источника), можно использовать следующую команду:</span><span class="sxs-lookup"><span data-stu-id="bad5b-118">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="bad5b-119">Кроме того, это можно сделать пошагово:</span><span class="sxs-lookup"><span data-stu-id="bad5b-119">You can also do it step by step:</span></span>

<span data-ttu-id="bad5b-120">Azure CLI требуется `SSL 1.1+`, и вам нужно создать `openssl 1.1` из источника перед созданием `python3`:</span><span class="sxs-lookup"><span data-stu-id="bad5b-120">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

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

<span data-ttu-id="bad5b-121">Затем выполните сборку Python 3 из источника:</span><span class="sxs-lookup"><span data-stu-id="bad5b-121">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="bad5b-122">Наконец, выполните шаги 1–2 [инструкции по установке](#install), чтобы добавить репозиторий Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="bad5b-122">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="bad5b-123">Затем можно скачать пакет и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="bad5b-123">You can now download the package and install it without dependency.</span></span>

> [!NOTE]
>
> <span data-ttu-id="bad5b-124">Если подключаемый модуль скачивания dnf не установлен, при выполнении приведенного ниже кода произойдет ошибка "Команда не найдена".</span><span class="sxs-lookup"><span data-stu-id="bad5b-124">In case you don't have the dnf download plugin installed, you will encounter command not found error on executing the below code.</span></span> <span data-ttu-id="bad5b-125">Установите подключаемый модуль скачивания dnf с помощью команды `dnf install 'dnf-command(download)'`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-125">Use `dnf install 'dnf-command(download)'` to   install the dnf download plugin.</span></span>

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="bad5b-126">В качестве альтернативы можно также установить Python 3, используя [дополнительные репозитории](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="bad5b-126">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="bad5b-127">Таким образом, если вы установили `python3`, но у вас по-прежнему возникает ошибка `python3: command not found` при попытке запустить CLI, необходимо включить его в путь.</span><span class="sxs-lookup"><span data-stu-id="bad5b-127">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="bad5b-128">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="bad5b-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="bad5b-129">Вы также можете явным образом настроить `dnf`, чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="bad5b-129">You may also want to explicitly configure `dnf` to use this proxy at all times.</span></span> <span data-ttu-id="bad5b-130">Убедитесь, что следующие строки отображаются в разделе `[main]` в `/etc/dnf/dnf.conf`:</span><span class="sxs-lookup"><span data-stu-id="bad5b-130">Make sure that the following lines appear under the `[main]` section of `/etc/dnf/dnf.conf`:</span></span>

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="bad5b-131">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:</span><span class="sxs-lookup"><span data-stu-id="bad5b-131">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="bad5b-132">Update</span><span class="sxs-lookup"><span data-stu-id="bad5b-132">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="bad5b-133">Вы также можете обновить Azure CLI с помощью команды `dnf update`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-133">You can also update the Azure CLI with the `dnf update` command.</span></span>

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="bad5b-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="bad5b-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="bad5b-135">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="bad5b-135">Remove the package from your system.</span></span>

   ```bash
   sudo dnf remove azure-cli
   ```

2. <span data-ttu-id="bad5b-136">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="bad5b-136">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="bad5b-137">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания.</span><span class="sxs-lookup"><span data-stu-id="bad5b-137">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
