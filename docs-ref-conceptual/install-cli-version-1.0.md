---
title: Установка Azure CLI 1.0
description: Установка Azure CLI 1.0 на компьютерах Mac OS, Linux и Windows и начало работы со службами Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dd2d8658819c03742ae65c639717837ca940659e
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388615"
---
# <a name="install-the-azure-cli-10"></a><span data-ttu-id="15ffb-103">Установка Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="15ffb-103">Install the Azure CLI 1.0</span></span>

> [!IMPORTANT]
> <span data-ttu-id="15ffb-104">В этом разделе описана установка Azure CLI 1.0.</span><span class="sxs-lookup"><span data-stu-id="15ffb-104">This topic describes how to install the Azure CLI 1.0.</span></span> <span data-ttu-id="15ffb-105">Это нерекомендуемый CLI, и его можно использовать только для поддержки с моделью управления службами Azure (ASM) с "классическими" ресурсами.</span><span class="sxs-lookup"><span data-stu-id="15ffb-105">This CLI is deprecated and should only be used for support with the Azure Service Management (ASM) model with "classic" resources.</span></span>
> <span data-ttu-id="15ffb-106">Для развертываний Azure Resource Manager используйте [Azure CLI 2.0](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="15ffb-106">For Azure Resource Manager deployments, use [Azure CLI 2.0](/cli/azure).</span></span>

<span data-ttu-id="15ffb-107">Вы можете выполнить быструю установку интерфейса командной строки Azure (Azure CLI 1.0), чтобы использовать набор консольных команд с открытым кодом для управления ресурсами в среде Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="15ffb-107">Quickly install the Azure Command-Line Interface (Azure CLI 1.0) to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="15ffb-108">Существует несколько вариантов установки этих кроссплатформенных инструментов на компьютер.</span><span class="sxs-lookup"><span data-stu-id="15ffb-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="15ffb-109">**Пакет npm**. Запустите npm (диспетчер пакетов для JavaScript), чтобы установить последнюю версию пакета для Azure CLI 1.0 в дистрибутиве или ОС Linux.</span><span class="sxs-lookup"><span data-stu-id="15ffb-109">**npm package** - Run npm (the package manager for JavaScript) to install the latest Azure CLI 1.0 package on your Linux distribution or OS.</span></span> <span data-ttu-id="15ffb-110">На компьютере должны быть установлены node.js и npm.</span><span class="sxs-lookup"><span data-stu-id="15ffb-110">Requires node.js and npm on your computer.</span></span>
* <span data-ttu-id="15ffb-111">**Установщик**. Скачайте установщик, чтобы легко установить эти инструменты на компьютеры Mac или Windows.</span><span class="sxs-lookup"><span data-stu-id="15ffb-111">**Installer** - Download an installer for easy installation on Mac or Windows.</span></span>
* <span data-ttu-id="15ffb-112">**Контейнер Docker**. Приступите к использованию последней версии интерфейса командной строки из готового контейнера Docker.</span><span class="sxs-lookup"><span data-stu-id="15ffb-112">**Docker container** - Start using the latest CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="15ffb-113">На компьютере требуется наличие узла Docker.</span><span class="sxs-lookup"><span data-stu-id="15ffb-113">Requires Docker host on your computer.</span></span>

<span data-ttu-id="15ffb-114">Дополнительные сведения и варианты установки см. в репозитории проектов на сайте [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="15ffb-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="15ffb-115">После установки Azure CLI 1.0 вы сможете [подключить его к своей подписке Azure](/cli/azure/authenticate-azure-cli) и работать с ресурсами Azure c помощью команд **azure** из интерфейса командной строки (Bash, терминала, командной строки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="15ffb-115">Once the Azure CLI 1.0 is installed, [connect it with your Azure subscription](/cli/azure/authenticate-azure-cli) and run the **azure** commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="15ffb-116">Вариант 1. Установка пакета npm</span><span class="sxs-lookup"><span data-stu-id="15ffb-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="15ffb-117">Для установки интерфейса командной строки из пакета NPM в системе должна быть установлена [последняя версия Node.js и npm](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="15ffb-117">To install the CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="15ffb-118">Затем запустите **npm install** для установки пакета azure-cli:</span><span class="sxs-lookup"><span data-stu-id="15ffb-118">Then, run **npm install** to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="15ffb-119">В системах Linux для выполнения команды **npm** может потребоваться команда **sudo**:</span><span class="sxs-lookup"><span data-stu-id="15ffb-119">On Linux distributions, you might need to use **sudo** to successfully run the **npm** command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="15ffb-120">Если необходимо установить или обновить Node.js и npm в дистрибутиве или ОС Linux, рекомендуется установить последнюю версию Node.js LTS (4.x).</span><span class="sxs-lookup"><span data-stu-id="15ffb-120">If you need to install or update Node.js and npm on your Linux distribution or OS, we recommend that you install the most recent Node.js LTS version (4.x).</span></span> <span data-ttu-id="15ffb-121">Если вы используете более раннюю версию, возможны ошибки при установке.</span><span class="sxs-lookup"><span data-stu-id="15ffb-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="15ffb-122">Если хотите, скачайте последнюю версию [TAR-файла][linux-installer] пакета npm для Linux на локальный компьютер.</span><span class="sxs-lookup"><span data-stu-id="15ffb-122">If you prefer, download the latest Linux [tar file][linux-installer] for the npm package locally.</span></span> <span data-ttu-id="15ffb-123">Затем установите скачанный пакет npm, как описано ниже (для дистрибутивов Linux может потребоваться использовать **sudo**).</span><span class="sxs-lookup"><span data-stu-id="15ffb-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use **sudo**):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="15ffb-124">Вариант 2. Использование установщика</span><span class="sxs-lookup"><span data-stu-id="15ffb-124">Option 2: Use an installer</span></span>

<span data-ttu-id="15ffb-125">При использовании компьютера Windows или Mac можно скачать следующие установщики интерфейса командной строки:</span><span class="sxs-lookup"><span data-stu-id="15ffb-125">If you use a Mac or Windows computer, the following CLI installers are available for download:</span></span>

* <span data-ttu-id="15ffb-126">[Установщик Mac OS X][mac-installer]</span><span class="sxs-lookup"><span data-stu-id="15ffb-126">[Mac OS X installer][mac-installer]</span></span>
* <span data-ttu-id="15ffb-127">[MSI-файл Windows][windows-installer]</span><span class="sxs-lookup"><span data-stu-id="15ffb-127">[Windows MSI][windows-installer]</span></span>

> [!TIP]
> <span data-ttu-id="15ffb-128">В Windows для установки интерфейса командной строки можно также скачать [установщик веб-платформы](https://go.microsoft.com/?linkid=9828653) .</span><span class="sxs-lookup"><span data-stu-id="15ffb-128">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the CLI.</span></span> <span data-ttu-id="15ffb-129">Этот установщик дает возможность установить дополнительный пакет SDK для Azure и программы командной строки после установки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="15ffb-129">This installer gives you the option to install additional Azure SDK and command-line tools after installing the CLI.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="15ffb-130">Вариант 3. Использование контейнера Docker</span><span class="sxs-lookup"><span data-stu-id="15ffb-130">Option 3: Use a Docker container</span></span>

<span data-ttu-id="15ffb-131">Если вы настроили компьютер в качестве узла [Docker](https://docs.docker.com/engine/understanding-docker/), то можете запустить последнюю версию Azure CLI 1.0 в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="15ffb-131">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the latest Azure CLI 1.0 in a Docker container.</span></span> <span data-ttu-id="15ffb-132">Выполните команду (в дистрибутивах Linux может потребоваться использование **sudo**):</span><span class="sxs-lookup"><span data-stu-id="15ffb-132">Run the command (on Linux distributions you might need to use **sudo**):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a><span data-ttu-id="15ffb-133">Выполнение команд Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="15ffb-133">Run Azure CLI 1.0 commands</span></span>

<span data-ttu-id="15ffb-134">После установки Azure CLI 1.0 выполните команду **azure** в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="15ffb-134">After the Azure CLI 1.0 is installed, run the **azure** command from your command-line user interface.</span></span> <span data-ttu-id="15ffb-135">Например, выполните команду help:</span><span class="sxs-lookup"><span data-stu-id="15ffb-135">For example, to run the help command:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="15ffb-136">Для некоторых дистрибутивов Linux может появиться сообщение об ошибке `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="15ffb-136">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="15ffb-137">Это связано с тем, что новые установки Node.js размещаются в папке /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="15ffb-137">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="15ffb-138">Для устранения этой ошибки создайте символьную ссылку /usr/bin/node, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="15ffb-138">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="15ffb-139">Чтобы просмотреть версию установленного пакета Azure CLI 1.0, введите следующую команду:</span><span class="sxs-lookup"><span data-stu-id="15ffb-139">To see the version of the Azure CLI 1.0 you installed, type the command:</span></span>

```azurecli
azure --version
```

<span data-ttu-id="15ffb-140">Для доступа ко всем командам CLI [подключитесь к своей подписке Azure из Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="15ffb-140">To access all the CLI commands, [connect to your Azure subscription from the Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="15ffb-141">При первом использовании Azure CLI появится сообщение с вопросом, следует ли разрешить корпорации Майкрософт собирать сведения об использовании.</span><span class="sxs-lookup"><span data-stu-id="15ffb-141">When you first use Azure CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="15ffb-142">Участие является добровольным.</span><span class="sxs-lookup"><span data-stu-id="15ffb-142">Participation is voluntary.</span></span> <span data-ttu-id="15ffb-143">Если вы согласились участвовать в этой программе, сбор сведений можно остановить в любой момент, выполнив команду `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="15ffb-143">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="15ffb-144">Чтобы включить участие в любой момент, выполните команду `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="15ffb-144">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-cli"></a><span data-ttu-id="15ffb-145">Обновление интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="15ffb-145">Update the CLI</span></span>

<span data-ttu-id="15ffb-146">Корпорация Майкрософт часто выпускает обновленные версии Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="15ffb-146">Microsoft frequently releases updated versions of the Azure CLI.</span></span> <span data-ttu-id="15ffb-147">Переустановите интерфейс командной строки с помощью установщика для соответствующей операционной системы или запустите актуальную версию контейнера Docker.</span><span class="sxs-lookup"><span data-stu-id="15ffb-147">Reinstall the CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="15ffb-148">Если вы установили последние версии Node.js и NPM, введите следующую команду (в системах Linux может потребоваться использовать режим **sudo**).</span><span class="sxs-lookup"><span data-stu-id="15ffb-148">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use **sudo**).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="15ffb-149">Включение выполнения нажатием клавиши TAB</span><span class="sxs-lookup"><span data-stu-id="15ffb-149">Enable tab completion</span></span>

<span data-ttu-id="15ffb-150">Выполнение команд интерфейса командной строки нажатием клавиши TAB поддерживается на компьютерах MAC и Linux.</span><span class="sxs-lookup"><span data-stu-id="15ffb-150">Tab completion of CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="15ffb-151">Чтобы включить эту функцию в zsh, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="15ffb-151">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="15ffb-152">Чтобы включить эту функцию в bash, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="15ffb-152">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="15ffb-153">Дополнительная информация</span><span class="sxs-lookup"><span data-stu-id="15ffb-153">Next steps</span></span>

* <span data-ttu-id="15ffb-154">[Подключитесь к подписке Azure из интерфейса командной строки](/cli/azure/authenticate-azure-cli) для создания ресурсов Azure и управления ими.</span><span class="sxs-lookup"><span data-stu-id="15ffb-154">[Connect from the CLI to your Azure subscription](/cli/azure/authenticate-azure-cli) to create and manage Azure resources.</span></span>
* <span data-ttu-id="15ffb-155">Для того чтобы получить дополнительные сведения об интерфейсе командной строки Azure, скачать исходный код, сообщить о проблемах или принять участие в проекте, зайдите в [репозиторий GitHub для интерфейса командной строки Azure](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="15ffb-155">To learn more about the Azure CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure CLI](https://github.com/azure/azure-xplat-cli).</span></span>
* <span data-ttu-id="15ffb-156">Если у вас возникли вопросы об использовании интерфейса командной строки Azure или платформы Azure, посетите [форумы Azure](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span><span class="sxs-lookup"><span data-stu-id="15ffb-156">If you have questions about using the Azure CLI, or Azure, visit the [Azure Forums](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span></span>

[mac-installer]: https://aka.ms/mac-azure-cli
[windows-installer]: https://aka.ms/webpi-azure-cli
[linux-installer]: https://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md
