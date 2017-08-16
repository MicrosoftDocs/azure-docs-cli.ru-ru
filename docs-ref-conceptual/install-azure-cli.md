---
title: "Установка Azure CLI 2.0"
description: "Справочная документация по Azure CLI 2.0"
keywords: "Azure CLI 2.0, справочник по Azure CLI 2.0, установка Azure CLI 2.0, Azure Python CLI, удаление Azure CLI 2.0"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 7065ed5270ef9bfc70beea81d0bc442a7b4df38c
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="bf147-104">Установка Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="bf147-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="bf147-105">Установите новую версию интерфейса командной строки Azure прямо сейчас!</span><span class="sxs-lookup"><span data-stu-id="bf147-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="bf147-106">Мы усовершенствовали и обновили его, предоставив удобный встроенный интерфейс командной строки для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="bf147-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="bf147-107">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="bf147-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="bf147-108">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="bf147-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="bf147-109">Если вам нужна предыдущая версия Azure CLI, см. статью [Установка Azure CLI 1.0](/azure/cli-install-nodejs).</span><span class="sxs-lookup"><span data-stu-id="bf147-109">If you need the previous version of the Azure CLI, here's how to [install Azure 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="macos"></a><span data-ttu-id="bf147-110">macOS</span><span class="sxs-lookup"><span data-stu-id="bf147-110">macOS</span></span>

1. <span data-ttu-id="bf147-111">Azure CLI 2.0 можно установить с помощью одной команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="bf147-111">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="bf147-112">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.</span><span class="sxs-lookup"><span data-stu-id="bf147-112">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="bf147-113">Запустите Azure CLI 2.0 из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="bf147-113">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bf147-114">При установке с помощью InstallAzureCli `az component update` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf147-114">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="bf147-115">Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.</span><span class="sxs-lookup"><span data-stu-id="bf147-115">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bf147-116">Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bf147-116">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="windows"></a><span data-ttu-id="bf147-117">Windows</span><span class="sxs-lookup"><span data-stu-id="bf147-117">Windows</span></span>

<span data-ttu-id="bf147-118">Интерфейс командной строки можно установить с помощью MSI-файла и использовать его в командной строке Windows или установить его на платформе Ubuntu в Windows с помощью apt-get для Bash.</span><span class="sxs-lookup"><span data-stu-id="bf147-118">You can install the CLI with the MSI and use it in the Windows command-line, or you can install the CLI with apt-get on Bash on Ubuntu on Windows.</span></span>

### <a name="msi-for-the-windows-command-line"></a><span data-ttu-id="bf147-119">MSI-файл для командной строки Windows</span><span class="sxs-lookup"><span data-stu-id="bf147-119">MSI for the Windows command-line</span></span> 

