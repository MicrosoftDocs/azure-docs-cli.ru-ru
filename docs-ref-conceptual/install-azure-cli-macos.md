---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI в macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593172"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="1a429-103">Установка Azure CLI в macOS</span><span class="sxs-lookup"><span data-stu-id="1a429-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="1a429-104">На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="1a429-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="1a429-105">Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="1a429-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="1a429-106">Пакет CLI протестирован с macOS 10.9 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="1a429-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="1a429-107">Install</span><span class="sxs-lookup"><span data-stu-id="1a429-107">Install</span></span>

<span data-ttu-id="1a429-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="1a429-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="1a429-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="1a429-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="1a429-110">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="1a429-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="1a429-111">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="1a429-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="1a429-112">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="1a429-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="1a429-113">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1a429-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1a429-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1a429-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1a429-115">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="1a429-115">Troubleshooting</span></span>

<span data-ttu-id="1a429-116">Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="1a429-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="1a429-117">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="1a429-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="1a429-118">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="1a429-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="1a429-119">Во время установки с помощью homebrew может наблюдаться несовпадение дополнительного номера версии или другая проблема.</span><span class="sxs-lookup"><span data-stu-id="1a429-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="1a429-120">CLI не использует виртуальное окружение Python и попытается обнаружить установленную версию Python.</span><span class="sxs-lookup"><span data-stu-id="1a429-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="1a429-121">Возможное решение — установить зависимость `python3` и повторно создать на нее ссылку из Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1a429-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="1a429-122">Установлена версия CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="1a429-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="1a429-123">Если установлена старая версия, это может произойти из-за устаревания кэша homebrew.</span><span class="sxs-lookup"><span data-stu-id="1a429-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="1a429-124">Следуйте инструкциям по [обновлению](#Update).</span><span class="sxs-lookup"><span data-stu-id="1a429-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="1a429-125">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="1a429-125">Update</span></span>

<span data-ttu-id="1a429-126">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="1a429-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="1a429-127">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="1a429-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="1a429-128">Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="1a429-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="1a429-129">Удаление</span><span class="sxs-lookup"><span data-stu-id="1a429-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="1a429-130">Для удаления пакета `azure-cli` воспользуйтесь homebrew.</span><span class="sxs-lookup"><span data-stu-id="1a429-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="1a429-131">Другие методы установки</span><span class="sxs-lookup"><span data-stu-id="1a429-131">Other installation methods</span></span>

<span data-ttu-id="1a429-132">При невозможности использовать Homebrew для установки Azure CLI в своей среде можно воспользоваться инструкциями по ручной установке для Linux.</span><span class="sxs-lookup"><span data-stu-id="1a429-132">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="1a429-133">Следует учесть, что этот процесс не является официально рекомендованным для macOS.</span><span class="sxs-lookup"><span data-stu-id="1a429-133">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="1a429-134">Всегда предпочтительнее использовать менеджер пакетов, например Homebrew.</span><span class="sxs-lookup"><span data-stu-id="1a429-134">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="1a429-135">Используйте метод ручной установки только при отсутствии других вариантов.</span><span class="sxs-lookup"><span data-stu-id="1a429-135">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="1a429-136">Инструкции по ручной установке Azure CLI в Linux см. в [соответствующей статье](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="1a429-136">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a429-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1a429-137">Next Steps</span></span>

<span data-ttu-id="1a429-138">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="1a429-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1a429-139">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1a429-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
