---
title: Установка классического интерфейса командной строки Azure (Azure Classic CLI)
description: Установка классического интерфейса командной строки Azure на компьютерах Mac OS, Linux и Windows и начало работы со службами Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/11/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 0cc1d7811223bf6f473c2c4516d0919306aa74c7
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779488"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="07647-103">Установка классического интерфейса командной строки Azure (Azure Classic CLI)</span><span class="sxs-lookup"><span data-stu-id="07647-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="07647-104">В этом разделе описывается, как установить классический интерфейс командной строки Azure (Azure Classic CLI).</span><span class="sxs-lookup"><span data-stu-id="07647-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="07647-105">Классический интерфейс командной строки считается нерекомендуемым, и его следует использовать только с классической моделью развертывания.</span><span class="sxs-lookup"><span data-stu-id="07647-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="07647-106">Для всех других развертываний используйте [Azure CLI](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="07647-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="07647-107">Классический интерфейс командной строки Azure можно быстро установить, чтобы использовать набор консольных команд с открытым кодом для создания ресурсов в Microsoft Azure и управления ими.</span><span class="sxs-lookup"><span data-stu-id="07647-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="07647-108">Существует несколько вариантов установки этих кроссплатформенных инструментов на компьютер.</span><span class="sxs-lookup"><span data-stu-id="07647-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="07647-109">**Пакет npm**. Запустите npm (диспетчер пакетов для JavaScript), чтобы установить пакет классического интерфейса командной строки Azure в дистрибутиве или ОС Linux.</span><span class="sxs-lookup"><span data-stu-id="07647-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="07647-110">Для этого требуется Node.js и npm.</span><span class="sxs-lookup"><span data-stu-id="07647-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="07647-111">**Установщик**. Скачайте установщик, чтобы легко установить этот инструмент на компьютеры под управлением macOS или Windows.</span><span class="sxs-lookup"><span data-stu-id="07647-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="07647-112">**Контейнер Docker**. Приступите к использованию классического интерфейса командной строки из готового контейнера Docker.</span><span class="sxs-lookup"><span data-stu-id="07647-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="07647-113">Для этого требуется узел Docker.</span><span class="sxs-lookup"><span data-stu-id="07647-113">Requires a Docker host.</span></span>

<span data-ttu-id="07647-114">Дополнительные сведения и варианты установки см. в репозитории проектов на сайте [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="07647-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="07647-115">Установив классический интерфейс командной строки Azure, установите подключение с помощью команды `azure login` и выполните команды `azure` из интерфейса командной строки (Bash, терминал, командная строка и т. п.) для работы с ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="07647-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="07647-116">Вариант 1. Установка пакета npm</span><span class="sxs-lookup"><span data-stu-id="07647-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="07647-117">Чтобы установить классический интерфейс командной строки из пакета npm, установите в системе [последнюю версию Node.js и npm](https://nodejs.org/en/download/package-manager/).</span><span class="sxs-lookup"><span data-stu-id="07647-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="07647-118">Затем выполните `npm install`, чтобы установить пакет azure-cli:</span><span class="sxs-lookup"><span data-stu-id="07647-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="07647-119">В дистрибутивах Linux для выполнения команды `sudo` может потребоваться команда `npm`:</span><span class="sxs-lookup"><span data-stu-id="07647-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="07647-120">Если вам нужно установить или обновить Node.js и npm на операционной системе, рекомендуется установить Node.js версии 4.х (LTS) или более поздней.</span><span class="sxs-lookup"><span data-stu-id="07647-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="07647-121">Если вы используете более раннюю версию, возможны ошибки при установке.</span><span class="sxs-lookup"><span data-stu-id="07647-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="07647-122">При необходимости также можно скачать TAR-файл из [страницы выпусков репозитория GitHub](https://github.com/Azure/azure-xplat-cli/releases).</span><span class="sxs-lookup"><span data-stu-id="07647-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="07647-123">Затем установите скачанный пакет npm как описано ниже (возможно, для дистрибутивов Linux потребуется использовать `sudo`).</span><span class="sxs-lookup"><span data-stu-id="07647-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="07647-124">Вариант 2. Использование установщика</span><span class="sxs-lookup"><span data-stu-id="07647-124">Option 2: Use an installer</span></span>

<span data-ttu-id="07647-125">Если вы используете компьютер с Mac или Windows, на [странице выпусков репозитория GitHub](https://github.com/Azure/azure-xplat-cli/releases) доступны установщики DMG и MSI.</span><span class="sxs-lookup"><span data-stu-id="07647-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="07647-126">Чтобы установить классический интерфейс командной строки в Windows, можете также скачать [установщик веб-платформы](https://go.microsoft.com/?linkid=9828653).</span><span class="sxs-lookup"><span data-stu-id="07647-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="07647-127">Этот установщик позволяет дополнительно установить пакет Azure SDK и инструменты командной строки.</span><span class="sxs-lookup"><span data-stu-id="07647-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="07647-128">Вариант 3. Использование контейнера Docker</span><span class="sxs-lookup"><span data-stu-id="07647-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="07647-129">Если вы настроили компьютер в качестве узла [Docker](https://docs.docker.com/engine/understanding-docker/), то можно запустить классический интерфейс командной строки Azure в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="07647-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="07647-130">Выполните следующую команду (возможно, для дистрибутивов Linux потребуется использовать `sudo`):</span><span class="sxs-lookup"><span data-stu-id="07647-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="07647-131">Выполнение команд классического интерфейса командной строки Azure</span><span class="sxs-lookup"><span data-stu-id="07647-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="07647-132">Установив классический интерфейс командной строки Azure, выполните команду `azure` в любом интерфейсе командной строки (Bash, терминале, командной строке и т. п.).</span><span class="sxs-lookup"><span data-stu-id="07647-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="07647-133">Например, чтобы выполнить команду справки, введите следующее:</span><span class="sxs-lookup"><span data-stu-id="07647-133">For example, to run the help command, type the following:</span></span>

```azurecli-interactive
azure help
```

> [!NOTE]
> <span data-ttu-id="07647-134">Для некоторых дистрибутивов Linux может появиться сообщение об ошибке `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="07647-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="07647-135">Это связано с тем, что новые установки Node.js размещаются в папке /usr/bin/nodejs.</span><span class="sxs-lookup"><span data-stu-id="07647-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="07647-136">Для устранения этой ошибки создайте символьную ссылку /usr/bin/node, выполнив следующую команду:</span><span class="sxs-lookup"><span data-stu-id="07647-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="07647-137">Чтобы просмотреть версии классического интерфейса командной строки Azure, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="07647-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli-interactive
azure --version
```

> [!NOTE]
> <span data-ttu-id="07647-138">При первом использовании классического интерфейса командной строки Azure появится сообщение с вопросом, следует ли разрешить корпорации Майкрософт собирать сведения об использовании.</span><span class="sxs-lookup"><span data-stu-id="07647-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="07647-139">Участие является добровольным.</span><span class="sxs-lookup"><span data-stu-id="07647-139">Participation is voluntary.</span></span> <span data-ttu-id="07647-140">Если вы согласились участвовать в этой программе, сбор сведений можно остановить в любой момент, выполнив команду `azure telemetry --disable`.</span><span class="sxs-lookup"><span data-stu-id="07647-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="07647-141">Чтобы включить участие в любой момент, выполните команду `azure telemetry --enable`.</span><span class="sxs-lookup"><span data-stu-id="07647-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="07647-142">Обновление классического интерфейса командной строки</span><span class="sxs-lookup"><span data-stu-id="07647-142">Update the classic CLI</span></span>

<span data-ttu-id="07647-143">Корпорация Майкрософт может выпускать обновленные версии классического интерфейса командной строки Azure.</span><span class="sxs-lookup"><span data-stu-id="07647-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="07647-144">Переустановите классический интерфейс командной строки с помощью установщика для соответствующей операционной системы или запустите последнюю версию контейнера Docker.</span><span class="sxs-lookup"><span data-stu-id="07647-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="07647-145">Если вы установили последние версии Node.js и npm, выполните обновление, введя следующую команду (возможно, для дистрибутивов Linux потребуется использовать `sudo`).</span><span class="sxs-lookup"><span data-stu-id="07647-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="07647-146">Включение выполнения нажатием клавиши TAB</span><span class="sxs-lookup"><span data-stu-id="07647-146">Enable tab completion</span></span>

<span data-ttu-id="07647-147">Дополнение команд классического интерфейса командной строки нажатием клавиши TAB поддерживается на компьютерах MAC и Linux.</span><span class="sxs-lookup"><span data-stu-id="07647-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="07647-148">Чтобы включить эту функцию в zsh, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="07647-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="07647-149">Чтобы включить эту функцию в bash, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="07647-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="07647-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="07647-150">Next steps</span></span>

* <span data-ttu-id="07647-151">Чтобы получить дополнительные сведения о классическом интерфейсе командной строки Azure, скачать исходный код, сообщить о проблемах или принять участие в проекте, посетите [этот репозиторий GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="07647-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>
