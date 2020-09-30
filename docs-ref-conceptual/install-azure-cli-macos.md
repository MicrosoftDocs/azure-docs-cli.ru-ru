---
title: Установка Azure CLI для macOS
description: Как установить Azure CLI в macOS
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/05/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ad2cda66e3876bafbc671b5a0593ca470d2308e6
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225802"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="a8c74-103">Установка Azure CLI в macOS</span><span class="sxs-lookup"><span data-stu-id="a8c74-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="a8c74-104">На платформе macOS Azure CLI можно установить с помощью [диспетчера пакетов Homebrew](https://brew.sh).</span><span class="sxs-lookup"><span data-stu-id="a8c74-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="a8c74-105">Homebrew позволяет без труда поддерживать установку CLI в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="a8c74-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="a8c74-106">Пакет CLI протестирован с macOS 10.9 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a8c74-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="a8c74-107">Установка с помощью Homebrew</span><span class="sxs-lookup"><span data-stu-id="a8c74-107">Install with Homebrew</span></span>

<span data-ttu-id="a8c74-108">Homebrew — это самый простой способ управления установкой CLI.</span><span class="sxs-lookup"><span data-stu-id="a8c74-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="a8c74-109">Это удобное средство установки, обновления и удаления,</span><span class="sxs-lookup"><span data-stu-id="a8c74-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="a8c74-110">Если у вас в системе нет диспетчера пакетов homebrew, [установите его](https://docs.brew.sh/Installation.html), прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="a8c74-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="a8c74-111">Можно установить CLI, обновив сведения о репозитории brew, а затем выполнив команду `install`:</span><span class="sxs-lookup"><span data-stu-id="a8c74-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="a8c74-112">Azure CLI имеет зависимость с пакетом Homebrew `python3` и выполняет его установку.</span><span class="sxs-lookup"><span data-stu-id="a8c74-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="a8c74-113">Интерфейс Azure CLI гарантированно совместим с последней версией `python3`, опубликованной в Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a8c74-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="a8c74-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="a8c74-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="a8c74-115">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="a8c74-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a8c74-116">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a8c74-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a8c74-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="a8c74-117">Troubleshooting</span></span>

<span data-ttu-id="a8c74-118">Если у вас возникли проблемы при установке CLI с помощью Homebrew, воспользуйтесь представленным ниже описанием распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="a8c74-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="a8c74-119">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a8c74-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="completion-is-not-working"></a><span data-ttu-id="a8c74-120">Сжатие не выполняется.</span><span class="sxs-lookup"><span data-stu-id="a8c74-120">Completion is not working</span></span>

<span data-ttu-id="a8c74-121">Формула Homebrew в Azure CLI устанавливает файл завершения с именем `az` в каталоге завершения, управляемом Homebrew (расположение по умолчанию — `/usr/local/etc/bash_completion.d/`).</span><span class="sxs-lookup"><span data-stu-id="a8c74-121">The Homebrew formula of Azure CLI installs a completion file named `az` in the Homebrew-managed completions directory (default location is `/usr/local/etc/bash_completion.d/`).</span></span> <span data-ttu-id="a8c74-122">Чтобы включить завершение, следуйте инструкциям по [использованию Homebrew](https://docs.brew.sh/Shell-Completion).</span><span class="sxs-lookup"><span data-stu-id="a8c74-122">To enable completion, please follow Homebrew's instructions [here](https://docs.brew.sh/Shell-Completion).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="a8c74-123">Не удается найти Python или установленные пакеты</span><span class="sxs-lookup"><span data-stu-id="a8c74-123">Unable to find Python or installed packages</span></span>

<span data-ttu-id="a8c74-124">Во время установки с помощью homebrew может наблюдаться несовпадение дополнительного номера версии или другая проблема.</span><span class="sxs-lookup"><span data-stu-id="a8c74-124">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="a8c74-125">CLI не использует виртуальное окружение Python и попытается обнаружить установленную версию Python.</span><span class="sxs-lookup"><span data-stu-id="a8c74-125">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="a8c74-126">Возможное решение — установить зависимость `python3` и повторно создать на нее ссылку из Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a8c74-126">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="a8c74-127">Установлена версия CLI 1.x</span><span class="sxs-lookup"><span data-stu-id="a8c74-127">CLI version 1.x is installed</span></span>

<span data-ttu-id="a8c74-128">Если установлена старая версия, это может произойти из-за устаревания кэша homebrew.</span><span class="sxs-lookup"><span data-stu-id="a8c74-128">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="a8c74-129">Следуйте инструкциям по [обновлению](#update).</span><span class="sxs-lookup"><span data-stu-id="a8c74-129">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="a8c74-130">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="a8c74-130">Proxy blocks connection</span></span>

<span data-ttu-id="a8c74-131">Вы не сможете получать ресурсы из Homebrew, если неправильно настроите использование прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a8c74-131">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="a8c74-132">Выполните [инструкции по настройке прокси-сервера Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span><span class="sxs-lookup"><span data-stu-id="a8c74-132">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a8c74-133">Если вы работаете за прокси-сервером, `HTTP_PROXY` и `HTTPS_PROXY` нужно задать для подключения к службам Azure с помощью CLI.</span><span class="sxs-lookup"><span data-stu-id="a8c74-133">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="a8c74-134">Если вы не используете обычную аутентификацию, рекомендуется экспортировать эти переменные в файл `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="a8c74-134">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="a8c74-135">Всегда следуйте корпоративным политикам безопасности и учитывайте требования системного администратора.</span><span class="sxs-lookup"><span data-stu-id="a8c74-135">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="a8c74-136">Чтобы вы могли получать соответствующие ресурсы из Homebrew, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="a8c74-136">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="a8c74-137">Update</span><span class="sxs-lookup"><span data-stu-id="a8c74-137">Update</span></span>

<span data-ttu-id="a8c74-138">CLI регулярно обновляется для исправления ошибок, а также реализации улучшений, новых возможностей и функции предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="a8c74-138">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="a8c74-139">Новый выпуск выходит примерно раз в две недели.</span><span class="sxs-lookup"><span data-stu-id="a8c74-139">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="a8c74-140">Обновите сведения о локальном репозитории, а затем — сам пакет `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="a8c74-140">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="a8c74-141">Удаление</span><span class="sxs-lookup"><span data-stu-id="a8c74-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="a8c74-142">Для удаления пакета `azure-cli` воспользуйтесь homebrew.</span><span class="sxs-lookup"><span data-stu-id="a8c74-142">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="a8c74-143">Другие методы установки</span><span class="sxs-lookup"><span data-stu-id="a8c74-143">Other installation methods</span></span>

<span data-ttu-id="a8c74-144">При невозможности использовать Homebrew для установки Azure CLI в своей среде можно воспользоваться инструкциями по ручной установке для Linux.</span><span class="sxs-lookup"><span data-stu-id="a8c74-144">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="a8c74-145">Следует учесть, что этот процесс не является официально рекомендованным для macOS.</span><span class="sxs-lookup"><span data-stu-id="a8c74-145">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="a8c74-146">Всегда предпочтительнее использовать менеджер пакетов, например Homebrew.</span><span class="sxs-lookup"><span data-stu-id="a8c74-146">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="a8c74-147">Используйте метод ручной установки только при отсутствии других вариантов.</span><span class="sxs-lookup"><span data-stu-id="a8c74-147">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="a8c74-148">Инструкции по ручной установке Azure CLI в Linux см. в [соответствующей статье](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="a8c74-148">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a8c74-149">Next Steps</span><span class="sxs-lookup"><span data-stu-id="a8c74-149">Next Steps</span></span>

<span data-ttu-id="a8c74-150">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="a8c74-150">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a8c74-151">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a8c74-151">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)