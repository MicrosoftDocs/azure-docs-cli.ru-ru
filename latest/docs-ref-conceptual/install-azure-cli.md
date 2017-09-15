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
ms.openlocfilehash: a61f47076854d0ff0a7056f82240794b7533fe3e
ms.sourcegitcommit: 3db5fb207db551a0d3fe0a88fe09e8f5e2ec184d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="3e0ed-104">Установка Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="3e0ed-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="3e0ed-105">Установите новую версию интерфейса командной строки Azure прямо сейчас!</span><span class="sxs-lookup"><span data-stu-id="3e0ed-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="3e0ed-106">Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="3e0ed-107">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="3e0ed-108">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3e0ed-109">Если вам нужна предыдущая версия Azure CLI, см. руководство по [установке Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="3e0ed-110"><a name="macOS"/>Установка в macOS</span><span class="sxs-lookup"><span data-stu-id="3e0ed-110"><a name="macOS"/>Install on macOS</span></span>

1. <span data-ttu-id="3e0ed-111">Установите Azure CLI 2.0 с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-111">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="3e0ed-112">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-112">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="3e0ed-113">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-113">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="3e0ed-114">Установка в Windows</span><span class="sxs-lookup"><span data-stu-id="3e0ed-114">Install on Windows</span></span>

<span data-ttu-id="3e0ed-115">Azure CLI 2.0 можно установить с помощью MSI-файла, чтобы использовать в командной строке Windows, или установить с помощью `apt-get` для Bash, чтобы использовать на платформе Ubuntu в Windows.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-115">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with `apt-get` on Bash on Ubuntu on Windows.</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="3e0ed-116">Установка с помощью MSI-файла для командной строки Windows</span><span class="sxs-lookup"><span data-stu-id="3e0ed-116">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="3e0ed-117">Чтобы установить CLI в Windows и использовать его в окне командной строки Windows, скачайте и запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-117">To install the CLI on Windows and use it in the Windows command-line, download and run the [MSI](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="3e0ed-118">Установка с помощью apt-get для Bash на платформе Ubuntu в Windows</span><span class="sxs-lookup"><span data-stu-id="3e0ed-118">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="3e0ed-119">Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-119">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="3e0ed-120">Откройте оболочку Bash.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-120">Open the Bash shell.</span></span>

3. <span data-ttu-id="3e0ed-121">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-121">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="3e0ed-122">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-122">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="3e0ed-123">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-123">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="3e0ed-124">Установка на Debian или Ubuntu с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="3e0ed-124">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="3e0ed-125">В системах на базе Debian и Ubuntu можно установить Azure CLI 2.0 с помощью `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-125">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="3e0ed-126">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-126">Modify your sources list:</span></span>
 
   - <span data-ttu-id="3e0ed-127">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-127">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="3e0ed-128">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-128">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="3e0ed-129">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="3e0ed-130">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="3e0ed-131">Установка в RHEL, Fedora и CentOS с помощью yum</span><span class="sxs-lookup"><span data-stu-id="3e0ed-131">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="3e0ed-132">Для любого дистрибутива на базе RedHat, который содержит диспетчер пакетов `yum`, Azure CLI 2.0 можно установить с помощью `yum`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-132">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="3e0ed-133">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-133">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="3e0ed-134">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-134">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="3e0ed-135">Обновите индекс пакета `yum` и выполните установку: </span><span class="sxs-lookup"><span data-stu-id="3e0ed-135">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="3e0ed-136">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-136">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="3e0ed-137">Установка в openSUSE и SLE с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="3e0ed-137">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="3e0ed-138">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-138">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="3e0ed-139">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-139">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="3e0ed-140">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-140">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="3e0ed-141">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-141">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="3e0ed-142">Установка с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="3e0ed-142">Install with Docker</span></span>

<span data-ttu-id="3e0ed-143">Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-143">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="3e0ed-144">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-144">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="3e0ed-145">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-145">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="3e0ed-146">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-146">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="3e0ed-147">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-147">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="3e0ed-148"><a name="Linux"/>Установка в Linux без использования apt-get</span><span class="sxs-lookup"><span data-stu-id="3e0ed-148"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="3e0ed-149">Рекомендуется по возможности устанавливать CLI с помощью диспетчера пакетов (если вы знаете, как это сделать).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-149">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="3e0ed-150">Для дистрибутивов, для которых диспетчер пакетов не предоставляется, CLI можно установить вручную.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-150">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="3e0ed-151">Установите необходимые компоненты с учетом дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-151">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="3e0ed-152">Если дистрибутив не указан в списке выше, вам нужно установить [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) и [OpenSSL](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-152">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="3e0ed-153">Установите CLI с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-153">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="3e0ed-154">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-154">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="3e0ed-155">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-155">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3e0ed-156">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3e0ed-156">Troubleshooting</span></span>

<span data-ttu-id="3e0ed-157">Если при установке CLI возникла проблема, ознакомьтесь с этим разделом, чтобы найти описание своего случая.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-157">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="3e0ed-158">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-158">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="3e0ed-159">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="3e0ed-159">curl "Object Moved" error</span></span>

<span data-ttu-id="3e0ed-160">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="3e0ed-160">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="homebrew-on-macos-installing-older-version"></a><span data-ttu-id="3e0ed-161">Homebrew на macOS устанавливает устаревшую версию</span><span class="sxs-lookup"><span data-stu-id="3e0ed-161">Homebrew on macOS installing older version</span></span>

<span data-ttu-id="3e0ed-162">Текущая формула `azure-cli` Homebrew для macOS устарела. При ее использовании будет устанавливаться CLI версии 1.x.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-162">The Homebrew `azure-cli` formula available for macOS is currently out of date, and will install a 1.x version of the CLI.</span></span> <span data-ttu-id="3e0ed-163">Вы можете узнать о ее обновлении, выполнив команду `brew info azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-163">You can see when it is updated by checking `brew info azure-cli`.</span></span>

<span data-ttu-id="3e0ed-164">А пока [удалите устаревшую версию](#uninstall_brew) и следуйте [инструкциям по установке для macOS](#macOS).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-164">Until then, [uninstall the older version](#uninstall_brew) and follow the [macOS install instructions](#macOS).</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="3e0ed-165">Удаление версий CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="3e0ed-165">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="3e0ed-166">Если в системе установлена более ранняя версия CLI 1.x, вы можете удалить ее с учетом примененного типа установки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-166">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="3e0ed-167">Удаление с помощью npm</span><span class="sxs-lookup"><span data-stu-id="3e0ed-167">Uninstall with npm</span></span>

<span data-ttu-id="3e0ed-168">Удалите устаревшую версию CLI с помощью команды `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-168">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="a-nameuninstallbrewuninstall-with-homebrew-on-macos"></a><span data-ttu-id="3e0ed-169"><a name="uninstall_brew"/>Удаление с помощью Homebrew на macOS</span><span class="sxs-lookup"><span data-stu-id="3e0ed-169"><a name="uninstall_brew"/>Uninstall with Homebrew on macOS</span></span>

<span data-ttu-id="3e0ed-170">Удалите устаревшую версию CLI с помощью команды `brew uninstall`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-170">Remove the older CLI with `brew uninstall`.</span></span>

```bash
brew uninstall azure-cli
```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="3e0ed-171">Удаление с помощью распространяемых компонентов</span><span class="sxs-lookup"><span data-stu-id="3e0ed-171">Uninstall with distributable</span></span>

<span data-ttu-id="3e0ed-172">Если установка выполнялась с использованием [MSI](http://aka.ms/webpi-azure-cli)-файла или [пакета macOS](http://aka.ms/mac-azure-cli), используйте то же средство для удаления файлов установки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-172">If you installed via [MSI](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="3e0ed-173">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="3e0ed-173">Uninstall with Docker</span></span>

<span data-ttu-id="3e0ed-174">Если вы установили образ Docker, чтобы использовать более раннюю версию CLI, удалите этот образ и все связанные контейнеры.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-174">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="3e0ed-175">Позже вы сможете повторно создать контейнеры, установив новый образ Docker, как описано в инструкциях по установке.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-175">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="3e0ed-176">Обновление интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="3e0ed-176">Update the CLI</span></span>

<span data-ttu-id="3e0ed-177">Чтобы обновить Azure CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-177">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-msi"></a><span data-ttu-id="3e0ed-178">Обновление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="3e0ed-178">Update with MSI</span></span>

<span data-ttu-id="3e0ed-179">Запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-179">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="3e0ed-180">Обновление с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="3e0ed-180">Update with apt-get</span></span>

<span data-ttu-id="3e0ed-181">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-181">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="3e0ed-182">В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-182">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="3e0ed-183">Чтобы обновить только CLI, используйте команду `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-183">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="3e0ed-184">Обновление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="3e0ed-184">Update with Docker</span></span>

1. <span data-ttu-id="3e0ed-185">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-185">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="3e0ed-186">Получите данные о контейнерах, которые используют образ CLI.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-186">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="3e0ed-187">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-187">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="3e0ed-188">Остановите и заново создайте контейнеры.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-188">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="3e0ed-189">Обновление вручную</span><span class="sxs-lookup"><span data-stu-id="3e0ed-189">Update manually</span></span>

<span data-ttu-id="3e0ed-190">Следуйте инструкциям по установке вручную для обновления в [macOS](#macOS) или [Linux](#Linux).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-190">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="3e0ed-191">Удаление</span><span class="sxs-lookup"><span data-stu-id="3e0ed-191">Uninstall</span></span>

<span data-ttu-id="3e0ed-192">Нам будет очень жаль, если вы решите удалить CLI.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-192">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="3e0ed-193">Чтобы удалить CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-193">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-msi"></a><span data-ttu-id="3e0ed-194">Удаление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="3e0ed-194">Uninstall with MSI</span></span>

<span data-ttu-id="3e0ed-195">Запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".</span><span class="sxs-lookup"><span data-stu-id="3e0ed-195">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="3e0ed-196">Удаление с помощью apt-get</span><span class="sxs-lookup"><span data-stu-id="3e0ed-196">Uninstall with apt-get</span></span>

<span data-ttu-id="3e0ed-197">Выполните удаление с помощью `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-197">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="3e0ed-198">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="3e0ed-198">Uninstall with Docker</span></span>

<span data-ttu-id="3e0ed-199">Если вы установили образ Docker, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-199">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="3e0ed-200">Получите данные о контейнерах, на которых запущен образ azure-cli.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-200">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="3e0ed-201">Удалите все контейнеры с образом CLI.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-201">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="3e0ed-202">Удалите локально установленный образ CLI.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-202">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="3e0ed-203">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-203">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

### <a name="uninstall-manually"></a><span data-ttu-id="3e0ed-204">Удаление вручную</span><span class="sxs-lookup"><span data-stu-id="3e0ed-204">Uninstall manually</span></span>

<span data-ttu-id="3e0ed-205">Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-205">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="3e0ed-206">Удалите установленные файлы.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-206">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="3e0ed-207">Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-207">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="3e0ed-208">Расположение установки по умолчанию — `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-208">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="3e0ed-209">Создание отчетов о проблемах CLI и обратная связь</span><span class="sxs-lookup"><span data-stu-id="3e0ed-209">Report CLI issues and feedback</span></span>

<span data-ttu-id="3e0ed-210">Если при работе со средством возникают ошибки, сообщите об этом в разделе репозитория GitHub, посвященном [проблемам](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3e0ed-210">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="3e0ed-211">Чтобы отправить отзыв из командной строки, используйте команду `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3e0ed-211">To provide feedback from the command line, use the `az feedback` command.</span></span>
