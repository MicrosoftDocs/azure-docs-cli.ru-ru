---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 31b6a6e1c4c987ea351ccebc5d5bf23313ed856f
ms.sourcegitcommit: 547d3db8a1469f11d33e738a82d96cb51de61bd6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "98147468"
---
## <a name="overview"></a><span data-ttu-id="2a0e7-101">Обзор</span><span class="sxs-lookup"><span data-stu-id="2a0e7-101">Overview</span></span>

<span data-ttu-id="2a0e7-102">Диспетчер пакетов `apt` содержит пакет x86_64 для Azure CLI, протестированный в следующих дистрибутивах.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-102">The `apt` package manager contains an x86_64 package for the Azure CLI that has been tested on the following distributions.</span></span>

| <span data-ttu-id="2a0e7-103">Distribution</span><span class="sxs-lookup"><span data-stu-id="2a0e7-103">Distribution</span></span> | <span data-ttu-id="2a0e7-104">Версия</span><span class="sxs-lookup"><span data-stu-id="2a0e7-104">Version</span></span> |
|:-------------|:--------|
| <span data-ttu-id="2a0e7-105">Ubuntu</span><span class="sxs-lookup"><span data-stu-id="2a0e7-105">Ubuntu</span></span>       | <span data-ttu-id="2a0e7-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span><span class="sxs-lookup"><span data-stu-id="2a0e7-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span></span> |
| <span data-ttu-id="2a0e7-107">Debian</span><span class="sxs-lookup"><span data-stu-id="2a0e7-107">Debian</span></span>       | <span data-ttu-id="2a0e7-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span><span class="sxs-lookup"><span data-stu-id="2a0e7-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span></span> |

> [!WARNING]
> <span data-ttu-id="2a0e7-109">Для Ubuntu 20.04 (Focal Fossa) и 20.10 (Groovy Gorilla) доступен пакет `azure-cli` с версией `2.0.81`, предоставляемый репозиторием `universe`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-109">Ubuntu 20.04 (Focal Fossa) and 20.10 (Groovy Gorilla) include an `azure-cli` package with version `2.0.81` provided by the `universe` repository.</span></span> <span data-ttu-id="2a0e7-110">Этот пакет устарел и не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-110">This package is outdated and not recommended.</span></span> <span data-ttu-id="2a0e7-111">Если этот пакет установлен, удалите его, прежде чем продолжать работу, выполнив команду `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-111">If this package is installed, remove the package before continuing by running the command `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span></span>

## <a name="installation-options"></a><span data-ttu-id="2a0e7-112">Варианты установки</span><span class="sxs-lookup"><span data-stu-id="2a0e7-112">Installation Options</span></span>

<span data-ttu-id="2a0e7-113">Есть два варианта установки Azure CLI в системе.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-113">There are two options to install the Azure CLI on your system.</span></span>  <span data-ttu-id="2a0e7-114">Во-первых, вы можете выполнить одну команду, которая скачает скрипт установки и выполнит команды установки.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-114">First, you may execute a single command that will download an install script and run the install commands for you.</span></span>  <span data-ttu-id="2a0e7-115">Или же вы можете выполнить пошаговый процесс установки самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-115">Or if you prefer, you can execute the install commands yourself in a step-by-step process.</span></span>  <span data-ttu-id="2a0e7-116">Оба метода описаны ниже.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-116">Both methods are provided below.</span></span>

## <a name="option-1-install-with-one-command"></a><span data-ttu-id="2a0e7-117">Вариант 1. Установка с помощью одной команды</span><span class="sxs-lookup"><span data-stu-id="2a0e7-117">Option 1: Install with one command</span></span>

<span data-ttu-id="2a0e7-118">Команда Azure CLI предоставляет скрипт для выполнения всех команд установки за один шаг.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-118">The Azure CLI team maintains a script to run all installation commands in one step.</span></span>  <span data-ttu-id="2a0e7-119">Этот скрипт скачивается с помощью `curl` и передается непосредственно в `bash` для установки CLI.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-119">This script is downloaded via `curl` and piped directly to `bash` to install the CLI.</span></span>

<span data-ttu-id="2a0e7-120">Если вы хотите проверить содержимое скрипта перед выполнением, просто скачайте скрипт с помощью `curl` и откройте его в любом текстовом редакторе.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-120">If you wish to inspect the contents of the script yourself before executing, simply download the script first using `curl` and inspect it in your favorite text editor.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a><span data-ttu-id="2a0e7-121">Вариант 2. Пошаговые инструкции по установке</span><span class="sxs-lookup"><span data-stu-id="2a0e7-121">Option 2: Step-by-step installation instructions</span></span>

