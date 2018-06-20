---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI 2.0 в macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 37358e991f96dd517d169e3b3ac651d513897d6d
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
ms.locfileid: "32044117"
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="e79c7-103">Установка Azure CLI 2.0 в macOS</span><span class="sxs-lookup"><span data-stu-id="e79c7-103">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="e79c7-104">На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](http://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="e79c7-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](http://brew.sh).</span></span> <span data-ttu-id="e79c7-105">Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="e79c7-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="e79c7-106">Пакет CLI протестирован с macOS 10.9 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="e79c7-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="e79c7-107">Install</span><span class="sxs-lookup"><span data-stu-id="e79c7-107">Install</span></span>

<span data-ttu-id="e79c7-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="e79c7-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="e79c7-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="e79c7-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="e79c7-110">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="e79c7-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="e79c7-111">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="e79c7-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="e79c7-112">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e79c7-113">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="e79c7-114">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e79c7-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e79c7-115">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e79c7-115">Troubleshooting</span></span>

<span data-ttu-id="e79c7-116">Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="e79c7-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="e79c7-117">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e79c7-117">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="e79c7-118">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="e79c7-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="e79c7-119">Если при установке не удается найти Python или установленные пакеты, причина может быть в незначительном несоответствии номера версии или в проблеме с установкой homebrew.</span><span class="sxs-lookup"><span data-stu-id="e79c7-119">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue that occurred during homebrew installation.</span></span> <span data-ttu-id="e79c7-120">Так как для CLI не используется виртуальное окружение Python, важно, чтобы была найдена правильная версия Python.</span><span class="sxs-lookup"><span data-stu-id="e79c7-120">Since the CLI does not use a Python virtual environment, it relies on being able to find correct Python version.</span></span> <span data-ttu-id="e79c7-121">Эти проблемы можно устранить, перенастроив установку Python.</span><span class="sxs-lookup"><span data-stu-id="e79c7-121">You may be able to fix these issues by relinking your Python installation.</span></span>

```bash
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="e79c7-122">Установлена версия CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="e79c7-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="e79c7-123">Если установлена устаревшая версия, возможно, причиной является устаревший кэш homebrew.</span><span class="sxs-lookup"><span data-stu-id="e79c7-123">If an out-of-date version was installed, it could be due to a stale homebrew cache.</span></span> <span data-ttu-id="e79c7-124">Следуйте инструкциям по [обновлению](#Update).</span><span class="sxs-lookup"><span data-stu-id="e79c7-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="e79c7-125">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="e79c7-125">Update</span></span>

<span data-ttu-id="e79c7-126">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="e79c7-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="e79c7-127">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="e79c7-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="e79c7-128">Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="e79c7-129">Удаление</span><span class="sxs-lookup"><span data-stu-id="e79c7-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="e79c7-130">Для удаления пакета `azure-cli` воспользуйтесь homebrew.</span><span class="sxs-lookup"><span data-stu-id="e79c7-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```
