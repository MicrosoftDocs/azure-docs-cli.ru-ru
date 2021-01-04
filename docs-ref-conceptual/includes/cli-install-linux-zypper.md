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
## <a name="overview"></a><span data-ttu-id="c3f56-101">Обзор</span><span class="sxs-lookup"><span data-stu-id="c3f56-101">Overview</span></span>

<span data-ttu-id="c3f56-102">Для дистрибутивов Linux, использующих `zypper`, например openSUSE или SLES, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c3f56-102">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="c3f56-103">Этот пакет протестирован с openSUSE Leap 15.1 и SLES 15.</span><span class="sxs-lookup"><span data-stu-id="c3f56-103">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="c3f56-104">Установка</span><span class="sxs-lookup"><span data-stu-id="c3f56-104">Install</span></span>

1. <span data-ttu-id="c3f56-105">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="c3f56-105">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="c3f56-106">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="c3f56-106">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="c3f56-107">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="c3f56-107">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="c3f56-108">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="c3f56-108">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```

   <span data-ttu-id="c3f56-109">Используйте вход 2 чтобы продолжить установку, игнорируя некоторые зависимости.</span><span class="sxs-lookup"><span data-stu-id="c3f56-109">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="c3f56-110">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="c3f56-111">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="c3f56-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="c3f56-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c3f56-112">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c3f56-113">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="c3f56-113">Troubleshooting</span></span>

<span data-ttu-id="c3f56-114">Ниже описаны некоторые распространенные проблемы при установке с помощью `zypper`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-114">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="c3f56-115">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c3f56-115">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="c3f56-116">Ошибка NotImplementedError в виртуальной машине OpenSUSE 15</span><span class="sxs-lookup"><span data-stu-id="c3f56-116">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="c3f56-117">Виртуальная машина OpenSUSE 15 поставляется с предварительно установленной версией Azure CLI `2.0.45`, которая устарела и имеет проблемы с `az login`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-117">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="c3f56-118">Удалите ее вместе с зависимостями, прежде чем переходить к [инструкции по установке](#install), чтобы добавить последнюю версию Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="c3f56-118">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>

```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="c3f56-119">Если вы обновили Azure CLI без удаления зависимостей версии `2.0.45`, старые зависимости могут повлиять на работу последней версии Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c3f56-119">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="c3f56-120">Необходимо вернуть старую версию, чтобы связать ее с зависимостями, а затем удалить `azure-cli` вместе с зависимостями:</span><span class="sxs-lookup"><span data-stu-id="c3f56-120">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>

```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="c3f56-121">Установка в SLES 12 или других системах без Python 3.6</span><span class="sxs-lookup"><span data-stu-id="c3f56-121">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="c3f56-122">В SLES 12 пакет `python3` по умолчанию теперь имеет версию `3.4` и не поддерживается в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c3f56-122">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="c3f56-123">Вы можете сначала выполнить шаги 1–3 [инструкции по установке](#install), чтобы добавить репозиторий `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-123">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="c3f56-124">Затем выполните сборку более поздней версии `python3` из источника.</span><span class="sxs-lookup"><span data-stu-id="c3f56-124">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="c3f56-125">Наконец, можно скачать пакет Azure CLI и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="c3f56-125">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="c3f56-126">Для установки Azure CLI можно использовать следующую команду (помните, что существующая версия Python 3 будет переопределена версией Python 3.6):</span><span class="sxs-lookup"><span data-stu-id="c3f56-126">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="c3f56-127">Кроме того, это можно сделать пошагово:</span><span class="sxs-lookup"><span data-stu-id="c3f56-127">Or you can do it step by step:</span></span>

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

### <a name="proxy-blocks-connection"></a><span data-ttu-id="c3f56-128">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="c3f56-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="c3f56-129">Вы также можете явным образом настроить `zypper` (через `yast2`), чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="c3f56-129">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="c3f56-130">Чтобы сделать это, выполните команду `yast2 proxy` как суперпользователь и заполните форму.</span><span class="sxs-lookup"><span data-stu-id="c3f56-130">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="c3f56-131">Если в системе установлен диспетчер окон, можно также использовать панель `Network Services > Proxy` в `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-131">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="c3f56-132">Дополнительные сведения о расширенной конфигурации см. в [документации по конфигурации прокси-сервера OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="c3f56-132">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="c3f56-133">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="c3f56-133">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="c3f56-134">Проблема с сертификатом SSL</span><span class="sxs-lookup"><span data-stu-id="c3f56-134">SSL certificate problem</span></span>

<span data-ttu-id="c3f56-135">Если сертификат на компьютере поврежден или устарел, может поступить сообщение об ошибке, указывающее на то, что произошел сбой при проверке подлинности сервера, из-за чего не удалось установить безопасное подключение.</span><span class="sxs-lookup"><span data-stu-id="c3f56-135">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="c3f56-136">Обновите сертификат, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="c3f56-136">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="c3f56-137">Update</span><span class="sxs-lookup"><span data-stu-id="c3f56-137">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="c3f56-138">Вы также можете обновить пакет с помощью команды `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="c3f56-138">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="c3f56-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="c3f56-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="c3f56-140">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="c3f56-140">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="c3f56-141">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="c3f56-141">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="c3f56-142">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="c3f56-142">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
