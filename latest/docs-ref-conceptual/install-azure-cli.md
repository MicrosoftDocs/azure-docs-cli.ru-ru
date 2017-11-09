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
ms.openlocfilehash: 4703a192e23b04d0ad42daf60e415d798610cce0
ms.sourcegitcommit: 932cc86172ab55c00346f62504787c096ed7b2bd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="42735-104">Установка Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="42735-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="42735-105">Установите новую версию интерфейса командной строки Azure прямо сейчас!</span><span class="sxs-lookup"><span data-stu-id="42735-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="42735-106">Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="42735-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="42735-107">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="42735-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="42735-108">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="42735-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="42735-109">Если вам нужна предыдущая версия Azure CLI, см. руководство по [установке Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="42735-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="42735-110"><a name="macOS"/>Установка в macOS</span><span class="sxs-lookup"><span data-stu-id="42735-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="42735-111">В macOS установку можно выполнить с помощью [Homebrew](https://brew.sh/) или вручную.</span><span class="sxs-lookup"><span data-stu-id="42735-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="42735-112">Установка с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="42735-112">Install with Homebrew</span></span>

1. <span data-ttu-id="42735-113">Если у вас нет этой программы, выполните [инструкции по установке Homebrew](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="42735-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="42735-114">Если CLI устанавливался вручную, следуйте инструкциям по [удалению вручную](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="42735-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="42735-115">Обновите свои локальные репозитории Homebrew.</span><span class="sxs-lookup"><span data-stu-id="42735-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="42735-116">Установите пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="42735-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="42735-117">Если вы ранее установили Azure CLI 1.0 с помощью Homebrew, вместо установки пакета можно получить CLI 2.0 при регулярном обновлении Homebrew.</span><span class="sxs-lookup"><span data-stu-id="42735-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="42735-118">Установка вручную</span><span class="sxs-lookup"><span data-stu-id="42735-118">Install manually</span></span>

1. <span data-ttu-id="42735-119">Установите Azure CLI 2.0 с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="42735-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="42735-120">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="42735-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="42735-121">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="42735-122">Установка в Windows</span><span class="sxs-lookup"><span data-stu-id="42735-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="42735-123">Установка с помощью MSI-файла для командной строки Windows</span><span class="sxs-lookup"><span data-stu-id="42735-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="42735-124">Чтобы установить CLI в Windows и использовать его в окне командной строки Windows, скачайте и запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="42735-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="42735-125">Установка с помощью apt-get для Bash на платформе Ubuntu в Windows</span><span class="sxs-lookup"><span data-stu-id="42735-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="42735-126">Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="42735-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="42735-127">Откройте оболочку Bash.</span><span class="sxs-lookup"><span data-stu-id="42735-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="42735-128">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="42735-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="42735-129">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="42735-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="42735-130">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="42735-131">Установка на Debian или Ubuntu с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="42735-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="42735-132">Для дистрибутивов с поддержкой диспетчера пакетов `apt` можно установить Azure CLI 2.0, используя `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="42735-132">For distributions using the `apt` package manager, you can install Azure CLI 2.0 via `apt-get`.</span></span>

> [!NOTE]
> <span data-ttu-id="42735-133">Для работы с CLI дистрибутив должен поддерживать Python 2.7.x или Python 3.x.</span><span class="sxs-lookup"><span data-stu-id="42735-133">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="42735-134">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="42735-134">Modify your sources list:</span></span>
 
   - <span data-ttu-id="42735-135">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="42735-135">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="42735-136">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="42735-136">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="42735-137">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="42735-137">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="42735-138">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-138">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="42735-139">Установка в RHEL, Fedora и CentOS с помощью yum</span><span class="sxs-lookup"><span data-stu-id="42735-139">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="42735-140">Для дистрибутивов с поддержкой диспетчера пакетов `yum` можно установить Azure CLI 2.0, используя `yum`.</span><span class="sxs-lookup"><span data-stu-id="42735-140">For distributions which use the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

> [!NOTE]
> <span data-ttu-id="42735-141">Для работы с CLI дистрибутив должен поддерживать Python 2.7.x или Python 3.x.</span><span class="sxs-lookup"><span data-stu-id="42735-141">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="42735-142">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="42735-142">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="42735-143">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="42735-143">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="42735-144">Обновите индекс пакета `yum` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="42735-144">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="42735-145">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-145">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="42735-146">Установка в openSUSE и SLE с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="42735-146">Install on openSUSE and SLE with zypper</span></span>

<span data-ttu-id="42735-147">Для дистрибутивов с поддержкой диспетчера пакетов `zypper` можно установить Azure CLI 2.0, используя `zypper`.</span><span class="sxs-lookup"><span data-stu-id="42735-147">For distributions which use the `zypper` package manager, you can install Azure CLI 2.0 via `zypper`.</span></span>

> [!NOTE]
> <span data-ttu-id="42735-148">Для работы с CLI дистрибутив должен поддерживать Python 2.7.x или Python 3.x.</span><span class="sxs-lookup"><span data-stu-id="42735-148">Your distribution must have support for Python 2.7.x or Python 3.x in order to use the CLI.</span></span>

1. <span data-ttu-id="42735-149">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="42735-149">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="42735-150">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="42735-150">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="42735-151">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="42735-151">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="42735-152">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-152">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="42735-153">Установка с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="42735-153">Install with Docker</span></span>

<span data-ttu-id="42735-154">Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="42735-154">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="42735-155">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="42735-155">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="42735-156">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="42735-156">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="42735-157">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="42735-157">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="42735-158">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="42735-158">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="42735-159"><a name="Linux"/>Установка в Linux без использования диспетчера пакетов</span><span class="sxs-lookup"><span data-stu-id="42735-159"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="42735-160">Рекомендуется по возможности устанавливать CLI с помощью диспетчера пакетов (если вы знаете, как это сделать).</span><span class="sxs-lookup"><span data-stu-id="42735-160">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="42735-161">Если вы не хотите добавлять репозитории Майкрософт или работаете с дистрибутивами, которые не поддерживают указанный пакет, CLI можно установить вручную.</span><span class="sxs-lookup"><span data-stu-id="42735-161">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="42735-162">Установите необходимые компоненты с учетом дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="42735-162">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="42735-163">Если дистрибутив не указан в списке выше, вам нужно установить [Python 2.7 или более поздней версии](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) и [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="42735-163">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="42735-164">Установите CLI с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="42735-164">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="42735-165">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="42735-165">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="42735-166">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="42735-166">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="42735-167">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="42735-167">Troubleshooting</span></span>

<span data-ttu-id="42735-168">Если при установке CLI возникла проблема, ознакомьтесь с этим разделом, чтобы найти описание своего случая.</span><span class="sxs-lookup"><span data-stu-id="42735-168">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="42735-169">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="42735-169">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="42735-170">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="42735-170">curl "Object Moved" error</span></span>

<span data-ttu-id="42735-171">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="42735-171">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="42735-172">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="42735-172">`az` command not found</span></span>

<span data-ttu-id="42735-173">Попробуйте очистить кэш хэша команд оболочки.</span><span class="sxs-lookup"><span data-stu-id="42735-173">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="42735-174">Выполнить</span><span class="sxs-lookup"><span data-stu-id="42735-174">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="42735-175">и посмотрите, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="42735-175">and see if the problem is resolved.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="42735-176">Удаление версий CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="42735-176">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="42735-177">Если в системе установлена более ранняя версия CLI 1.x, вы можете удалить ее с учетом примененного типа установки.</span><span class="sxs-lookup"><span data-stu-id="42735-177">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="42735-178">Удаление с помощью npm</span><span class="sxs-lookup"><span data-stu-id="42735-178">Uninstall with npm</span></span>

<span data-ttu-id="42735-179">Удалите устаревшую версию CLI с помощью команды `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="42735-179">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="42735-180">Удаление с помощью распространяемых компонентов</span><span class="sxs-lookup"><span data-stu-id="42735-180">Uninstall with distributable</span></span>

<span data-ttu-id="42735-181">Если установка выполнялась с использованием [установщика Azure CLI (MSI)](http://aka.ms/webpi-azure-cli) или [пакета macOS](http://aka.ms/mac-azure-cli), используйте то же средство для удаления файлов установки.</span><span class="sxs-lookup"><span data-stu-id="42735-181">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="42735-182">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="42735-182">Uninstall with Docker</span></span>

<span data-ttu-id="42735-183">Если вы установили образ Docker, чтобы использовать более раннюю версию CLI, удалите этот образ и все связанные контейнеры.</span><span class="sxs-lookup"><span data-stu-id="42735-183">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="42735-184">Позже вы сможете повторно создать контейнеры, установив новый образ Docker, как описано в инструкциях по установке.</span><span class="sxs-lookup"><span data-stu-id="42735-184">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="42735-185">Обновление интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="42735-185">Update the CLI</span></span>

<span data-ttu-id="42735-186">Чтобы обновить Azure CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="42735-186">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="42735-187">Обновление с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="42735-187">Update with Homebrew</span></span>

1. <span data-ttu-id="42735-188">Если установка выполнялась вручную, следуйте инструкциям по [установке с помощью Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="42735-188">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="42735-189">Обновите свои данные в локальном репозитории Homebrew.</span><span class="sxs-lookup"><span data-stu-id="42735-189">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="42735-190">Обновите установленные пакеты.</span><span class="sxs-lookup"><span data-stu-id="42735-190">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="42735-191">Обновление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="42735-191">Update with MSI</span></span>

<span data-ttu-id="42735-192">Запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows) еще раз.</span><span class="sxs-lookup"><span data-stu-id="42735-192">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="42735-193">Обновление с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="42735-193">Update with apt-get</span></span>

<span data-ttu-id="42735-194">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="42735-194">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="42735-195">В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="42735-195">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="42735-196">Чтобы обновить только CLI, используйте команду `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="42735-196">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="42735-197">Обновление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="42735-197">Update with Docker</span></span>

1. <span data-ttu-id="42735-198">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="42735-198">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="42735-199">Получите данные о контейнерах, которые используют образ CLI.</span><span class="sxs-lookup"><span data-stu-id="42735-199">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="42735-200">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="42735-200">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="42735-201">Остановите и заново создайте контейнеры.</span><span class="sxs-lookup"><span data-stu-id="42735-201">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="42735-202">Обновление вручную</span><span class="sxs-lookup"><span data-stu-id="42735-202">Update manually</span></span>

<span data-ttu-id="42735-203">Следуйте инструкциям по установке вручную для обновления в [macOS](#macOS) или [Linux](#Linux).</span><span class="sxs-lookup"><span data-stu-id="42735-203">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="42735-204">Удаление</span><span class="sxs-lookup"><span data-stu-id="42735-204">Uninstall</span></span>

<span data-ttu-id="42735-205">Нам будет очень жаль, если вы решите удалить CLI.</span><span class="sxs-lookup"><span data-stu-id="42735-205">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="42735-206">Чтобы удалить CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="42735-206">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="42735-207">Удаление с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="42735-207">Uninstall with Homebrew</span></span>

<span data-ttu-id="42735-208">Удалите пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="42735-208">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="42735-209">Удаление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="42735-209">Uninstall with MSI</span></span>

<span data-ttu-id="42735-210">Запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".</span><span class="sxs-lookup"><span data-stu-id="42735-210">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="42735-211">Удаление с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="42735-211">Uninstall with apt-get</span></span>

<span data-ttu-id="42735-212">Выполните удаление с помощью `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="42735-212">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="42735-213">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="42735-213">Uninstall with Docker</span></span>

<span data-ttu-id="42735-214">Если вы установили образ Docker, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.</span><span class="sxs-lookup"><span data-stu-id="42735-214">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="42735-215">Получите данные о контейнерах, на которых запущен образ azure-cli.</span><span class="sxs-lookup"><span data-stu-id="42735-215">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="42735-216">Удалите все контейнеры с образом CLI.</span><span class="sxs-lookup"><span data-stu-id="42735-216">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="42735-217">Удалите локально установленный образ CLI.</span><span class="sxs-lookup"><span data-stu-id="42735-217">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="42735-218">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="42735-218">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="42735-219"><a name="UninstallManually"/>Удаление вручную</span><span class="sxs-lookup"><span data-stu-id="42735-219"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="42735-220">Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="42735-220">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="42735-221">Удалите установленные файлы.</span><span class="sxs-lookup"><span data-stu-id="42735-221">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="42735-222">Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="42735-222">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="42735-223">Если оболочка использует кэш команд, перезагрузите его.</span><span class="sxs-lookup"><span data-stu-id="42735-223">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="42735-224">Расположение установки по умолчанию — `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="42735-224">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="42735-225">Создание отчетов о проблемах CLI и обратная связь</span><span class="sxs-lookup"><span data-stu-id="42735-225">Report CLI issues and feedback</span></span>

<span data-ttu-id="42735-226">Если при работе со средством возникают ошибки, сообщите об этом в разделе репозитория GitHub, посвященном [проблемам](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="42735-226">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="42735-227">Чтобы отправить отзыв из командной строки, используйте команду `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="42735-227">To provide feedback from the command line, use the `az feedback` command.</span></span>