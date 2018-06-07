---
title: Установка Azure CLI 2.0 для Linux вручную
description: Как установить Azure CLI 2.0 в Linux вручную
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b11ab99626227cb53a604d429fa32c560e4255d9
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703134"
---
# <a name="install-azure-cli-20-on-linux-manually"></a><span data-ttu-id="9c5b6-103">Установка Azure CLI 2.0 в Linux вручную</span><span class="sxs-lookup"><span data-stu-id="9c5b6-103">Install Azure CLI 2.0 on Linux manually</span></span>

<span data-ttu-id="9c5b6-104">Если в вашем диспетчере пакетов нет доступного пакета для Azure CLI, вы всегда можете установить CLI вручную, запустив скрипт установки.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-104">If you do not have a package for the Azure CLI available on your distribution, you can always install the CLI manually by running an installation script.</span></span>

> [!NOTE]
> <span data-ttu-id="9c5b6-105">Настоятельно рекомендуем использовать для CLI диспетчер пакетов.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-105">It's strongly recommend that you use a package manager for the CLI.</span></span> <span data-ttu-id="9c5b6-106">Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="9c5b6-107">Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c5b6-108">предварительным требованиям</span><span class="sxs-lookup"><span data-stu-id="9c5b6-108">Prerequisites</span></span>

<span data-ttu-id="9c5b6-109">Для установки CLI в системе должно быть следующее программное обеспечение:</span><span class="sxs-lookup"><span data-stu-id="9c5b6-109">In order to install the CLI, you need the following software available on your system:</span></span>

* [<span data-ttu-id="9c5b6-110">Python 2.7 или Python 3.x</span><span class="sxs-lookup"><span data-stu-id="9c5b6-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="9c5b6-111">libffi</span><span class="sxs-lookup"><span data-stu-id="9c5b6-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="9c5b6-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="9c5b6-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="9c5b6-113">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="9c5b6-113">Install or update</span></span>

<span data-ttu-id="9c5b6-114">При установке или обновлении CLI необходимо выполнить полную установку.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-114">Whether you are installing or updating the CLI, you need to perform a full installation.</span></span> <span data-ttu-id="9c5b6-115">При наличии необходимых компонентов установите CLI, выполнив команду `curl`.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-115">Once you have the prerequisites, you can install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="9c5b6-116">Либо же вы можете скачать скрипт и запустить его локально.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-116">You can also download the script and run it locally instead.</span></span> <span data-ttu-id="9c5b6-117">Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-117">You may have to restart your shell in order for changes to take effect.</span></span> 

<span data-ttu-id="9c5b6-118">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="9c5b6-119">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-119">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="9c5b6-120">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9c5b6-120">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="9c5b6-121">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="9c5b6-121">Troubleshooting</span></span>

<span data-ttu-id="9c5b6-122">Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="9c5b6-123">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="9c5b6-123">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>
### <a name="curl-object-moved-error"></a><span data-ttu-id="9c5b6-124">Ошибка "Объект перемещен" при выполнении команды curl</span><span class="sxs-lookup"><span data-stu-id="9c5b6-124">curl "Object Moved" error</span></span>

<span data-ttu-id="9c5b6-125">Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:</span><span class="sxs-lookup"><span data-stu-id="9c5b6-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="9c5b6-126">Команда `az` не найдена</span><span class="sxs-lookup"><span data-stu-id="9c5b6-126">`az` command not found</span></span>

<span data-ttu-id="9c5b6-127">Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="9c5b6-128">Выполнить</span><span class="sxs-lookup"><span data-stu-id="9c5b6-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="9c5b6-129">и проверьте, будет ли устранена проблема.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="9c5b6-130">Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-130">The issue can also occur if you did not restart your shell after installation.</span></span> <span data-ttu-id="9c5b6-131">Убедитесь, что команда `az` добавлена в переменную `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="9c5b6-132">Расположение команды `az`:</span><span class="sxs-lookup"><span data-stu-id="9c5b6-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="9c5b6-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="9c5b6-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9c5b6-134">Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="9c5b6-135">Расположение установки по умолчанию — `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="9c5b6-136">Удалите установленные файлы CLI.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-136">Remove the installed CLI files.</span></span>

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. <span data-ttu-id="9c5b6-137">Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:</span><span class="sxs-lookup"><span data-stu-id="9c5b6-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. <span data-ttu-id="9c5b6-138">При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.</span><span class="sxs-lookup"><span data-stu-id="9c5b6-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

  ```bash
  hash -r
  ```
