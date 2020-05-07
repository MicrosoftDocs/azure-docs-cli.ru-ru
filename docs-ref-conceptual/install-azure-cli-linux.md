---
title: Установка Azure CLI для Linux вручную
description: Как установить Azure CLI в Linux вручную
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9a98da54f397c1fd03a7cc6b581a769afe84ef88
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779590"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="0bffb-103">Установка Azure CLI в Linux вручную</span><span class="sxs-lookup"><span data-stu-id="0bffb-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="0bffb-104">Если для вашего дистрибутива отсутствует пакет Azure CLI, установите CLI вручную, выполнив скрипт.</span><span class="sxs-lookup"><span data-stu-id="0bffb-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="0bffb-105">Настоятельно рекомендуется устанавливать CLI с помощью диспетчера пакетов.</span><span class="sxs-lookup"><span data-stu-id="0bffb-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="0bffb-106">Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI.</span><span class="sxs-lookup"><span data-stu-id="0bffb-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="0bffb-107">Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="0bffb-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bffb-108">предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0bffb-108">Prerequisites</span></span>

<span data-ttu-id="0bffb-109">Для использования CLI требуется следующее ПО:</span><span class="sxs-lookup"><span data-stu-id="0bffb-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="0bffb-110">[Python 3.6.x, 3.7.x или 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="0bffb-110">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="0bffb-111">libffi</span><span class="sxs-lookup"><span data-stu-id="0bffb-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="0bffb-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="0bffb-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="0bffb-113">Начиная с версии `2.1.0`, в CLI прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="0bffb-113">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="0bffb-114">Новые версии больше не будут гарантированно работать при использовании Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="0bffb-114">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="0bffb-115">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="0bffb-115">Install or update</span></span>

<span data-ttu-id="0bffb-116">Для установки и обновления CLI требуется повторный запуск установочного скрипта.</span><span class="sxs-lookup"><span data-stu-id="0bffb-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="0bffb-117">Установите CLI, выполнив `curl`.</span><span class="sxs-lookup"><span data-stu-id="0bffb-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="0bffb-118">Скрипт также можно скачать и выполнить на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="0bffb-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="0bffb-119">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="0bffb-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="0bffb-120">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="0bffb-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="0bffb-121">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="0bffb-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0bffb-122">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0bffb-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0bffb-123">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="0bffb-123">Troubleshooting</span></span>

<span data-ttu-id="0bffb-124">Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную.</span><span class="sxs-lookup"><span data-stu-id="0bffb-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="0bffb-125">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="0bffb-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="0bffb-126">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="0bffb-126">curl "Object Moved" error</span></span>

<span data-ttu-id="0bffb-127">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="0bffb-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="0bffb-128">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="0bffb-128">`az` command not found</span></span>

<span data-ttu-id="0bffb-129">Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="0bffb-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="0bffb-130">Run (Запустить)</span><span class="sxs-lookup"><span data-stu-id="0bffb-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="0bffb-131">и проверьте, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="0bffb-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="0bffb-132">Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="0bffb-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="0bffb-133">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="0bffb-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="0bffb-134">Расположение команды `az`:</span><span class="sxs-lookup"><span data-stu-id="0bffb-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="0bffb-135">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="0bffb-135">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="0bffb-136">Чтобы вы могли получить скрипты установки, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="0bffb-136">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="0bffb-137">Конечные точки, используемые диспетчером пакетов дистрибутива (при его наличии) для основных пакетов</span><span class="sxs-lookup"><span data-stu-id="0bffb-137">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="0bffb-138">Удаление</span><span class="sxs-lookup"><span data-stu-id="0bffb-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0bffb-139">Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке.</span><span class="sxs-lookup"><span data-stu-id="0bffb-139">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="0bffb-140">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="0bffb-140">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="0bffb-141">Удалите установленные файлы CLI.</span><span class="sxs-lookup"><span data-stu-id="0bffb-141">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="0bffb-142">Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:</span><span class="sxs-lookup"><span data-stu-id="0bffb-142">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="0bffb-143">При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="0bffb-143">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="0bffb-144">Next Steps</span><span class="sxs-lookup"><span data-stu-id="0bffb-144">Next Steps</span></span>

<span data-ttu-id="0bffb-145">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="0bffb-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0bffb-146">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="0bffb-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
