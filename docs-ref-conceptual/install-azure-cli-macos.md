---
title: "Установка Azure CLI для macOS"
description: "Как установить Azure CLI 2.0 в macOS"
keywords: Azure CLI,Install Azure CLI,azure macos, azure install macos
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: e615d2b3ab3b1307e982cb1d4d456633440afdf6
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-macos"></a><span data-ttu-id="c14a1-104">Установка Azure CLI 2.0 в macOS</span><span class="sxs-lookup"><span data-stu-id="c14a1-104">Install Azure CLI 2.0 on macOS</span></span>

<span data-ttu-id="c14a1-105">Для платформы macOS можно установить Azure CLI с помощью [диспетчера пакетов homebrew](http://brew.sh) или вручную.</span><span class="sxs-lookup"><span data-stu-id="c14a1-105">For the macOS platform, you can install the Azure CLI either through the [homebrew package manager](http://brew.sh) or manually.</span></span> <span data-ttu-id="c14a1-106">Использовать диспетчер пакетов homebrew предпочтительнее, так как это средство упрощает установку, обновление и удаление (при необходимости).</span><span class="sxs-lookup"><span data-stu-id="c14a1-106">The preferred installation method is through homebrew, so that it's easier to install, get updates, and uninstall if you need to.</span></span>

## <a name="use-homebrew-to-install"></a><span data-ttu-id="c14a1-107">Установка с помощью homebrew</span><span class="sxs-lookup"><span data-stu-id="c14a1-107">Use homebrew to install</span></span>

<span data-ttu-id="c14a1-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="c14a1-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="c14a1-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="c14a1-109">It provides convenient ways to install, update, and uninstall.</span></span> <span data-ttu-id="c14a1-110">как и другие аналогичные средства, включая `apt` или `yum`.</span><span class="sxs-lookup"><span data-stu-id="c14a1-110">It's similar to other package managers such as `apt` or `yum`.</span></span>
<span data-ttu-id="c14a1-111">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="c14a1-111">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="c14a1-112">Установка с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="c14a1-112">Install with homebrew</span></span>

<span data-ttu-id="c14a1-113">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="c14a1-113">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="c14a1-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="c14a1-114">You can then run the Azure CLI with the `az` command.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="c14a1-115">Обновление с помощью homebrew</span><span class="sxs-lookup"><span data-stu-id="c14a1-115">Update with homebrew</span></span>

<span data-ttu-id="c14a1-116">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="c14a1-116">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="c14a1-117">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="c14a1-117">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="c14a1-118">Вам нужно будет обновить сведения о локальном репозитории, а затем — обновить сам пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="c14a1-118">You will need to update your local repository information, and then update the CLI package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

### <a name="troubleshooting"></a><span data-ttu-id="c14a1-119">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="c14a1-119">Troubleshooting</span></span>

<span data-ttu-id="c14a1-120">У вас возникли проблемы с установкой или обновлением CLI с помощью homebrew?</span><span class="sxs-lookup"><span data-stu-id="c14a1-120">Did you encounter a problem when installing or updating the CLI with homebrew?</span></span> <span data-ttu-id="c14a1-121">Ниже описаны некоторые распространенные ошибки, а также способы их диагностики и устранения.</span><span class="sxs-lookup"><span data-stu-id="c14a1-121">Here are some common errors that might occur, and ways to diagnose and resolve them.</span></span>

#### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="c14a1-122">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="c14a1-122">Unable to find Python or installed packages</span></span>

<span data-ttu-id="c14a1-123">Если при установке не удается найти Python или установленные пакеты, причина может быть в незначительном несоответствии номера версии или в проблеме с установкой homebrew.</span><span class="sxs-lookup"><span data-stu-id="c14a1-123">If your install is unable to find Python or installed packages, there may be a minor version mismatch or other issue which occurred during homebrew installation.</span></span> <span data-ttu-id="c14a1-124">Так как CLI не использует virtualenv, важно, чтобы при установке с помощью homebrew была найдена правильная версия Python.</span><span class="sxs-lookup"><span data-stu-id="c14a1-124">Since the CLI does not use a virtualenv, it relies on being able to find correct versions of Python installed by homebrew.</span></span> <span data-ttu-id="c14a1-125">Эти проблемы можно устранить, перенастроив установку Python:</span><span class="sxs-lookup"><span data-stu-id="c14a1-125">You may be able to fix these issues by re-linking your Python installation:</span></span>

```bash
brew link --overwrite python3
```

#### <a name="the-cli-version-is-out-of-date"></a><span data-ttu-id="c14a1-126">Версия CLI устарела</span><span class="sxs-lookup"><span data-stu-id="c14a1-126">The CLI version is out of date</span></span>

<span data-ttu-id="c14a1-127">Если вы считаете, что установленная версия CLI могла устареть, последовательно выполните команды `brew update` и `brew upgrade azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="c14a1-127">If you think that your installed CLI version might be out of date, you will need to run a `brew update` command, followed by `brew upgrade azure-cli`.</span></span> <span data-ttu-id="c14a1-128">Если обновление CLI не произойдет, имейте в виду, что пакеты homebrew могут развертываться медленнее, чем общие выпуски.</span><span class="sxs-lookup"><span data-stu-id="c14a1-128">If this does not update the CLI, be aware that homebrew packages may roll out more slowly than general releases.</span></span> <span data-ttu-id="c14a1-129">Если вам нужно установить самую последнюю версию CLI, выполните [установку вручную](#manage-the-cli-manually).</span><span class="sxs-lookup"><span data-stu-id="c14a1-129">If you require bleeding-edge installs of the CLI, then you should [install manually](#manage-the-cli-manually).</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="c14a1-130">Удаление с помощью homebrew</span><span class="sxs-lookup"><span data-stu-id="c14a1-130">Uninstall with homebrew</span></span>

<span data-ttu-id="c14a1-131">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="c14a1-131">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="c14a1-132">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="c14a1-132">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="c14a1-133">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="c14a1-133">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="c14a1-134">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="c14a1-134">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="c14a1-135">Если установка выполнялась с помощью homebrew, это же средство следует использовать и для удаления.</span><span class="sxs-lookup"><span data-stu-id="c14a1-135">If you installed with homebrew, you should also use it to uninstall.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="install-the-cli-manually"></a><span data-ttu-id="c14a1-136">Установка CLI вручную</span><span class="sxs-lookup"><span data-stu-id="c14a1-136">Install the CLI manually</span></span>

<span data-ttu-id="c14a1-137">Если вы не можете или не хотите использовать homebrew, установить CLI можно вручную.</span><span class="sxs-lookup"><span data-stu-id="c14a1-137">If you can't or don't want to rely on homebrew to manage the CLI install for you, then you can manually install.</span></span>

<span data-ttu-id="c14a1-138">Выполните [инструкции по установке в Linux вручную](install-azure-cli-linux.md), чтобы установить CLI вручную в macOS.</span><span class="sxs-lookup"><span data-stu-id="c14a1-138">Follow the [manual Linux installation instructions](install-azure-cli-linux.md) to install manually on macOS.</span></span> <span data-ttu-id="c14a1-139">В macOS версии 10.9 и выше должны содержаться все необходимые зависимости.</span><span class="sxs-lookup"><span data-stu-id="c14a1-139">macOS versions 10.9 and later should include all of the required dependencies.</span></span>
