---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI 2.0 в macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: fd829c6ff9162b660a889d3e08615a76f42aeb97
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388479"
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="3c75d-103">Установка Azure CLI 2.0 в macOS</span><span class="sxs-lookup"><span data-stu-id="3c75d-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="3c75d-104">На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="3c75d-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="3c75d-105">Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="3c75d-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="3c75d-106">Пакет CLI протестирован с macOS 10.9 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="3c75d-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="3c75d-107">Install</span><span class="sxs-lookup"><span data-stu-id="3c75d-107">Install</span></span>

<span data-ttu-id="3c75d-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="3c75d-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="3c75d-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="3c75d-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="3c75d-110">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="3c75d-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="3c75d-111">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="3c75d-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="3c75d-112">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="3c75d-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="3c75d-113">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="3c75d-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="3c75d-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="3c75d-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3c75d-115">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="3c75d-115">Troubleshooting</span></span>

<span data-ttu-id="3c75d-116">Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="3c75d-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="3c75d-117">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="3c75d-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="3c75d-118">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="3c75d-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="3c75d-119">Во время установки с помощью homebrew может наблюдаться несовпадение дополнительного номера версии или другая проблема.</span><span class="sxs-lookup"><span data-stu-id="3c75d-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="3c75d-120">CLI не использует виртуальное окружение Python и попытается обнаружить установленную версию Python.</span><span class="sxs-lookup"><span data-stu-id="3c75d-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="3c75d-121">Возможное решение — установить зависимость `python3` и повторно создать на нее ссылку из Homebrew.</span><span class="sxs-lookup"><span data-stu-id="3c75d-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="3c75d-122">Установлена версия CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="3c75d-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="3c75d-123">Если установлена старая версия, это может произойти из-за устаревания кэша homebrew.</span><span class="sxs-lookup"><span data-stu-id="3c75d-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="3c75d-124">Следуйте инструкциям по [обновлению](#Update).</span><span class="sxs-lookup"><span data-stu-id="3c75d-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="3c75d-125">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="3c75d-125">Update</span></span>

<span data-ttu-id="3c75d-126">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="3c75d-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="3c75d-127">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="3c75d-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="3c75d-128">Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="3c75d-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="3c75d-129">Удаление</span><span class="sxs-lookup"><span data-stu-id="3c75d-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="3c75d-130">Для удаления пакета `azure-cli` воспользуйтесь homebrew.</span><span class="sxs-lookup"><span data-stu-id="3c75d-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
