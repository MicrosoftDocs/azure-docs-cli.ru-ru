---
title: Установка Azure CLI в Linux с помощью zypper
description: Как установить Azure CLI с помощью zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e501d05985b0483442ab11f78343d773fd7e55bf
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687096"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="af79a-103">Установка Azure CLI с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="af79a-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="af79a-104">Для дистрибутивов Linux, использующих `zypper`, например openSUSE или SLES, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="af79a-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="af79a-105">Этот пакет протестирован с openSUSE Leap 15.1 и SLES 15.</span><span class="sxs-lookup"><span data-stu-id="af79a-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="af79a-106">Установка</span><span class="sxs-lookup"><span data-stu-id="af79a-106">Install</span></span>

1. <span data-ttu-id="af79a-107">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="af79a-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="af79a-108">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="af79a-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="af79a-109">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="af79a-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="af79a-110">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="af79a-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   <span data-ttu-id="af79a-111">Используйте вход 2 чтобы продолжить установку, игнорируя некоторые зависимости.</span><span class="sxs-lookup"><span data-stu-id="af79a-111">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="af79a-112">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="af79a-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="af79a-113">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="af79a-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="af79a-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="af79a-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="af79a-115">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="af79a-115">Troubleshooting</span></span>

<span data-ttu-id="af79a-116">Ниже описаны некоторые распространенные проблемы при установке с помощью `zypper`.</span><span class="sxs-lookup"><span data-stu-id="af79a-116">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="af79a-117">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="af79a-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="af79a-118">Ошибка NotImplementedError в виртуальной машине OpenSUSE 15</span><span class="sxs-lookup"><span data-stu-id="af79a-118">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="af79a-119">Виртуальная машина OpenSUSE 15 поставляется с предварительно установленной версией Azure CLI `2.0.45`, которая устарела и имеет проблемы с `az login`.</span><span class="sxs-lookup"><span data-stu-id="af79a-119">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="af79a-120">Удалите ее вместе с зависимостями, прежде чем переходить к [инструкции по установке](#install), чтобы добавить последнюю версию Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="af79a-120">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>
```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="af79a-121">Если вы обновили Azure CLI без удаления зависимостей версии `2.0.45`, старые зависимости могут повлиять на работу последней версии Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="af79a-121">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="af79a-122">Необходимо вернуть старую версию, чтобы связать ее с зависимостями, а затем удалить `azure-cli` вместе с зависимостями:</span><span class="sxs-lookup"><span data-stu-id="af79a-122">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>
```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```


### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="af79a-123">Установка в SLES 12 или других системах без Python 3.6</span><span class="sxs-lookup"><span data-stu-id="af79a-123">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="af79a-124">В SLES 12 пакет `python3` по умолчанию теперь имеет версию `3.4` и не поддерживается в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="af79a-124">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="af79a-125">Вы можете сначала выполнить шаги 1–3 [инструкции по установке](#install), чтобы добавить репозиторий `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="af79a-125">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="af79a-126">Затем выполните сборку более поздней версии `python3` из источника.</span><span class="sxs-lookup"><span data-stu-id="af79a-126">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="af79a-127">Наконец, можно скачать пакет Azure CLI и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="af79a-127">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="af79a-128">Для установки Azure CLI можно использовать следующую команду (помните, что существующая версия Python 3 будет переопределена версией Python 3.6):</span><span class="sxs-lookup"><span data-stu-id="af79a-128">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="af79a-129">Кроме того, это можно сделать пошагово:</span><span class="sxs-lookup"><span data-stu-id="af79a-129">Or you can do it step by step:</span></span>

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

### <a name="proxy-blocks-connection"></a><span data-ttu-id="af79a-130">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="af79a-130">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="af79a-131">Вы также можете явным образом настроить `zypper` (через `yast2`), чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="af79a-131">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="af79a-132">Чтобы сделать это, выполните команду `yast2 proxy` как суперпользователь и заполните форму.</span><span class="sxs-lookup"><span data-stu-id="af79a-132">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="af79a-133">Если в системе установлен диспетчер окон, можно также использовать панель `Network Services > Proxy` в `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="af79a-133">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="af79a-134">Дополнительные сведения о расширенной конфигурации см. в [документации по конфигурации прокси-сервера OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="af79a-134">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="af79a-135">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="af79a-135">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="af79a-136">Проблема с сертификатом SSL</span><span class="sxs-lookup"><span data-stu-id="af79a-136">SSL certificate problem</span></span>

<span data-ttu-id="af79a-137">Если сертификат на компьютере поврежден или устарел, может поступить сообщение об ошибке, указывающее на то, что произошел сбой при проверке подлинности сервера, из-за чего не удалось установить безопасное подключение.</span><span class="sxs-lookup"><span data-stu-id="af79a-137">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="af79a-138">Обновите сертификат, чтобы устранить проблему.</span><span class="sxs-lookup"><span data-stu-id="af79a-138">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="af79a-139">Update</span><span class="sxs-lookup"><span data-stu-id="af79a-139">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="af79a-140">Вы также можете обновить пакет с помощью команды `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="af79a-140">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="af79a-141">Удаление</span><span class="sxs-lookup"><span data-stu-id="af79a-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="af79a-142">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="af79a-142">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="af79a-143">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="af79a-143">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="af79a-144">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="af79a-144">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="af79a-145">Next Steps</span><span class="sxs-lookup"><span data-stu-id="af79a-145">Next Steps</span></span>

<span data-ttu-id="af79a-146">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="af79a-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="af79a-147">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="af79a-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)