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
ms.openlocfilehash: 229b109b307453c87abf260a66084c94ced33d81
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422006"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="5a27c-103">Установка Azure CLI в Linux вручную</span><span class="sxs-lookup"><span data-stu-id="5a27c-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="5a27c-104">Если для вашего дистрибутива отсутствует пакет Azure CLI, установите CLI вручную, выполнив скрипт.</span><span class="sxs-lookup"><span data-stu-id="5a27c-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="5a27c-105">Настоятельно рекомендуется устанавливать CLI с помощью диспетчера пакетов.</span><span class="sxs-lookup"><span data-stu-id="5a27c-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="5a27c-106">Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI.</span><span class="sxs-lookup"><span data-stu-id="5a27c-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="5a27c-107">Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="5a27c-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a27c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5a27c-108">Prerequisites</span></span>

<span data-ttu-id="5a27c-109">Для использования CLI требуется следующее ПО:</span><span class="sxs-lookup"><span data-stu-id="5a27c-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="5a27c-110">[Python версии 3.6.x или 3.7.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="5a27c-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="5a27c-111">libffi</span><span class="sxs-lookup"><span data-stu-id="5a27c-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="5a27c-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="5a27c-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="5a27c-113">Интерфейс CLI также совместим с Python 2.7.x, поддержка которого прекращается 1 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="5a27c-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="5a27c-114">Поэтому мы рекомендуем установить для CLI Python 3.</span><span class="sxs-lookup"><span data-stu-id="5a27c-114">For this reason we recommend that you install Python 3 to run the CLI.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="5a27c-115">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="5a27c-115">Install or update</span></span>

<span data-ttu-id="5a27c-116">Для установки и обновления CLI требуется повторный запуск установочного скрипта.</span><span class="sxs-lookup"><span data-stu-id="5a27c-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="5a27c-117">Установите CLI, выполнив `curl`.</span><span class="sxs-lookup"><span data-stu-id="5a27c-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="5a27c-118">Скрипт также можно скачать и выполнить на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="5a27c-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="5a27c-119">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="5a27c-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="5a27c-120">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="5a27c-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="5a27c-121">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5a27c-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5a27c-122">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5a27c-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5a27c-123">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5a27c-123">Troubleshooting</span></span>

<span data-ttu-id="5a27c-124">Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную.</span><span class="sxs-lookup"><span data-stu-id="5a27c-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="5a27c-125">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5a27c-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="5a27c-126">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="5a27c-126">curl "Object Moved" error</span></span>

<span data-ttu-id="5a27c-127">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="5a27c-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="5a27c-128">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="5a27c-128">`az` command not found</span></span>

<span data-ttu-id="5a27c-129">Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="5a27c-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="5a27c-130">Run (Запустить)</span><span class="sxs-lookup"><span data-stu-id="5a27c-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="5a27c-131">и проверьте, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="5a27c-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="5a27c-132">Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="5a27c-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="5a27c-133">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="5a27c-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="5a27c-134">Расположение команды `az`:</span><span class="sxs-lookup"><span data-stu-id="5a27c-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="5a27c-135">Удаление</span><span class="sxs-lookup"><span data-stu-id="5a27c-135">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="5a27c-136">Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке.</span><span class="sxs-lookup"><span data-stu-id="5a27c-136">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="5a27c-137">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="5a27c-137">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="5a27c-138">Удалите установленные файлы CLI.</span><span class="sxs-lookup"><span data-stu-id="5a27c-138">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="5a27c-139">Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:</span><span class="sxs-lookup"><span data-stu-id="5a27c-139">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="5a27c-140">При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="5a27c-140">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="5a27c-141">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5a27c-141">Next Steps</span></span>

<span data-ttu-id="5a27c-142">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="5a27c-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5a27c-143">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5a27c-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
