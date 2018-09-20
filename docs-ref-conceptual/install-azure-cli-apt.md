---
title: Установка Azure CLI 2.0 в Linux с помощью apt
description: Как установить Azure CLI 2.0 с помощью apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 88b4570f62858ec1e12898aea51a5dbce6d677b5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388428"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="b2ebc-103">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="b2ebc-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="b2ebc-104">Если вы используете дистрибутив, включающий `apt`, например Ubuntu ил Debian, доступен 64-разрядный пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="b2ebc-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="b2ebc-105">This package has been tested with:</span></span>

* <span data-ttu-id="b2ebc-106">Ubuntu trusty, xenial, artful и bionic</span><span class="sxs-lookup"><span data-stu-id="b2ebc-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="b2ebc-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="b2ebc-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="b2ebc-108">Install</span><span class="sxs-lookup"><span data-stu-id="b2ebc-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="b2ebc-109">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-109">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="b2ebc-110">Получите ключ подписывания Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="b2ebc-111">Установите интерфейс командной строки.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="b2ebc-112">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="b2ebc-113">Если возникли ошибки с ключом подписывания, убедитесь, что вы [получили ключ подписывания последней версии](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="b2ebc-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="b2ebc-115">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="b2ebc-116">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-116">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b2ebc-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b2ebc-117">Troubleshooting</span></span>

<span data-ttu-id="b2ebc-118">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="b2ebc-119">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="b2ebc-120">Выполнение lsb_release завершается ошибкой "Команда не найдена"</span><span class="sxs-lookup"><span data-stu-id="b2ebc-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="b2ebc-121">При выполнении команды `lsb_release` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="b2ebc-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="b2ebc-122">Эта ошибка возникла, так как команда `lsb_release` не установлена.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-122">The error is due to the `lsb_release` command not being installed.</span></span> <span data-ttu-id="b2ebc-123">Ошибку можно устранить, установив пакет `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="b2ebc-124">lsb_release не возвращает версию основного дистрибутива</span><span class="sxs-lookup"><span data-stu-id="b2ebc-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="b2ebc-125">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="b2ebc-126">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="b2ebc-127">Если известно, на основе какой версии создан дистрибутив, можно установить значение параметра `AZ_REPO` вручную на [первом шаге установки](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="b2ebc-128">В противном случае найдите информацию о том, как определить имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="b2ebc-129">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="b2ebc-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="b2ebc-130">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="b2ebc-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="b2ebc-131">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="b2ebc-132">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="b2ebc-133">Зависает apt-key</span><span class="sxs-lookup"><span data-stu-id="b2ebc-133">apt-key hangs</span></span>

<span data-ttu-id="b2ebc-134">Если при использовании брандмауэра блокируются исходящие подключения к порту 11371, команда `apt-key` может перестать работать на неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="b2ebc-135">Возможно, брандмауэр требует использовать для исходящих подключений прокси-сервер HTTP:</span><span class="sxs-lookup"><span data-stu-id="b2ebc-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="b2ebc-136">Чтобы определить, используется ли у вас прокси-сервер, обратитесь к своему системному администратору.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-136">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="b2ebc-137">Если прокси-сервер не требует имени для входа, не указывайте имя пользователя, пароль и маркер `@`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-137">If your proxy does not require a login, then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="b2ebc-138">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="b2ebc-138">Update</span></span>

<span data-ttu-id="b2ebc-139">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="b2ebc-140">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="b2ebc-141">Если возникли ошибки с ключом подписывания, убедитесь, что вы [получили ключ подписывания последней версии](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="b2ebc-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="b2ebc-142">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="b2ebc-143">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="b2ebc-144">Удаление</span><span class="sxs-lookup"><span data-stu-id="b2ebc-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b2ebc-145">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="b2ebc-146">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-146">If you don't plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="b2ebc-147">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="b2ebc-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
