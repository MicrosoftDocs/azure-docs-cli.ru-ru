---
title: Установка Azure CLI в Linux с помощью yum
description: Как установить Azure CLI с помощью yum
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/26/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a98a51e4dc3ac85d27e27ef9b9164a7f98431d31
ms.sourcegitcommit: 465f2402b71e3de8c699798dc2a766fc90df241a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2020
ms.locfileid: "78953334"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="d1a6c-103">Установка Azure CLI с помощью yum</span><span class="sxs-lookup"><span data-stu-id="d1a6c-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="d1a6c-104">Для дистрибутивов Linux, использующих `yum`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="d1a6c-105">Этот пакет протестирован с RHEL 7.7 и 8, Fedora 24 и более поздних версий, а также CentOS 7 и 8.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="d1a6c-106">Установка</span><span class="sxs-lookup"><span data-stu-id="d1a6c-106">Install</span></span>

1. <span data-ttu-id="d1a6c-107">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="d1a6c-108">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="d1a6c-109">Выполните установку с помощью команды `yum install`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="d1a6c-110">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d1a6c-111">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="d1a6c-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d1a6c-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d1a6c-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d1a6c-113">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="d1a6c-113">Troubleshooting</span></span>

<span data-ttu-id="d1a6c-114">Ниже описаны некоторые распространенные проблемы при установке с помощью `yum`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="d1a6c-115">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d1a6c-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="d1a6c-116">Установка в RHEL 7.6 или других системах без Python 3</span><span class="sxs-lookup"><span data-stu-id="d1a6c-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="d1a6c-117">По возможности обновите систему до версии с официальной поддержкой пакета `python3`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-117">If you can, please upgrade your system to a version with official support for `python3` package.</span></span> <span data-ttu-id="d1a6c-118">В противном случае необходимо сначала установить пакет `python3`, а также выполнить [сборку из источника](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) или выполнить установку из определенного [дополнительного репозитория](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="d1a6c-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="d1a6c-119">Затем можно скачать пакет и установить его без зависимости.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="d1a6c-120">Если вы установили Python 3, но у вас по-прежнему возникает ошибка `python3: command not found` при попытке запустить CLI, необходимо добавить путь в переменную среды.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-120">If you have setup python3 but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>
```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="d1a6c-121">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="d1a6c-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="d1a6c-122">Вы также можете явным образом настроить `yum`, чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-122">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="d1a6c-123">Убедитесь, что следующие строки отображаются в разделе `[main]` в `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="d1a6c-123">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="d1a6c-124">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:</span><span class="sxs-lookup"><span data-stu-id="d1a6c-124">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="d1a6c-125">Update</span><span class="sxs-lookup"><span data-stu-id="d1a6c-125">Update</span></span>

<span data-ttu-id="d1a6c-126">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-126">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d1a6c-127">Удаление</span><span class="sxs-lookup"><span data-stu-id="d1a6c-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d1a6c-128">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-128">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="d1a6c-129">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-129">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="d1a6c-130">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-130">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="d1a6c-131">Next Steps</span><span class="sxs-lookup"><span data-stu-id="d1a6c-131">Next Steps</span></span>

<span data-ttu-id="d1a6c-132">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="d1a6c-132">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d1a6c-133">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d1a6c-133">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