<span data-ttu-id="2a0e7-122">Если вы предпочитаете пошаговый процесс установки, выполните следующие действия, чтобы установить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-122">If you prefer a step-by-step installation process, complete the following steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="2a0e7-123">Получение пакетов, необходимых для процесса установки:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-123">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="2a0e7-124">Скачайте и установите ключ подписывания (Майкрософт):</span><span class="sxs-lookup"><span data-stu-id="2a0e7-124">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="2a0e7-125">Добавьте репозиторий программного обеспечения Azure CLI (пропустите этот шаг для дистрибутивов Linux ARM64):</span><span class="sxs-lookup"><span data-stu-id="2a0e7-125">Add the Azure CLI software repository (skip this step on ARM64 Linux distributions):</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="2a0e7-126">Обновите сведения о репозитории и установите пакет `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-126">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a><span data-ttu-id="2a0e7-127">Вход с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2a0e7-127">Sign in to Azure with the Azure CLI</span></span>

<span data-ttu-id="2a0e7-128">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-128">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2a0e7-129">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="2a0e7-129">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="2a0e7-130">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2a0e7-130">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2a0e7-131">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="2a0e7-131">Troubleshooting</span></span>

<span data-ttu-id="2a0e7-132">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-132">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="2a0e7-133">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2a0e7-133">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="2a0e7-134">Проблема с отсутствием модуля в Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="2a0e7-134">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>

<span data-ttu-id="2a0e7-135">Если вы установили `azure-cli` в выпуске `Focal`, не добавив репозиторий программного обеспечения Azure CLI, как предписывает [шаг 3](#set-release) инструкций по установке вручную, или с помощью нашего [скрипта](#option-1-install-with-one-command), могут возникнуть проблемы, например с отсутствием модуля с именем decorator или antlr4, так как установленный вами пакет является устаревшим пакетом `azure-cli 2.0.81` из репозитория `focal/universe`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-135">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#option-1-install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="2a0e7-136">Сначала удалите его с помощью команды `sudo apt remove azure-cli -y && sudo apt autoremove -y`, а затем выполните приведенные выше [инструкции](#install), чтобы установить последнюю версию пакета `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-136">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="2a0e7-137">Команда lsb_release не возвращает правильную версию базового дистрибутива</span><span class="sxs-lookup"><span data-stu-id="2a0e7-137">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="2a0e7-138">Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-138">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="2a0e7-139">Это значение используется при установке для определения устанавливаемого пакета.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-139">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="2a0e7-140">Если вы знаете кодовое имя версии Ubuntu или Debian, на основе которой создан ваш дистрибутив, можно установить значение параметра `AZ_REPO` вручную при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2a0e7-140">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2a0e7-141">В противном случае найдите информацию о том, как определить кодовое имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-141">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="2a0e7-142">Для вашего дистрибутива отсутствует пакет</span><span class="sxs-lookup"><span data-stu-id="2a0e7-142">No package for your distribution</span></span>

<span data-ttu-id="2a0e7-143">Иногда между выпуском дистрибутива и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-143">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="2a0e7-144">Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-144">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="2a0e7-145">Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-145">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="2a0e7-146">Для этого вручную установите значение `AZ_REPO` при [добавлении репозитория](#set-release).</span><span class="sxs-lookup"><span data-stu-id="2a0e7-146">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="2a0e7-147">Для дистрибутивов Ubuntu используйте репозиторий `bionic`, а для дистрибутивов Debian используйте репозиторий `stretch`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-147">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="2a0e7-148">Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-148">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="2a0e7-149">В Elementary OS (EOS) не удалось установить Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2a0e7-149">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="2a0e7-150">В EOS не удалось установить Azure CLI, так как `lsb_release` возвращает `HERA`, то есть имя выпуска EOS.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-150">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="2a0e7-151">Чтобы устранить проблему, нужно исправить файл `/etc/apt/sources.list.d/azure-cli.list` и изменить `hera main` на `bionic main`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-151">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="2a0e7-152">Исходное содержимое файла:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-152">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="2a0e7-153">Измененное содержимое файла:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-153">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="2a0e7-154">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="2a0e7-154">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="2a0e7-155">Вы также можете явным образом настроить `apt`, чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-155">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="2a0e7-156">Убедитесь, что следующие строки отображаются в файле конфигурации `apt` в `/etc/apt/apt.conf.d/`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-156">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="2a0e7-157">Мы рекомендуем использовать существующий файл глобальной конфигурации или существующий файл конфигурации прокси-сервера (`40proxies` или `99local`), но вам следует учитывать требования системного администратора.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-157">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="2a0e7-158">Если прокси-сервер не использует обычную аутентификацию, __удалите__ часть `[username]:[password]@` URI прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-158">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="2a0e7-159">См. подробнее о конфигурации прокси-сервера в официальной документации по Ubuntu:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-159">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="2a0e7-160">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="2a0e7-160">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="2a0e7-161">Вики-сайт, посвященный Ubuntu (справочник по команде apt-get)</span><span class="sxs-lookup"><span data-stu-id="2a0e7-161">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="2a0e7-162">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-162">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="2a0e7-163">Update</span><span class="sxs-lookup"><span data-stu-id="2a0e7-163">Update</span></span>
[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="2a0e7-164">Вы также можете обновить пакет CLI с помощью команды `apt-get upgrade`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-164">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="2a0e7-165">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-165">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="2a0e7-166">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-166">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="2a0e7-167">Удаление</span><span class="sxs-lookup"><span data-stu-id="2a0e7-167">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="2a0e7-168">Выполите удаление с помощью команды `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-168">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="2a0e7-169">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-169">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="2a0e7-170">Если вы не используете другие пакеты от корпорации Майкрософт, удалите ключ подписывания.</span><span class="sxs-lookup"><span data-stu-id="2a0e7-170">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="2a0e7-171">Удалите все ненужные пакеты:</span><span class="sxs-lookup"><span data-stu-id="2a0e7-171">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```
