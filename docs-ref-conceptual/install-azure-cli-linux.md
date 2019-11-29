---
title: Установка Azure CLI для Linux вручную
description: Как установить Azure CLI в Linux вручную
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: caca30ec186f302e47f2978b9bfe616d4b2a5c02
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543640"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="f0878-103">Установка Azure CLI в Linux вручную</span><span class="sxs-lookup"><span data-stu-id="f0878-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="f0878-104">Если для вашего дистрибутива отсутствует пакет Azure CLI, установите CLI вручную, выполнив скрипт.</span><span class="sxs-lookup"><span data-stu-id="f0878-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="f0878-105">Настоятельно рекомендуется устанавливать CLI с помощью диспетчера пакетов.</span><span class="sxs-lookup"><span data-stu-id="f0878-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="f0878-106">Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI.</span><span class="sxs-lookup"><span data-stu-id="f0878-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="f0878-107">Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="f0878-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0878-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f0878-108">Prerequisites</span></span>

<span data-ttu-id="f0878-109">Для использования CLI требуется следующее ПО:</span><span class="sxs-lookup"><span data-stu-id="f0878-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="f0878-110">[Python версии 3.6.x или 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="f0878-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="f0878-111">libffi</span><span class="sxs-lookup"><span data-stu-id="f0878-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="f0878-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="f0878-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="f0878-113">Интерфейс CLI также совместим с Python 2.7.x, поддержка которого прекращается 1 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="f0878-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="f0878-114">В следующей версии Azure CLI поддержка Python 2.7 будет прекращена.</span><span class="sxs-lookup"><span data-stu-id="f0878-114">A future version of Azure CLI will drop support for Python 2.7.</span></span> <span data-ttu-id="f0878-115">Поэтому мы рекомендуем установить для CLI Python 3.</span><span class="sxs-lookup"><span data-stu-id="f0878-115">For this reason we recommend that you install Python 3 to run the CLI.</span></span> 

## <a name="install-or-update"></a><span data-ttu-id="f0878-116">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="f0878-116">Install or update</span></span>

<span data-ttu-id="f0878-117">Для установки и обновления CLI требуется повторный запуск установочного скрипта.</span><span class="sxs-lookup"><span data-stu-id="f0878-117">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="f0878-118">Установите CLI, выполнив `curl`.</span><span class="sxs-lookup"><span data-stu-id="f0878-118">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="f0878-119">Скрипт также можно скачать и выполнить на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="f0878-119">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="f0878-120">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="f0878-120">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="f0878-121">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="f0878-121">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f0878-122">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f0878-122">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f0878-123">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f0878-123">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f0878-124">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="f0878-124">Troubleshooting</span></span>

<span data-ttu-id="f0878-125">Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную.</span><span class="sxs-lookup"><span data-stu-id="f0878-125">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="f0878-126">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f0878-126">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="f0878-127">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="f0878-127">curl "Object Moved" error</span></span>

<span data-ttu-id="f0878-128">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="f0878-128">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="f0878-129">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="f0878-129">`az` command not found</span></span>

<span data-ttu-id="f0878-130">Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="f0878-130">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="f0878-131">Run (Запустить)</span><span class="sxs-lookup"><span data-stu-id="f0878-131">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="f0878-132">и проверьте, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="f0878-132">and check if the problem is resolved.</span></span>

<span data-ttu-id="f0878-133">Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="f0878-133">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="f0878-134">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="f0878-134">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="f0878-135">Расположение команды `az`:</span><span class="sxs-lookup"><span data-stu-id="f0878-135">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="f0878-136">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="f0878-136">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="f0878-137">Чтобы вы могли получить скрипты установки, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="f0878-137">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="f0878-138">Конечные точки, используемые диспетчером пакетов дистрибутива (при его наличии) для основных пакетов</span><span class="sxs-lookup"><span data-stu-id="f0878-138">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="f0878-139">Удаление</span><span class="sxs-lookup"><span data-stu-id="f0878-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f0878-140">Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке.</span><span class="sxs-lookup"><span data-stu-id="f0878-140">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="f0878-141">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="f0878-141">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="f0878-142">Удалите установленные файлы CLI.</span><span class="sxs-lookup"><span data-stu-id="f0878-142">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="f0878-143">Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:</span><span class="sxs-lookup"><span data-stu-id="f0878-143">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="f0878-144">При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="f0878-144">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="f0878-145">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f0878-145">Next Steps</span></span>

<span data-ttu-id="f0878-146">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="f0878-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f0878-147">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f0878-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
