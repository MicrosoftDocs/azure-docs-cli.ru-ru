---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2cba7031b3fe4c54edcb7c0dcef6f37b97d2f785
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744622"
---
## <a name="overview"></a><span data-ttu-id="aa8d6-101">Обзор</span><span class="sxs-lookup"><span data-stu-id="aa8d6-101">Overview</span></span>

> [!NOTE]
> <span data-ttu-id="aa8d6-102">Настоятельно рекомендуется устанавливать CLI с помощью диспетчера пакетов.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-102">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="aa8d6-103">Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-103">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="aa8d6-104">Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-104">Check and see if there is a package for your distribution before installing manually.</span></span>

<span data-ttu-id="aa8d6-105">Для использования CLI требуется следующее ПО:</span><span class="sxs-lookup"><span data-stu-id="aa8d6-105">The CLI requires the following software:</span></span>

* <span data-ttu-id="aa8d6-106">[Python 3.6.x, 3.7.x или 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="aa8d6-106">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span>
* [<span data-ttu-id="aa8d6-107">libffi</span><span class="sxs-lookup"><span data-stu-id="aa8d6-107">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="aa8d6-108">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="aa8d6-108">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="aa8d6-109">Начиная с версии `2.1.0`, в CLI прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-109">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="aa8d6-110">Новые версии больше не будут гарантированно работать при использовании Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-110">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="aa8d6-111">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="aa8d6-111">Install or update</span></span>

<span data-ttu-id="aa8d6-112">Для установки и обновления CLI требуется повторный запуск установочного скрипта.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-112">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="aa8d6-113">Установите CLI, выполнив `curl`.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-113">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="aa8d6-114">Скрипт также можно скачать и выполнить на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-114">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="aa8d6-115">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-115">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="aa8d6-116">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="aa8d6-117">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="aa8d6-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="aa8d6-118">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="aa8d6-118">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="aa8d6-119">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="aa8d6-119">Troubleshooting</span></span>

<span data-ttu-id="aa8d6-120">Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-120">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="aa8d6-121">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="aa8d6-121">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="aa8d6-122">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="aa8d6-122">curl "Object Moved" error</span></span>

<span data-ttu-id="aa8d6-123">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="aa8d6-123">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="aa8d6-124">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="aa8d6-124">`az` command not found</span></span>

<span data-ttu-id="aa8d6-125">Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-125">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="aa8d6-126">Выполнить</span><span class="sxs-lookup"><span data-stu-id="aa8d6-126">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="aa8d6-127">и проверьте, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-127">and check if the problem is resolved.</span></span>

<span data-ttu-id="aa8d6-128">Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-128">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="aa8d6-129">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-129">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="aa8d6-130">Расположение команды `az`:</span><span class="sxs-lookup"><span data-stu-id="aa8d6-130">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="aa8d6-131">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="aa8d6-131">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="aa8d6-132">Чтобы вы могли получить скрипты установки, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="aa8d6-132">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="aa8d6-133">Конечные точки, используемые диспетчером пакетов дистрибутива (при его наличии) для основных пакетов</span><span class="sxs-lookup"><span data-stu-id="aa8d6-133">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="aa8d6-134">Удаление</span><span class="sxs-lookup"><span data-stu-id="aa8d6-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

<span data-ttu-id="aa8d6-135">Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-135">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="aa8d6-136">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-136">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="aa8d6-137">Удалите установленные файлы CLI.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-137">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="aa8d6-138">Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:</span><span class="sxs-lookup"><span data-stu-id="aa8d6-138">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="aa8d6-139">При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="aa8d6-139">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```