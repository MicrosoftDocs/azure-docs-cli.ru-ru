---
title: Установка Azure CLI в Linux с помощью apt
description: Как установить Azure CLI с помощью диспетчера пакетов apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/19/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: fa2e1db439b4836d7506409b3abcce74fb6e6695
ms.sourcegitcommit: 5864f72b9a6fbf82a4d98bf805b3a16a7da18556
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "58343151"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="59528-103">Установка Azure CLI с помощью apt</span><span class="sxs-lookup"><span data-stu-id="59528-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="59528-104">Если вы используете дистрибутив, включающий `apt`, например Ubuntu или Debian, доступен пакет Azure CLI x86_64.</span><span class="sxs-lookup"><span data-stu-id="59528-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="59528-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="59528-105">This package has been tested with:</span></span>

* <span data-ttu-id="59528-106">Ubuntu trusty, xenial, artful и bionic</span><span class="sxs-lookup"><span data-stu-id="59528-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="59528-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="59528-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="59528-108">Пакет для Azure CLI устанавливает собственный интерпретатор Python и не использует системный Python.</span><span class="sxs-lookup"><span data-stu-id="59528-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="59528-109">Install</span><span class="sxs-lookup"><span data-stu-id="59528-109">Install</span></span>

1. <span data-ttu-id="59528-110">Получите пакеты, необходимые для установки:</span><span class="sxs-lookup"><span data-stu-id="59528-110">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gpg
    ```

2. <span data-ttu-id="59528-111">Скачайте и установите ключ подписывания (Майкрософт):</span><span class="sxs-lookup"><span data-stu-id="59528-111">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="59528-112">Добавьте репозиторий программного обеспечения Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="59528-112">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="59528-113">Обновите сведения о репозитории и установите пакет `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="59528-113">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="59528-114">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="59528-114">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="59528-115">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="59528-115">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="59528-116">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="59528-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="59528-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="59528-117">Troubleshooting</span></span>

<span data-ttu-id="59528-118">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="59528-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="59528-119">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="59528-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="59528-120">Команда lsb_release не возвращает правильную версию базового дистрибутива</span><span class="sxs-lookup"><span data-stu-id="59528-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="59528-121">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="59528-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="59528-122">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="59528-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="59528-123">Если вы знаете кодовое имя версии Ubuntu или Debian, на основе которой создан ваш дистрибутив, можно установить значение параметра `AZ_REPO` вручную при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="59528-123">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="59528-124">В противном случае найдите информацию о том, как определить кодовое имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="59528-124">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="59528-125">Для вашего дистрибутива отсутствует пакет</span><span class="sxs-lookup"><span data-stu-id="59528-125">No package for your distribution</span></span>

<span data-ttu-id="59528-126">Иногда между выпуском дистрибутива и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время.</span><span class="sxs-lookup"><span data-stu-id="59528-126">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="59528-127">Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей.</span><span class="sxs-lookup"><span data-stu-id="59528-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="59528-128">Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="59528-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="59528-129">Для этого вручную установите значение `AZ_REPO` при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="59528-129">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="59528-130">Для дистрибутивов Ubuntu используйте репозиторий `bionic`, а для дистрибутивов Debian используйте репозиторий `stretch`.</span><span class="sxs-lookup"><span data-stu-id="59528-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="59528-131">Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="59528-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="59528-132">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="59528-132">Update</span></span>

<span data-ttu-id="59528-133">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="59528-133">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="59528-134">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="59528-134">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="59528-135">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="59528-135">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="59528-136">Удаление</span><span class="sxs-lookup"><span data-stu-id="59528-136">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="59528-137">Выполите удаление с помощью команды `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="59528-137">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="59528-138">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="59528-138">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="59528-139">Удалите ключ подписывания:</span><span class="sxs-lookup"><span data-stu-id="59528-139">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="59528-140">Удалите все ненужные пакеты:</span><span class="sxs-lookup"><span data-stu-id="59528-140">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="59528-141">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="59528-141">Next Steps</span></span>

<span data-ttu-id="59528-142">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="59528-142">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="59528-143">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="59528-143">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
