---
title: "Установка Azure CLI 2.0"
description: "Справочная документация по установке Azure CLI 2.0"
keywords: Azure CLI, Install Azure CLI, Azure Python CLI, Azure CLI Reference
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 5a667ad8720100b45ff714601225535ef442545c
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="8cc75-104">Установка Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="8cc75-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="8cc75-105">Установите новую версию интерфейса командной строки Azure прямо сейчас!</span><span class="sxs-lookup"><span data-stu-id="8cc75-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="8cc75-106">Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="8cc75-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="8cc75-107">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="8cc75-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="8cc75-108">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8cc75-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="8cc75-109">При использовании модели управления службами Azure [установите Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="8cc75-109">If you are using the Azure Service Management (ASM) model, [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="8cc75-110"><a name="macOS"/>Установка в macOS</span><span class="sxs-lookup"><span data-stu-id="8cc75-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="8cc75-111">В macOS установку можно выполнить с помощью [Homebrew](https://brew.sh/) или вручную.</span><span class="sxs-lookup"><span data-stu-id="8cc75-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="8cc75-112">Установка с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cc75-112">Install with Homebrew</span></span>

1. <span data-ttu-id="8cc75-113">Если у вас нет этой программы, выполните [инструкции по установке Homebrew](https://docs.brew.sh/Installation.html).</span><span class="sxs-lookup"><span data-stu-id="8cc75-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="8cc75-114">Если CLI устанавливался вручную, следуйте инструкциям по [удалению вручную](#UninstallManually).</span><span class="sxs-lookup"><span data-stu-id="8cc75-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="8cc75-115">Обновите свои локальные репозитории Homebrew.</span><span class="sxs-lookup"><span data-stu-id="8cc75-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="8cc75-116">Установите пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="8cc75-117">Если вы ранее установили Azure CLI 1.0 с помощью Homebrew, вместо установки пакета можно получить CLI 2.0 при регулярном обновлении Homebrew.</span><span class="sxs-lookup"><span data-stu-id="8cc75-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="8cc75-118">Установка вручную</span><span class="sxs-lookup"><span data-stu-id="8cc75-118">Install manually</span></span>

1. <span data-ttu-id="8cc75-119">Установите Azure CLI 2.0 с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="8cc75-120">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

3. <span data-ttu-id="8cc75-121">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="8cc75-122">Установка в Windows</span><span class="sxs-lookup"><span data-stu-id="8cc75-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="8cc75-123">Установка с помощью MSI-файла для командной строки Windows</span><span class="sxs-lookup"><span data-stu-id="8cc75-123">Install with MSI for the Windows command-line</span></span>

<span data-ttu-id="8cc75-124">Чтобы установить CLI в Windows и использовать его в окне командной строки Windows, скачайте и запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows).</span><span class="sxs-lookup"><span data-stu-id="8cc75-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="8cc75-125">Установка с помощью apt-get для Bash на платформе Ubuntu в Windows</span><span class="sxs-lookup"><span data-stu-id="8cc75-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="8cc75-126">Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="8cc75-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="8cc75-127">Откройте оболочку Bash.</span><span class="sxs-lookup"><span data-stu-id="8cc75-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="8cc75-128">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="8cc75-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="8cc75-129">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="8cc75-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="8cc75-130">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-apt-package-manager"></a><span data-ttu-id="8cc75-131">Установка с помощью диспетчера пакетов apt</span><span class="sxs-lookup"><span data-stu-id="8cc75-131">Install with apt package manager</span></span>

<span data-ttu-id="8cc75-132">Для дистрибутивов с поддержкой диспетчера пакетов `apt`, например Ubuntu или Debian, можно установить Azure CLI 2.0, используя `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-132">For distributions using the `apt` package manager such as Ubuntu or Debian, you can install Azure CLI 2.0 via `apt-get`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="8cc75-133">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="8cc75-133">Modify your sources list:</span></span>

   - <span data-ttu-id="8cc75-134">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="8cc75-134">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="8cc75-135">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="8cc75-135">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="8cc75-136">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="8cc75-136">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="8cc75-137">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-137">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-yum-package-manager"></a><span data-ttu-id="8cc75-138">Установка с помощью диспетчера пакетов yum</span><span class="sxs-lookup"><span data-stu-id="8cc75-138">Install with yum package manager</span></span>

<span data-ttu-id="8cc75-139">Для дистрибутивов с поддержкой диспетчера пакетов `yum`, например Red Hat Enterprise Linux (RHEL), Fedora или CentOS, можно установить Azure CLI 2.0, используя `yum`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-139">For distributions which use the `yum` package manager such as Red Hat Enterprise Linux (RHEL), Fedora, or CentOS, you can install Azure CLI 2.0 via `yum`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="8cc75-140">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="8cc75-140">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="8cc75-141">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="8cc75-141">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="8cc75-142">Обновите индекс пакета `yum` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="8cc75-142">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="8cc75-143">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-143">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-zypper-package-manager"></a><span data-ttu-id="8cc75-144">Установка с помощью диспетчера пакетов zypper</span><span class="sxs-lookup"><span data-stu-id="8cc75-144">Install with zypper package manager</span></span>

<span data-ttu-id="8cc75-145">Для дистрибутивов с поддержкой диспетчера пакетов `zypper`, например OpenSUSE или SLE, можно установить Azure CLI 2.0, используя `zypper`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-145">For distributions which use the `zypper` package manager such as OpenSUSE or SLE, you can install Azure CLI 2.0 via `zypper`.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

1. <span data-ttu-id="8cc75-146">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="8cc75-146">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="8cc75-147">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="8cc75-147">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="8cc75-148">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="8cc75-148">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="8cc75-149">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-149">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="8cc75-150">Установка с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="8cc75-150">Install with Docker</span></span>

<span data-ttu-id="8cc75-151">Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="8cc75-151">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="8cc75-152">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-152">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="8cc75-153">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="8cc75-153">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="8cc75-154">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-154">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="8cc75-155">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-155">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-a-package-manager"></a><span data-ttu-id="8cc75-156"><a name="Linux"/>Установка в Linux без использования диспетчера пакетов</span><span class="sxs-lookup"><span data-stu-id="8cc75-156"><a name="Linux"/>Install on Linux without a package manager</span></span>

<span data-ttu-id="8cc75-157">Рекомендуется по возможности устанавливать CLI с помощью диспетчера пакетов (если вы знаете, как это сделать).</span><span class="sxs-lookup"><span data-stu-id="8cc75-157">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="8cc75-158">Если вы не хотите добавлять репозитории Майкрософт или работаете с дистрибутивами, которые не поддерживают указанный пакет, CLI можно установить вручную.</span><span class="sxs-lookup"><span data-stu-id="8cc75-158">If you do not want to add Microsoft's repositories, or are working with a distribution which does not have a provided package, you can manually install the CLI.</span></span>

1. <span data-ttu-id="8cc75-159">Установите необходимые компоненты с учетом дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="8cc75-159">Install the prerequisites based on your Linux distribution.</span></span>

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

<span data-ttu-id="8cc75-160">Если дистрибутив не указан в списке выше, вам нужно установить [Python 2.7 или более поздней версии](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) и [OpenSSL 1.0.2](https://www.openssl.org/source/).</span><span class="sxs-lookup"><span data-stu-id="8cc75-160">If your distribution is not listed above, you will need to install [Python 2.7 or later](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL 1.0.2](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="8cc75-161">Установите CLI с помощью команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-161">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="8cc75-162">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск оболочки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-162">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="8cc75-163">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-163">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="8cc75-164">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="8cc75-164">Troubleshooting</span></span>

<span data-ttu-id="8cc75-165">Если при установке CLI возникла проблема, ознакомьтесь с этим разделом, чтобы найти описание своего случая.</span><span class="sxs-lookup"><span data-stu-id="8cc75-165">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="8cc75-166">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8cc75-166">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="8cc75-167">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="8cc75-167">curl "Object Moved" error</span></span>

<span data-ttu-id="8cc75-168">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="8cc75-168">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="8cc75-169">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="8cc75-169">`az` command not found</span></span>

<span data-ttu-id="8cc75-170">Попробуйте очистить кэш хэша команд оболочки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-170">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="8cc75-171">Выполнить</span><span class="sxs-lookup"><span data-stu-id="8cc75-171">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="8cc75-172">и посмотрите, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="8cc75-172">and see if the problem is resolved.</span></span> <span data-ttu-id="8cc75-173">Кроме того, команда может отсутствовать в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-173">The command may also not be in your `$PATH`.</span></span> <span data-ttu-id="8cc75-174">Убедитесь, что `<install path>/bin` отображается в `$PATH` и при необходимости перезапустите оболочку.</span><span class="sxs-lookup"><span data-stu-id="8cc75-174">Make sure that `<install path>/bin` appears in your `$PATH`, and restart your shell if necessary.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="8cc75-175">Удаление версий CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="8cc75-175">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="8cc75-176">Если в системе установлена более ранняя версия CLI 1.x, вы можете удалить ее с учетом примененного типа установки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-176">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="8cc75-177">Удаление с помощью npm</span><span class="sxs-lookup"><span data-stu-id="8cc75-177">Uninstall with npm</span></span>

<span data-ttu-id="8cc75-178">Удалите устаревшую версию CLI с помощью команды `npm uninstall`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-178">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="8cc75-179">Удаление с помощью распространяемых компонентов</span><span class="sxs-lookup"><span data-stu-id="8cc75-179">Uninstall with distributable</span></span>

<span data-ttu-id="8cc75-180">Если установка выполнялась с использованием [установщика Azure CLI (MSI)](http://aka.ms/webpi-azure-cli) или [пакета macOS](http://aka.ms/mac-azure-cli), используйте то же средство для удаления файлов установки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-180">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="8cc75-181">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="8cc75-181">Uninstall with Docker</span></span>

<span data-ttu-id="8cc75-182">Если вы установили образ Docker, чтобы использовать более раннюю версию CLI, удалите этот образ и все связанные контейнеры.</span><span class="sxs-lookup"><span data-stu-id="8cc75-182">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="8cc75-183">Позже вы сможете повторно создать контейнеры, установив новый образ Docker, как описано в инструкциях по установке.</span><span class="sxs-lookup"><span data-stu-id="8cc75-183">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="8cc75-184">Обновление интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="8cc75-184">Update the CLI</span></span>

<span data-ttu-id="8cc75-185">Чтобы обновить Azure CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-185">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="8cc75-186">Обновление с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cc75-186">Update with Homebrew</span></span>

1. <span data-ttu-id="8cc75-187">Если установка выполнялась вручную, следуйте инструкциям по [установке с помощью Homebrew](#macOS).</span><span class="sxs-lookup"><span data-stu-id="8cc75-187">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="8cc75-188">Обновите свои данные в локальном репозитории Homebrew.</span><span class="sxs-lookup"><span data-stu-id="8cc75-188">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="8cc75-189">Обновите установленные пакеты.</span><span class="sxs-lookup"><span data-stu-id="8cc75-189">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="8cc75-190">Обновление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="8cc75-190">Update with MSI</span></span>

<span data-ttu-id="8cc75-191">Запустите [установщик Azure CLI (MSI)](https://aka.ms/InstallAzureCliWindows) еще раз.</span><span class="sxs-lookup"><span data-stu-id="8cc75-191">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt"></a><span data-ttu-id="8cc75-192">Обновление с помощью apt</span><span class="sxs-lookup"><span data-stu-id="8cc75-192">Update with apt</span></span>

<span data-ttu-id="8cc75-193">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="8cc75-193">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="8cc75-194">В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="8cc75-194">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="8cc75-195">Чтобы обновить только CLI, используйте команду `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-195">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-yum"></a><span data-ttu-id="8cc75-196">Обновление с помощью yum</span><span class="sxs-lookup"><span data-stu-id="8cc75-196">Update with yum</span></span>

<span data-ttu-id="8cc75-197">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-197">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

### <a name="update-with-zypper"></a><span data-ttu-id="8cc75-198">Обновление с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="8cc75-198">Update with zypper</span></span>

<span data-ttu-id="8cc75-199">Можно обновить пакет, воспользовавшись командой `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-199">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

### <a name="update-with-docker"></a><span data-ttu-id="8cc75-200">Обновление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="8cc75-200">Update with Docker</span></span>

1. <span data-ttu-id="8cc75-201">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-201">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="8cc75-202">Получите данные о контейнерах, которые используют образ CLI.</span><span class="sxs-lookup"><span data-stu-id="8cc75-202">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="8cc75-203">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="8cc75-203">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="8cc75-204">Остановите и заново создайте контейнеры.</span><span class="sxs-lookup"><span data-stu-id="8cc75-204">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="8cc75-205">Обновление вручную</span><span class="sxs-lookup"><span data-stu-id="8cc75-205">Update manually</span></span>

<span data-ttu-id="8cc75-206">Следуйте инструкциям по установке вручную для обновления в [macOS](#macOS) или [Linux](#Linux).</span><span class="sxs-lookup"><span data-stu-id="8cc75-206">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="8cc75-207">Удаление</span><span class="sxs-lookup"><span data-stu-id="8cc75-207">Uninstall</span></span>

<span data-ttu-id="8cc75-208">Нам будет очень жаль, если вы решите удалить CLI.</span><span class="sxs-lookup"><span data-stu-id="8cc75-208">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="8cc75-209">Чтобы удалить CLI, используйте тот же метод, что и для установки.</span><span class="sxs-lookup"><span data-stu-id="8cc75-209">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="8cc75-210">Удаление с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="8cc75-210">Uninstall with Homebrew</span></span>

<span data-ttu-id="8cc75-211">Удалите пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-211">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="8cc75-212">Удаление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="8cc75-212">Uninstall with MSI</span></span>

<span data-ttu-id="8cc75-213">Запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".</span><span class="sxs-lookup"><span data-stu-id="8cc75-213">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt"></a><span data-ttu-id="8cc75-214">Удаление с помощью apt</span><span class="sxs-lookup"><span data-stu-id="8cc75-214">Uninstall with apt</span></span>

<span data-ttu-id="8cc75-215">Выполните удаление с помощью `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-215">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-yum"></a><span data-ttu-id="8cc75-216">Удаление с помощью yum</span><span class="sxs-lookup"><span data-stu-id="8cc75-216">Uninstall with yum</span></span>

1. <span data-ttu-id="8cc75-217">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="8cc75-217">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="8cc75-218">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="8cc75-218">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="8cc75-219">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="8cc75-219">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-zypper"></a><span data-ttu-id="8cc75-220">Удаление с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="8cc75-220">Uninstall with zypper</span></span>

1. <span data-ttu-id="8cc75-221">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="8cc75-221">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="8cc75-222">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="8cc75-222">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="8cc75-223">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="8cc75-223">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="8cc75-224">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="8cc75-224">Uninstall with Docker</span></span>

<span data-ttu-id="8cc75-225">Если вы установили образ Docker, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.</span><span class="sxs-lookup"><span data-stu-id="8cc75-225">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="8cc75-226">Получите данные о контейнерах, на которых запущен образ azure-cli.</span><span class="sxs-lookup"><span data-stu-id="8cc75-226">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="8cc75-227">Удалите все контейнеры с образом CLI.</span><span class="sxs-lookup"><span data-stu-id="8cc75-227">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="8cc75-228">Удалите локально установленный образ CLI.</span><span class="sxs-lookup"><span data-stu-id="8cc75-228">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="8cc75-229">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="8cc75-229">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="8cc75-230"><a name="UninstallManually"/>Удаление вручную</span><span class="sxs-lookup"><span data-stu-id="8cc75-230"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="8cc75-231">Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="8cc75-231">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="8cc75-232">Удалите установленные файлы.</span><span class="sxs-lookup"><span data-stu-id="8cc75-232">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="8cc75-233">Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-233">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

3. <span data-ttu-id="8cc75-234">Если оболочка использует кэш команд, перезагрузите его.</span><span class="sxs-lookup"><span data-stu-id="8cc75-234">If your shell uses a command cache, reload it.</span></span>

   ```bash
   hash -r
   ```

> [!Note]
> <span data-ttu-id="8cc75-235">Каталог установки по умолчанию — `/Users/<username>` для macOS и `/home/<username>` для Linux.</span><span class="sxs-lookup"><span data-stu-id="8cc75-235">The default install location is `/Users/<username>` for macOS and `/home/<username>` for Linux.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="8cc75-236">Создание отчетов о проблемах CLI и обратная связь</span><span class="sxs-lookup"><span data-stu-id="8cc75-236">Report CLI issues and feedback</span></span>

<span data-ttu-id="8cc75-237">Если при работе со средством возникают ошибки, сообщите об этом в разделе репозитория GitHub, посвященном [проблемам](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="8cc75-237">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="8cc75-238">Чтобы отправить отзыв из командной строки, используйте команду `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8cc75-238">To provide feedback from the command line, use the `az feedback` command.</span></span>
