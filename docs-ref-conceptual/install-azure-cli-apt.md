---
title: Установка Azure CLI в Linux с помощью apt
description: Как установить Azure CLI с помощью диспетчера пакетов apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476262"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="f7ddd-103">Установка Azure CLI с помощью apt</span><span class="sxs-lookup"><span data-stu-id="f7ddd-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="f7ddd-104">Если вы используете дистрибутив, включающий `apt`, например Ubuntu или Debian, доступен пакет Azure CLI x86_64.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="f7ddd-105">Этот пакет протестирован и поддерживается для:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="f7ddd-106">Ubuntu Trusty, Xenial, Artful, Bionic и Disco.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-106">Ubuntu trusty, xenial, artful, bionic, and disco</span></span>
* <span data-ttu-id="f7ddd-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="f7ddd-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="f7ddd-108">Пакет для Azure CLI устанавливает собственный интерпретатор Python и не использует системный Python.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="f7ddd-109">Install</span><span class="sxs-lookup"><span data-stu-id="f7ddd-109">Install</span></span>

<span data-ttu-id="f7ddd-110">Мы предлагаем два способа установки Azure CLI с дистрибутивами, которые поддерживают `apt`: комплексный скрипт, который автоматически выполняет команды установки, и инструкции, которые вы сами можете выполнять поэтапно.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-110">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="f7ddd-111">Установка с помощью одной команды</span><span class="sxs-lookup"><span data-stu-id="f7ddd-111">Install with one command</span></span>

<span data-ttu-id="f7ddd-112">Мы предлагаем и поддерживаем скрипт, который выполняет все команды установки за один шаг.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-112">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="f7ddd-113">Запустите его с помощью `curl` и передайте непосредственно в `bash` или скачайте скрипт в файл и проверьте его перед запуском.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-113">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f7ddd-114">Этот скрипт протестирован только для Ubuntu 16.04+ и Debian 8+.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-114">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="f7ddd-115">Он может не работать в других дистрибутивах.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-115">It may not work on other distributions.</span></span>
> <span data-ttu-id="f7ddd-116">Если вы используете производный дистрибутив, например Linux Mint, следуйте инструкциям по установке вручную и выполните необходимые действия для устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-116">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="f7ddd-117">Инструкции по установке вручную</span><span class="sxs-lookup"><span data-stu-id="f7ddd-117">Manual install instructions</span></span>

<span data-ttu-id="f7ddd-118">Если вы не хотите запускать скрипт как суперпользователь, воспользуйтесь приведенными ниже инструкциями, чтобы установить Azure CLI вручную.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-118">If you don't want to run a script as superuser, follow these manual steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="f7ddd-119">Получите пакеты, необходимые для установки:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-119">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="f7ddd-120">Скачайте и установите ключ подписывания (Майкрософт):</span><span class="sxs-lookup"><span data-stu-id="f7ddd-120">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="f7ddd-121">Добавьте репозиторий программного обеспечения Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-121">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="f7ddd-122">Обновите сведения о репозитории и установите пакет `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-122">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="f7ddd-123">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-123">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f7ddd-124">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="f7ddd-124">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f7ddd-125">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f7ddd-125">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f7ddd-126">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="f7ddd-126">Troubleshooting</span></span>

<span data-ttu-id="f7ddd-127">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-127">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="f7ddd-128">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f7ddd-128">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="f7ddd-129">Команда lsb_release не возвращает правильную версию базового дистрибутива</span><span class="sxs-lookup"><span data-stu-id="f7ddd-129">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="f7ddd-130">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-130">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="f7ddd-131">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-131">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="f7ddd-132">Если вы знаете кодовое имя версии Ubuntu или Debian, на основе которой создан ваш дистрибутив, можно установить значение параметра `AZ_REPO` вручную при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="f7ddd-132">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="f7ddd-133">В противном случае найдите информацию о том, как определить кодовое имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-133">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="f7ddd-134">Для вашего дистрибутива отсутствует пакет</span><span class="sxs-lookup"><span data-stu-id="f7ddd-134">No package for your distribution</span></span>

<span data-ttu-id="f7ddd-135">Иногда между выпуском дистрибутива и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-135">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="f7ddd-136">Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-136">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="f7ddd-137">Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-137">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="f7ddd-138">Для этого вручную установите значение `AZ_REPO` при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="f7ddd-138">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="f7ddd-139">Для дистрибутивов Ubuntu используйте репозиторий `disco`, а для дистрибутивов Debian используйте репозиторий `stretch`.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-139">For Ubuntu distributions use the `disco` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="f7ddd-140">Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-140">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="f7ddd-141">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="f7ddd-141">Update</span></span>

<span data-ttu-id="f7ddd-142">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="f7ddd-143">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-143">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="f7ddd-144">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-144">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="f7ddd-145">Удаление</span><span class="sxs-lookup"><span data-stu-id="f7ddd-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="f7ddd-146">Выполите удаление с помощью команды `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-146">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="f7ddd-147">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-147">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="f7ddd-148">Удалите ключ подписывания:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-148">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="f7ddd-149">Удалите все ненужные пакеты:</span><span class="sxs-lookup"><span data-stu-id="f7ddd-149">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="f7ddd-150">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f7ddd-150">Next Steps</span></span>

<span data-ttu-id="f7ddd-151">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="f7ddd-151">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f7ddd-152">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f7ddd-152">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
