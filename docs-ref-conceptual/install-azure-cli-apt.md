---
title: Установка Azure CLI 2.0 в Linux с помощью apt
description: Как установить Azure CLI 2.0 с помощью apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/24/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7b5835581bf1e14e2d9fdc7c9584c704d1a5d82f
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703185"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="dffa6-103">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="dffa6-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="dffa6-104">Если вы используете дистрибутив, который поставляется с `apt`, например Ubuntu или Debian, можно применить 64-разрядный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="dffa6-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="dffa6-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="dffa6-105">This package has been tested with:</span></span>

* <span data-ttu-id="dffa6-106">Ubuntu wheezy, xenial и artful</span><span class="sxs-lookup"><span data-stu-id="dffa6-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="dffa6-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="dffa6-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="dffa6-108">Install</span><span class="sxs-lookup"><span data-stu-id="dffa6-108">Install</span></span>

1. <span data-ttu-id="dffa6-109"><a name="install-step-1"/> Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="dffa6-109"><a name="install-step-1"/> Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <a name="signingKey"></a><span data-ttu-id="dffa6-110">Получите ключ подписывания Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dffa6-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="dffa6-111">Установите интерфейс командной строки.</span><span class="sxs-lookup"><span data-stu-id="dffa6-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="dffa6-112">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dffa6-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="dffa6-113">Если возникли ошибки с ключом подписывания, убедитесь, что вы [получили ключ подписывания последней версии](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="dffa6-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="dffa6-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="dffa6-115">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="dffa6-116">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="dffa6-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="dffa6-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="dffa6-117">Troubleshooting</span></span>

<span data-ttu-id="dffa6-118">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="dffa6-119">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="dffa6-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="dffa6-120">Выполнение lsb_release завершается ошибкой "Команда не найдена"</span><span class="sxs-lookup"><span data-stu-id="dffa6-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="dffa6-121">При выполнении команды `lsb_release` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="dffa6-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="dffa6-122">Ошибка возникает из-за отсутствия установки lsb_release.</span><span class="sxs-lookup"><span data-stu-id="dffa6-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="dffa6-123">Ошибку можно устранить, установив пакет `lsb-release`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="dffa6-124">lsb_release не возвращает версию основного дистрибутива</span><span class="sxs-lookup"><span data-stu-id="dffa6-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="dffa6-125">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="dffa6-126">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="dffa6-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="dffa6-127">Если известно, на основе какой версии создан дистрибутив, можно установить значение параметра `AZ_REPO` вручную на [первом шаге установки](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="dffa6-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="dffa6-128">В противном случае найдите информацию о том, как определить имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="dffa6-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="dffa6-129">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="dffa6-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="dffa6-130">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="dffa6-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="dffa6-131">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="dffa6-132">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="dffa6-133">Зависает apt-key</span><span class="sxs-lookup"><span data-stu-id="dffa6-133">apt-key hangs</span></span>

<span data-ttu-id="dffa6-134">Если при использовании брандмауэра блокируются исходящие подключения к порту 11371, команда `apt-key` может перестать работать на неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="dffa6-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="dffa6-135">Возможно, брандмауэр требует использовать для исходящих подключений прокси-сервер HTTP:</span><span class="sxs-lookup"><span data-stu-id="dffa6-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="dffa6-136">Если вы не знаете, есть ли у вас прокси-сервер, обратитесь к своему системному администратору.</span><span class="sxs-lookup"><span data-stu-id="dffa6-136">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="dffa6-137">Если для прокси-сервера не требуется имя для входа, не указывайте имя пользователя, пароль и маркер `@`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-137">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="dffa6-138">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="dffa6-138">Update</span></span>

<span data-ttu-id="dffa6-139">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="dffa6-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="dffa6-140">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dffa6-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="dffa6-141">Если возникли ошибки с ключом подписывания, убедитесь, что вы [получили ключ подписывания последней версии](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="dffa6-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
   
> [!NOTE]
> <span data-ttu-id="dffa6-142">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="dffa6-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="dffa6-143">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="dffa6-144">Удаление</span><span class="sxs-lookup"><span data-stu-id="dffa6-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="dffa6-145">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="dffa6-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="dffa6-146">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="dffa6-146">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="dffa6-147">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="dffa6-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
