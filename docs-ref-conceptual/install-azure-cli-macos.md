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
ms.openlocfilehash: 790c63a60a5d23863b48227dcc99462bbf950d80
ms.sourcegitcommit: b42ce26476b135bb2047c8d9d787580c858f8b6b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "72163846"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="249a7-103">Установка Azure CLI в macOS</span><span class="sxs-lookup"><span data-stu-id="249a7-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="249a7-104">На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="249a7-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="249a7-105">Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="249a7-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="249a7-106">Пакет CLI протестирован с macOS 10.9 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="249a7-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="249a7-107">Установка с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="249a7-107">Install with Homebrew</span></span>

<span data-ttu-id="249a7-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="249a7-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="249a7-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="249a7-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="249a7-110">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="249a7-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="249a7-111">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="249a7-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="249a7-112">Azure CLI имеет зависимость с пакетом Homebrew `python3` и выполняет его установку.</span><span class="sxs-lookup"><span data-stu-id="249a7-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="249a7-113">Интерфейс Azure CLI гарантированно совместим с последней версией `python3`, опубликованной в Homebrew.</span><span class="sxs-lookup"><span data-stu-id="249a7-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="249a7-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="249a7-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="249a7-115">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="249a7-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="249a7-116">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="249a7-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="249a7-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="249a7-117">Troubleshooting</span></span>

<span data-ttu-id="249a7-118">Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="249a7-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="249a7-119">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="249a7-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="249a7-120">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="249a7-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="249a7-121">Во время установки с помощью homebrew может наблюдаться несовпадение дополнительного номера версии или другая проблема.</span><span class="sxs-lookup"><span data-stu-id="249a7-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="249a7-122">CLI не использует виртуальное окружение Python и попытается обнаружить установленную версию Python.</span><span class="sxs-lookup"><span data-stu-id="249a7-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="249a7-123">Возможное решение — установить зависимость `python3` и повторно создать на нее ссылку из Homebrew.</span><span class="sxs-lookup"><span data-stu-id="249a7-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="249a7-124">Установлена версия CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="249a7-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="249a7-125">Если установлена старая версия, это может произойти из-за устаревания кэша homebrew.</span><span class="sxs-lookup"><span data-stu-id="249a7-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="249a7-126">Следуйте инструкциям по [обновлению](#update).</span><span class="sxs-lookup"><span data-stu-id="249a7-126">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="249a7-127">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="249a7-127">Proxy blocks connection</span></span>

<span data-ttu-id="249a7-128">Вы не сможете получать ресурсы из Homebrew, если неправильно настроите использование прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="249a7-128">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="249a7-129">Выполните [инструкции по настройке прокси-сервера Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span><span class="sxs-lookup"><span data-stu-id="249a7-129">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="249a7-130">Если вы работаете за прокси-сервером, `HTTP_PROXY` и `HTTPS_PROXY` нужно задать для подключения к службам Azure с помощью CLI.</span><span class="sxs-lookup"><span data-stu-id="249a7-130">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="249a7-131">Если вы не используете обычную аутентификацию, рекомендуется экспортировать эти переменные в файл `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="249a7-131">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="249a7-132">Всегда следуйте корпоративным политикам безопасности и учитывайте требования системного администратора.</span><span class="sxs-lookup"><span data-stu-id="249a7-132">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="249a7-133">Чтобы вы могли получать соответствующие ресурсы из Homebrew, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="249a7-133">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="249a7-134">Обновление</span><span class="sxs-lookup"><span data-stu-id="249a7-134">Update</span></span>

<span data-ttu-id="249a7-135">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="249a7-135">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="249a7-136">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="249a7-136">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="249a7-137">Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="249a7-137">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="249a7-138">Удаление</span><span class="sxs-lookup"><span data-stu-id="249a7-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="249a7-139">Для удаления пакета `azure-cli` воспользуйтесь homebrew.</span><span class="sxs-lookup"><span data-stu-id="249a7-139">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="249a7-140">Другие методы установки</span><span class="sxs-lookup"><span data-stu-id="249a7-140">Other installation methods</span></span>

<span data-ttu-id="249a7-141">При невозможности использовать Homebrew для установки Azure CLI в своей среде можно воспользоваться инструкциями по ручной установке для Linux.</span><span class="sxs-lookup"><span data-stu-id="249a7-141">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="249a7-142">Следует учесть, что этот процесс не является официально рекомендованным для macOS.</span><span class="sxs-lookup"><span data-stu-id="249a7-142">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="249a7-143">Всегда предпочтительнее использовать менеджер пакетов, например Homebrew.</span><span class="sxs-lookup"><span data-stu-id="249a7-143">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="249a7-144">Используйте метод ручной установки только при отсутствии других вариантов.</span><span class="sxs-lookup"><span data-stu-id="249a7-144">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="249a7-145">Инструкции по ручной установке Azure CLI в Linux см. в [соответствующей статье](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="249a7-145">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="249a7-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="249a7-146">Next Steps</span></span>

<span data-ttu-id="249a7-147">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="249a7-147">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="249a7-148">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="249a7-148">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