<span data-ttu-id="bf147-120">Чтобы установить интерфейс командной строки в Windows и использовать его в окне командной строке Windows, скачайте и запустите соответствующий [MSI](https://aka.ms/InstallAzureCliWindows)-файл.</span><span class="sxs-lookup"><span data-stu-id="bf147-120">To install the CLI on Windows and use it in the Windows command-line, download and run the [msi](https://aka.ms/InstallAzureCliWindows).</span></span>

> [!NOTE]
> <span data-ttu-id="bf147-121">При установке с помощью MSI-файла `az component` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf147-121">When you install with the msi, `az component` isn't supported.</span></span>
> <span data-ttu-id="bf147-122">Для обновления до последней версии интерфейса командной строки запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз.</span><span class="sxs-lookup"><span data-stu-id="bf147-122">To update to the latest CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again.</span></span>
> 
> <span data-ttu-id="bf147-123">Чтобы удалить интерфейс командной строки, запустите [MSI](https://aka.ms/InstallAzureCliWindows)-файл еще раз и щелкните "Удалить".</span><span class="sxs-lookup"><span data-stu-id="bf147-123">To uninstall the CLI, run the [msi](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="bf147-124">apt-get для Bash на платформе Ubuntu в Windows</span><span class="sxs-lookup"><span data-stu-id="bf147-124">apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="bf147-125">Если у вас не установлена командная оболочка Bash в Windows, [установите ее](https://msdn.microsoft.com/commandline/wsl/install_guide).</span><span class="sxs-lookup"><span data-stu-id="bf147-125">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="bf147-126">Откройте оболочку Bash.</span><span class="sxs-lookup"><span data-stu-id="bf147-126">Open the Bash shell.</span></span>

3. <span data-ttu-id="bf147-127">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="bf147-127">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="bf147-128">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="bf147-128">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="bf147-129">При установке с помощью apt-get `az component` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf147-129">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="bf147-130">Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.</span><span class="sxs-lookup"><span data-stu-id="bf147-130">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bf147-131">Для удаления выполните команду `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bf147-131">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux"></a><span data-ttu-id="bf147-132">Linux</span><span class="sxs-lookup"><span data-stu-id="bf147-132">Linux</span></span>

1. <span data-ttu-id="bf147-133">В Linux может потребоваться установить определенные [необходимые компоненты](#linux-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="bf147-133">On Linux, you may need to install specific [prerequisites](#linux-prerequisites).</span></span>

2. <span data-ttu-id="bf147-134">Azure CLI 2.0 можно установить с помощью одной команды `curl`.</span><span class="sxs-lookup"><span data-stu-id="bf147-134">Install Azure CLI 2.0 with one `curl` command.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="bf147-135">Чтобы некоторые изменения вступили в силу, может потребоваться перезапуск командной оболочки.</span><span class="sxs-lookup"><span data-stu-id="bf147-135">You may have to restart your command shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="bf147-136">Запустите Azure CLI 2.0 из командной строки с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="bf147-136">Run Azure CLI 2.0 from the command prompt with the `az` command.</span></span>

> [!Note]
> <span data-ttu-id="bf147-137">При установке с помощью InstallAzureCli `az component update` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf147-137">When you install with InstallAzureCli, `az component update` isn't supported.</span></span>
> <span data-ttu-id="bf147-138">Для обновления до последней версии интерфейса командной строки выполните команду `curl -L https://aka.ms/InstallAzureCli | bash` еще раз.</span><span class="sxs-lookup"><span data-stu-id="bf147-138">To update to the latest CLI, run `curl -L https://aka.ms/InstallAzureCli | bash` again.</span></span>
> 
> <span data-ttu-id="bf147-139">Чтобы удалить интерфейс командной строки, см. раздел [по удалению программ вручную](#uninstall).</span><span class="sxs-lookup"><span data-stu-id="bf147-139">To uninstall, see the [manual uninstall instructions](#uninstall).</span></span>

## <a name="docker"></a><span data-ttu-id="bf147-140">Docker</span><span class="sxs-lookup"><span data-stu-id="bf147-140">Docker</span></span>

<span data-ttu-id="bf147-141">Мы поддерживаем образ Docker, предварительно настроенный с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="bf147-141">We maintain a Docker image preconfigured with the Azure CLI.</span></span>

<span data-ttu-id="bf147-142">Установите Azure CLI с помощью `docker run`.</span><span class="sxs-lookup"><span data-stu-id="bf147-142">Install the Azure CLI using `docker run`.</span></span>

```bash
docker run azuresdk/azure-cli-python:<version>
```

<span data-ttu-id="bf147-143">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/).</span><span class="sxs-lookup"><span data-stu-id="bf147-143">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

> [!NOTE]
> <span data-ttu-id="bf147-144">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="bf147-144">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>
>
> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

> [!NOTE]
> <span data-ttu-id="bf147-145">Образ Docker не поддерживает [ функцию `component`](/cli/azure/component).</span><span class="sxs-lookup"><span data-stu-id="bf147-145">The Docker image does not support the [`component` feature](/cli/azure/component).</span></span>
> <span data-ttu-id="bf147-146">Чтобы обновить Azure CLI 2.0, используйте `docker run` для установки последней версии образа или выбранного вами определенного образа.</span><span class="sxs-lookup"><span data-stu-id="bf147-146">To update the Azure CLI 2.0, use `docker run` to install the latest image, or the specific image that you want.</span></span>

## <a name="apt-get"></a><span data-ttu-id="bf147-147">apt-get</span><span class="sxs-lookup"><span data-stu-id="bf147-147">apt-get</span></span>

<span data-ttu-id="bf147-148">В системах на базе Debian и Ubuntu можно установить Azure CLI 2.0 с помощью `apt-get`.</span><span class="sxs-lookup"><span data-stu-id="bf147-148">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="bf147-149">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="bf147-149">Modify your sources list.</span></span>

   - <span data-ttu-id="bf147-150">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="bf147-150">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="bf147-151">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="bf147-151">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="bf147-152">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="bf147-152">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="bf147-153">При установке с помощью apt-get `az component` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf147-153">When you install with apt-get, `az component` isn't supported.</span></span>
> <span data-ttu-id="bf147-154">Чтобы обновить интерфейс командной строки, выполните `sudo apt-get update && sudo apt-get install azure-cli` еще раз.</span><span class="sxs-lookup"><span data-stu-id="bf147-154">To update the CLI, run `sudo apt-get update && sudo apt-get install azure-cli` again.</span></span>
> 
> <span data-ttu-id="bf147-155">Для удаления выполните команду `sudo apt-get remove azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="bf147-155">To uninstall, run `sudo apt-get remove azure-cli`.</span></span>

## <a name="linux-prerequisites"></a><span data-ttu-id="bf147-156">Предварительные требования для Linux</span><span class="sxs-lookup"><span data-stu-id="bf147-156">Linux Prerequisites</span></span>

1. <span data-ttu-id="bf147-157">Если у вас не установлен язык [Python](https://www.python.org/downloads), установите его.</span><span class="sxs-lookup"><span data-stu-id="bf147-157">If you don't have it, install [Python](https://www.python.org/downloads).</span></span>

2. <span data-ttu-id="bf147-158">В зависимости от дистрибутива Linux установите необходимые компоненты.</span><span class="sxs-lookup"><span data-stu-id="bf147-158">Depending on your Linux distribution, install the prerequisites.</span></span>

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

## <a name="troubleshooting"></a><span data-ttu-id="bf147-159">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="bf147-159">Troubleshooting</span></span>

### <a name="errors-with-curl-redirection"></a><span data-ttu-id="bf147-160">Ошибки, связанные с перенаправлением curl</span><span class="sxs-lookup"><span data-stu-id="bf147-160">Errors with curl redirection</span></span>

<span data-ttu-id="bf147-161">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса aka.ms:</span><span class="sxs-lookup"><span data-stu-id="bf147-161">If you get an error from the `curl` command regarding the `-L` parameter, or an error saying "Object Moved", try using the full url instead of the aka.ms url:</span></span>

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

## <a name="uninstall"></a><span data-ttu-id="bf147-162">Удаление</span><span class="sxs-lookup"><span data-stu-id="bf147-162">Uninstall</span></span>

<span data-ttu-id="bf147-163">Если для установки интерфейса командной строки использовался скрипт со страницы https://aka.ms/InstallAzureCli, для удаления можно выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="bf147-163">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="bf147-164">Удалите установленные файлы.</span><span class="sxs-lookup"><span data-stu-id="bf147-164">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="bf147-165">Удалите строку `<install location>/lib/azure-cli/az.completion` из `<install location>/.bash_profile`.</span><span class="sxs-lookup"><span data-stu-id="bf147-165">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="bf147-166">Расположение установки по умолчанию — `/Users/<username>`.</span><span class="sxs-lookup"><span data-stu-id="bf147-166">The default install location is `/Users/<username>`.</span></span>

<span data-ttu-id="bf147-167">Если вы использовали apt-get, Docker или MSI-файл для установки интерфейса командной строки, используйте тот же инструмент для его удаления.</span><span class="sxs-lookup"><span data-stu-id="bf147-167">If you used apt-get, Docker, or the msi to install the CLI, use the same tool to uninstall it.</span></span>

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="bf147-168">Создание отчетов о проблемах и обратная связь</span><span class="sxs-lookup"><span data-stu-id="bf147-168">Reporting issues and feedback</span></span>

<span data-ttu-id="bf147-169">При появлении ошибок в средстве сообщите о проблеме в разделе [Проблемы](https://github.com/Azure/azure-cli/issues) репозитория GitHub.</span><span class="sxs-lookup"><span data-stu-id="bf147-169">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repo.</span></span>
<span data-ttu-id="bf147-170">Чтобы отправить отзыв из командной строки, попробуйте использовать команду `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bf147-170">To provide feedback from the command line, try the `az feedback` command.</span></span>
