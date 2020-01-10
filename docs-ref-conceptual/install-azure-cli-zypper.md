---
title: Установка Azure CLI в Linux с помощью zypper
description: Как установить Azure CLI с помощью zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7e5897fe545527aa2708432e0ad0cf626584c785
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216890"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="73184-103">Установка Azure CLI с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="73184-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="73184-104">Для дистрибутивов Linux, использующих `zypper`, например openSUSE или SLES, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="73184-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="73184-105">Этот пакет протестирован с openSUSE Leap 15.1 и SLES 15.</span><span class="sxs-lookup"><span data-stu-id="73184-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="73184-106">Установка</span><span class="sxs-lookup"><span data-stu-id="73184-106">Install</span></span>

1. <span data-ttu-id="73184-107">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="73184-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="73184-108">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="73184-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="73184-109">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="73184-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="73184-110">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="73184-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="73184-111">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="73184-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="73184-112">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="73184-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="73184-113">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="73184-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="73184-114">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="73184-114">Troubleshooting</span></span>

<span data-ttu-id="73184-115">Ниже описаны некоторые распространенные проблемы при установке с помощью `zypper`.</span><span class="sxs-lookup"><span data-stu-id="73184-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="73184-116">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="73184-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-other-systems-without-python-36"></a><span data-ttu-id="73184-117">Установка в SLES 12 или других системах без Python 3.6</span><span class="sxs-lookup"><span data-stu-id="73184-117">Install on SLES 12 or other other systems without Python 3.6</span></span>

<span data-ttu-id="73184-118">В SLES 12 пакет python3 по умолчанию теперь имеет версию 3.4 и не поддерживается в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="73184-118">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="73184-119">Сначала можно создать более позднюю версию python3 из источника.</span><span class="sxs-lookup"><span data-stu-id="73184-119">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="73184-120">Затем можно скачать пакет Azure CLI и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="73184-120">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure --with-ssl
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="73184-121">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="73184-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="73184-122">Вы также можете явным образом настроить `zypper` (через `yast2`), чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="73184-122">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="73184-123">Чтобы сделать это, выполните команду `yast2 proxy` как суперпользователь и заполните форму.</span><span class="sxs-lookup"><span data-stu-id="73184-123">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="73184-124">Если в системе установлен диспетчер окон, можно также использовать панель `Network Services > Proxy` в `YaST Control Center`.</span><span class="sxs-lookup"><span data-stu-id="73184-124">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="73184-125">Дополнительные сведения о расширенной конфигурации см. в [документации по конфигурации прокси-сервера OpenSUSE](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="73184-125">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="73184-126">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="73184-126">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="73184-127">Update</span><span class="sxs-lookup"><span data-stu-id="73184-127">Update</span></span>

<span data-ttu-id="73184-128">Можно обновить пакет, воспользовавшись командой `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="73184-128">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="73184-129">Удаление</span><span class="sxs-lookup"><span data-stu-id="73184-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="73184-130">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="73184-130">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="73184-131">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="73184-131">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="73184-132">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="73184-132">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="73184-133">Next Steps</span><span class="sxs-lookup"><span data-stu-id="73184-133">Next Steps</span></span>

<span data-ttu-id="73184-134">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="73184-134">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="73184-135">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="73184-135">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
