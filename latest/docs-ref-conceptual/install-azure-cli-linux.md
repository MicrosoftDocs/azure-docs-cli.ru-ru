---
title: "Установка Azure CLI 2.0 для Linux вручную"
description: "Как установить Azure CLI 2.0 в Linux вручную"
keywords: Azure CLI,Install Azure CLI,azure linux, azure install linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="df68b-104">Установка Azure CLI 2.0 в Linux вручную</span><span class="sxs-lookup"><span data-stu-id="df68b-104">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="df68b-105">Если в вашем диспетчере пакетов нет доступного пакета для Azure CLI, вы всегда можете установить CLI вручную, запустив скрипт установки.</span><span class="sxs-lookup"><span data-stu-id="df68b-105">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manualy by running an installation script.</span></span> <span data-ttu-id="df68b-106">Установка с помощью доступного пакета является рекомендуемым способом.</span><span class="sxs-lookup"><span data-stu-id="df68b-106">If you do have a package available, that is always the recommended installation method.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df68b-107">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="df68b-107">Prerequisites</span></span>

<span data-ttu-id="df68b-108">Для установки CLI в системе должно быть следующее программное обеспечение:</span><span class="sxs-lookup"><span data-stu-id="df68b-108">In order to install the CLI, you will need the following software available on your system:</span></span>

* [<span data-ttu-id="df68b-109">Python 2.7 или Python 3.x</span><span class="sxs-lookup"><span data-stu-id="df68b-109">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="df68b-110">libffi</span><span class="sxs-lookup"><span data-stu-id="df68b-110">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="df68b-111">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="df68b-111">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a><span data-ttu-id="df68b-112">Установка или обновление вручную</span><span class="sxs-lookup"><span data-stu-id="df68b-112">Install or update manually</span></span>

<span data-ttu-id="df68b-113">При установке или обновлении CLI необходимо выполнить полную установку.</span><span class="sxs-lookup"><span data-stu-id="df68b-113">Whether you are installing or updating the CLI, you will need to perform a full installation.</span></span> <span data-ttu-id="df68b-114">При наличии необходимых компонентов установите CLI, выполнив команду `curl`.</span><span class="sxs-lookup"><span data-stu-id="df68b-114">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="df68b-115">При необходимости (или если вы не можете выполнить `curl` в системе) можно скачать скрипт и запустить его локально.</span><span class="sxs-lookup"><span data-stu-id="df68b-115">If you would prefer, or do not have `curl` on your system, you can download the script and run it locally instead.</span></span> <span data-ttu-id="df68b-116">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="df68b-116">You may have to restart your shell in order for changes to take effect.</span></span> <span data-ttu-id="df68b-117">Когда установка будет завершена, запустите CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="df68b-117">After installation, run the CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="df68b-118">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="df68b-118">Troubleshooting</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="df68b-119">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="df68b-119">curl "Object Moved" error</span></span>

<span data-ttu-id="df68b-120">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="df68b-120">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="df68b-121">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="df68b-121">`az` command not found</span></span>

<span data-ttu-id="df68b-122">Если вы не можете выполнить эту команду после установки, может потребоваться очистить кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="df68b-122">After installation if you can't run the command, you may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="df68b-123">Выполнить</span><span class="sxs-lookup"><span data-stu-id="df68b-123">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="df68b-124">и посмотрите, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="df68b-124">and see if the problem is resolved.</span></span>

<span data-ttu-id="df68b-125">Это также может произойти, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="df68b-125">This can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="df68b-126">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="df68b-126">Make sure that the location of the `az` command is in your `$PATH`.</span></span>

<span data-ttu-id="df68b-127">Если вы запустили сценарий установки, результат будет таким:</span><span class="sxs-lookup"><span data-stu-id="df68b-127">If you ran the installation script, this will be:</span></span>

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a><span data-ttu-id="df68b-128">Удаление вручную</span><span class="sxs-lookup"><span data-stu-id="df68b-128">Unstinall manually</span></span>

<span data-ttu-id="df68b-129">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="df68b-129">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="df68b-130">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="df68b-130">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="df68b-131">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="df68b-131">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="df68b-132">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="df68b-132">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="df68b-133">CLI можно удалить, удалив файлы непосредственно из расположения установки.</span><span class="sxs-lookup"><span data-stu-id="df68b-133">You can uninstall the CLI by directly deleting the files from the install location.</span></span> <span data-ttu-id="df68b-134">Если используется скрипт `https://aka.ms/InstallAzureCLI`, расположение установки следует выбрать во время установки.</span><span class="sxs-lookup"><span data-stu-id="df68b-134">Your install location should have been chosen at the time of install, if you installed via the `https://aka.ms/InstallAzureCLI` script.</span></span> <span data-ttu-id="df68b-135">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="df68b-135">The default installation location is `$HOME`.</span></span>

<span data-ttu-id="df68b-136">Во-первых, удалите установленные файлы CLI:</span><span class="sxs-lookup"><span data-stu-id="df68b-136">First, remove the installed CLI files:</span></span>

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

<span data-ttu-id="df68b-137">Затем измените файл `$HOME/.bash_profile`, чтобы удалить строку:</span><span class="sxs-lookup"><span data-stu-id="df68b-137">Then modify your `$HOME/.bash_profile` file to remove the line:</span></span>

```
<install location>/lib/azure-cli/az.completion
```

<span data-ttu-id="df68b-138">И, наконец, перезагрузите кэш команд в оболочке (если он используется).</span><span class="sxs-lookup"><span data-stu-id="df68b-138">And finally, reload your shell's command cache if it uses one.</span></span> <span data-ttu-id="df68b-139">Пользователям `bash` и `zsh` необходимо выполнить этот шаг:</span><span class="sxs-lookup"><span data-stu-id="df68b-139">`bash` and `zsh` users will need to perform this step:</span></span>

```bash
hash -r
```
