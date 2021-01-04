---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6f121eff4f024da81dbf107fba5f5bd9d3b8aa0b
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744628"
---
## <a name="overview"></a><span data-ttu-id="5549e-101">Обзор</span><span class="sxs-lookup"><span data-stu-id="5549e-101">Overview</span></span>

<span data-ttu-id="5549e-102">Для дистрибутивов Linux, использующих `yum`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5549e-102">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="5549e-103">Этот пакет протестирован с RHEL 7.7 и 8, Fedora 24 и более поздних версий, а также CentOS 7 и 8.</span><span class="sxs-lookup"><span data-stu-id="5549e-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="5549e-104">Установка</span><span class="sxs-lookup"><span data-stu-id="5549e-104">Install</span></span>

1. <span data-ttu-id="5549e-105">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5549e-105">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="5549e-106">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="5549e-106">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="5549e-107">Выполните установку с помощью команды `yum install`.</span><span class="sxs-lookup"><span data-stu-id="5549e-107">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="5549e-108">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="5549e-108">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="5549e-109">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5549e-109">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="5549e-110">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5549e-110">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5549e-111">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5549e-111">Troubleshooting</span></span>

<span data-ttu-id="5549e-112">Ниже описаны некоторые распространенные проблемы при установке с помощью `yum`.</span><span class="sxs-lookup"><span data-stu-id="5549e-112">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="5549e-113">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5549e-113">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="5549e-114">Установка в RHEL 7.6 или других системах без Python 3</span><span class="sxs-lookup"><span data-stu-id="5549e-114">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="5549e-115">По возможности обновите систему до версии с официальной поддержкой пакета `python 3.6+`.</span><span class="sxs-lookup"><span data-stu-id="5549e-115">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="5549e-116">В противном случае необходимо сначала установить пакет `python3`, а затем установить Azure CLI без зависимости.</span><span class="sxs-lookup"><span data-stu-id="5549e-116">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="5549e-117">Для установки Azure CLI с `python 3.6` (сборка из источника), можно использовать следующую команду:</span><span class="sxs-lookup"><span data-stu-id="5549e-117">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="5549e-118">Кроме того, это можно сделать пошагово:</span><span class="sxs-lookup"><span data-stu-id="5549e-118">You can also do it step by step:</span></span>

<span data-ttu-id="5549e-119">Azure CLI требуется `SSL 1.1+`, и вам нужно создать `openssl 1.1` из источника перед созданием `python3`:</span><span class="sxs-lookup"><span data-stu-id="5549e-119">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

```bash
$ sudo yum install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
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

<span data-ttu-id="5549e-120">Затем выполните сборку Python 3 из источника:</span><span class="sxs-lookup"><span data-stu-id="5549e-120">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="5549e-121">Наконец, выполните шаги 1–2 [инструкции по установке](#install), чтобы добавить репозиторий Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5549e-121">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="5549e-122">Затем можно скачать пакет и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="5549e-122">You can now download the package and install it without dependency.</span></span>

```bash
$ sudo yum install yum-utils -y
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="5549e-123">В качестве альтернативы можно также установить Python 3, используя [дополнительные репозитории](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="5549e-123">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="5549e-124">Таким образом, если вы установили `python3`, но у вас по-прежнему возникает ошибка `python3: command not found` при попытке запустить CLI, необходимо включить его в путь.</span><span class="sxs-lookup"><span data-stu-id="5549e-124">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="5549e-125">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="5549e-125">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="5549e-126">Вы также можете явным образом настроить `yum`, чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="5549e-126">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="5549e-127">Убедитесь, что следующие строки отображаются в разделе `[main]` в `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="5549e-127">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="5549e-128">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:</span><span class="sxs-lookup"><span data-stu-id="5549e-128">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="5549e-129">Update</span><span class="sxs-lookup"><span data-stu-id="5549e-129">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="5549e-130">Вы также можете обновить Azure CLI с помощью команды `yum update`.</span><span class="sxs-lookup"><span data-stu-id="5549e-130">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="5549e-131">Удаление</span><span class="sxs-lookup"><span data-stu-id="5549e-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="5549e-132">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="5549e-132">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="5549e-133">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="5549e-133">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="5549e-134">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания.</span><span class="sxs-lookup"><span data-stu-id="5549e-134">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
