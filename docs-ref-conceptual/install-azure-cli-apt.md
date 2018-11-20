---
title: Установка Azure CLI в Linux с помощью apt
description: Как установить Azure CLI с помощью диспетчера пакетов apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0d4311e88fec9903c1aab1410cc71328f896dc65
ms.sourcegitcommit: 728a050f13d3682122be4a8993596cc4185a45ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2018
ms.locfileid: "51680940"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="194d2-103">Установка Azure CLI с помощью apt</span><span class="sxs-lookup"><span data-stu-id="194d2-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="194d2-104">Если вы используете дистрибутив, включающий `apt`, например Ubuntu ил Debian, доступен 64-разрядный пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="194d2-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="194d2-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="194d2-105">This package has been tested with:</span></span>

* <span data-ttu-id="194d2-106">Ubuntu trusty, xenial, artful и bionic</span><span class="sxs-lookup"><span data-stu-id="194d2-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="194d2-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="194d2-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="194d2-108">Install</span><span class="sxs-lookup"><span data-stu-id="194d2-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="194d2-109">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="194d2-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="194d2-110">Получите ключ подписывания Microsoft.</span><span class="sxs-lookup"><span data-stu-id="194d2-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="194d2-111">Установите интерфейс командной строки.</span><span class="sxs-lookup"><span data-stu-id="194d2-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="194d2-112">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="194d2-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="194d2-113">Если вы получаете сообщения об ошибках подписи, убедитесь, что вы используете [последний ключ подписывания](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="194d2-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="194d2-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="194d2-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="194d2-115">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="194d2-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="194d2-116">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="194d2-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="194d2-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="194d2-117">Troubleshooting</span></span>

<span data-ttu-id="194d2-118">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="194d2-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="194d2-119">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="194d2-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="194d2-120">lsb_release не возвращает версию основного дистрибутива</span><span class="sxs-lookup"><span data-stu-id="194d2-120">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="194d2-121">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="194d2-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="194d2-122">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="194d2-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="194d2-123">Если известно, на основе какой версии создан дистрибутив, можно установить значение параметра `AZ_REPO` вручную на [первом шаге установки](#install-step-1).</span><span class="sxs-lookup"><span data-stu-id="194d2-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="194d2-124">В противном случае найдите информацию о том, как определить имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="194d2-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="194d2-125">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="194d2-125">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="194d2-126">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="194d2-126">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="194d2-127">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="194d2-127">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="194d2-128">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="194d2-128">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="194d2-129">Зависает apt-key</span><span class="sxs-lookup"><span data-stu-id="194d2-129">apt-key hangs</span></span>

<span data-ttu-id="194d2-130">Если при использовании брандмауэра блокируются исходящие подключения к порту 11371, команда `apt-key` может перестать работать на неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="194d2-130">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="194d2-131">Ваш брандмауэр может требовать использования прокси-сервера HTTP для исходящих подключений:</span><span class="sxs-lookup"><span data-stu-id="194d2-131">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="194d2-132">Чтобы определить, используется ли у вас прокси-сервер, обратитесь к своему системному администратору.</span><span class="sxs-lookup"><span data-stu-id="194d2-132">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="194d2-133">Если прокси-сервер не требует входа, не указывайте имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="194d2-133">If your proxy does not require a login, then leave out the user and password information.</span></span>

## <a name="update"></a><span data-ttu-id="194d2-134">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="194d2-134">Update</span></span>

<span data-ttu-id="194d2-135">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="194d2-135">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="194d2-136">Ключ подписывания обновлен и заменен в мае 2018 г.</span><span class="sxs-lookup"><span data-stu-id="194d2-136">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="194d2-137">Если вы получаете сообщения об ошибках подписи, убедитесь, что вы используете [последний ключ подписывания](#signingKey).</span><span class="sxs-lookup"><span data-stu-id="194d2-137">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="194d2-138">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="194d2-138">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="194d2-139">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="194d2-139">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="194d2-140">Удаление</span><span class="sxs-lookup"><span data-stu-id="194d2-140">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="194d2-141">Выполите удаление с помощью команды `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="194d2-141">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="194d2-142">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="194d2-142">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="194d2-143">Удалите ключ подписывания:</span><span class="sxs-lookup"><span data-stu-id="194d2-143">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="194d2-144">Удалите все ненужные пакеты:</span><span class="sxs-lookup"><span data-stu-id="194d2-144">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="194d2-145">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="194d2-145">Next Steps</span></span>

<span data-ttu-id="194d2-146">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="194d2-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="194d2-147">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="194d2-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)