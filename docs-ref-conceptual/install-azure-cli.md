---
title: "Установка Azure CLI 2.0"
description: "Справочные документы для установки Azure CLI 2.0"
keywords: "Azure CLI 2.0, справочник по Azure CLI 2.0, установка Azure CLI 2.0, Azure Python CLI, удаление Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 08/17/2017
ms.topic: "articleå"
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 432edac070e238a6f1be0ccd76b9b3582b082219
ms.sourcegitcommit: 2ec80224c6b831e31038b710d912c0dbb1ddfef6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="00a35-104">Установка Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="00a35-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="00a35-105">Установите новую версию интерфейса командной строки Azure прямо сейчас!</span><span class="sxs-lookup"><span data-stu-id="00a35-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="00a35-106">Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="00a35-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="00a35-107">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="00a35-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="00a35-108">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="00a35-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-109">Если вам нужна предыдущая версия Azure CLI, см. руководство по [установке Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="00a35-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="00a35-110">macOS</span><span class="sxs-lookup"><span data-stu-id="00a35-110">macOS</span></span>

> [!WARNING]
> <span data-ttu-id="00a35-111">Формула Homebrew для Azure CLI (`azure-cli`) сейчас устарела и будет устанавливать предыдущую версию.</span><span class="sxs-lookup"><span data-stu-id="00a35-111">The Homebrew formula for the Azure CLI, `azure-cli`, is currently out of date and will install a previous version.</span></span>

1. <span data-ttu-id="00a35-112">Azure CLI 2.0 можно установить с помощью одной команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="00a35-112">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="00a35-113">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.</span><span class="sxs-lookup"><span data-stu-id="00a35-113">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="00a35-114">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="00a35-114">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="00a35-115">При установке с помощью InstallAzureCli [`az component update`](/cli/azure/component#update) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a35-115">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="00a35-116">Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.</span><span class="sxs-lookup"><span data-stu-id="00a35-116">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="00a35-117">Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="00a35-117">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="00a35-118">Windows</span><span class="sxs-lookup"><span data-stu-id="00a35-118">Windows</span></span>

<span data-ttu-id="00a35-119">Azure CLI 2.0 можно установить с помощью MSI-файла, чтобы использовать в командной строке Windows, или с помощью apt-get для Bash, чтобы использовать на платформе Ubuntu в Windows.</span><span class="sxs-lookup"><span data-stu-id="00a35-119">You can install Azure CLI 2.0 with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="00a35-120">MSI-файл для командной строки Windows</span><span class="sxs-lookup"><span data-stu-id="00a35-120">MSI for the Windows command-line</span></span> 

<span data-ttu-id="00a35-121">Чтобы установить интерфейс командной строки в Windows и использовать его в окне командной строке Windows, скачайте и запустите соответствующий [MSI](https://aka.ms/InstallAzureCliWindows)-файл.</span><span class="sxs-lookup"><span data-stu-id="00a35-121">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-122">При установке с помощью MSI-файла [`az component`](/cli/azure/component) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a35-122">When you install with the msi, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="00a35-123">Для обновления до последней версии интерфейса командной строки запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз.</span><span class="sxs-lookup"><span data-stu-id="00a35-123">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="00a35-124">Чтобы удалить интерфейс командной строки, запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".</span><span class="sxs-lookup"><span data-stu-id="00a35-124">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="00a35-125">apt-get для Bash на платформе Ubuntu в Windows</span><span class="sxs-lookup"><span data-stu-id="00a35-125">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="00a35-126">Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="00a35-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="00a35-127">Откройте оболочку Bash.</span><span class="sxs-lookup"><span data-stu-id="00a35-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="00a35-128">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="00a35-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="00a35-129">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="00a35-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="00a35-130">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="00a35-130">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-131">При установке с помощью apt-get [`az component`](/cli/azure/component) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a35-131">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="00a35-132">Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.</span><span class="sxs-lookup"><span data-stu-id="00a35-132">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="00a35-133">Для удаления выполните команду `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="00a35-133">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="apt-get-for-debianubuntu"></a><span data-ttu-id="00a35-134">apt-get для Debian и Ubuntu</span><span class="sxs-lookup"><span data-stu-id="00a35-134">apt-get for Debian/Ubuntu</span></span>

<span data-ttu-id="00a35-135">В системах на базе Debian и Ubuntu можно установить Azure CLI 2.0 с помощью `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="00a35-135">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="00a35-136">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="00a35-136">Modify your sources list.</span></span>
 
   - <span data-ttu-id="00a35-137">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="00a35-137">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="00a35-138">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="00a35-138">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="00a35-139">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="00a35-139">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="00a35-140">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="00a35-140">Run the CLI from the command prompt with the `az` command.</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-141">При установке с помощью apt-get [`az component`](/cli/azure/component) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a35-141">When you install with apt-get, [`az component`](/cli/azure/component) isn't supported.</span></span>
> <span data-ttu-id="00a35-142">Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.</span><span class="sxs-lookup"><span data-stu-id="00a35-142">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="00a35-143">Для удаления выполните команду `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="00a35-143">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="docker"></a><span data-ttu-id="00a35-144">Docker</span><span class="sxs-lookup"><span data-stu-id="00a35-144">Docker</span></span>

<span data-ttu-id="00a35-145">Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="00a35-145">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="00a35-146">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="00a35-146">Install the CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="00a35-147">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="00a35-147">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-148">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="00a35-148">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

>> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

<span data-ttu-id="00a35-149">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="00a35-149">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="00a35-150">Образ Docker не поддерживает функцию [`az component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="00a35-150">The Docker image does not support the [`az component`](/cli/azure/component) feature.</span></span>
> <span data-ttu-id="00a35-151">Чтобы обновить Azure CLI 2.0, используйте `docker run` для установки последней версии образа или выбранного вами определенного образа.</span><span class="sxs-lookup"><span data-stu-id="00a35-151">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="linux"></a><span data-ttu-id="00a35-152">Linux</span><span class="sxs-lookup"><span data-stu-id="00a35-152">Linux</span></span>

1. <span data-ttu-id="00a35-153">Если у вас не установлен язык [Python](https://www.python.org/downloads), установите его.</span><span class="sxs-lookup"><span data-stu-id="00a35-153">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="00a35-154">В зависимости от дистрибутива Linux установите необходимые компоненты.</span><span class="sxs-lookup"><span data-stu-id="00a35-154">Depending on your Linux distribution, install the prerequisites.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install gcc libffi-devel python-devel openssl-devel
   ```

3. <span data-ttu-id="00a35-155">Установите CLI с помощью одной команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="00a35-155">Install the CLI with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

4. <span data-ttu-id="00a35-156">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.</span><span class="sxs-lookup"><span data-stu-id="00a35-156">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

5. <span data-ttu-id="00a35-157">Запустите CLI из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="00a35-157">Run the CLI from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="00a35-158">При установке с помощью InstallAzureCli [`az component update`](/cli/azure/component#update) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a35-158">When you install with InstallAzureCli, [`az component update`](/cli/azure/component#update) isn't supported.</span></span>
> <span data-ttu-id="00a35-159">Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.</span><span class="sxs-lookup"><span data-stu-id="00a35-159">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="00a35-160">Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="00a35-160">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="00a35-161">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="00a35-161">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="00a35-162">Ошибки, связанные с перенаправлением curl</span><span class="sxs-lookup"><span data-stu-id="00a35-162">Errors with curl redirection</span></span>

<span data-ttu-id="00a35-163">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса aka.ms:</span><span class="sxs-lookup"><span data-stu-id="00a35-163">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

```
# If you see this:
curl -L https://aka.ms/InstallAzureCli | bash
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   175  100   175    0     0    562      0 --:--:-- --:--:-- --:--:--   560
bash: line 1: syntax error near unexpected token `<'
'ash: line 1: `<html><head><title>Object moved</title></head><body>

#### Try this instead:
curl https://azurecliprod.blob.core.windows.net/install | bash
```

## <a name="uninstall"></a><span data-ttu-id="00a35-164">Удаление</span><span class="sxs-lookup"><span data-stu-id="00a35-164">Uninstall</span></span>

<span data-ttu-id="00a35-165">Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="00a35-165">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="00a35-166">Удалите установленные файлы.</span><span class="sxs-lookup"><span data-stu-id="00a35-166">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="00a35-167">Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="00a35-167">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="00a35-168">Расположение установки по умолчанию — `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="00a35-168">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="00a35-169">Если вы использовали apt-get, Docker или MSI-файл для установки интерфейса командной строки, используйте тот же инструмент для его удаления.</span><span class="sxs-lookup"><span data-stu-id="00a35-169">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="00a35-170">Создание отчетов о проблемах и обратная связь</span><span class="sxs-lookup"><span data-stu-id="00a35-170">Reporting issues and feedback</span></span>

<span data-ttu-id="00a35-171">При появлении ошибок в средстве сообщите о проблеме в разделе [Проблемы](https://github.com/Azure/azure-cli/issues) репозитория GitHub.</span><span class="sxs-lookup"><span data-stu-id="00a35-171">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="00a35-172">Чтобы отправить отзыв из командной строки, попробуйте использовать команду `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="00a35-172">To provide feedback from the command line, try the `az feedback` command.</span></span>
