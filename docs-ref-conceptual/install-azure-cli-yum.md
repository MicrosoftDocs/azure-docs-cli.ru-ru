---
title: Установка Azure CLI в Linux с помощью yum
description: Как установить Azure CLI с помощью yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a33b5850abc40e91a1ffbeacd49d56169f67d282
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543604"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="73d3f-103">Установка Azure CLI с помощью yum</span><span class="sxs-lookup"><span data-stu-id="73d3f-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="73d3f-104">Для дистрибутивов Linux, использующих `yum`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="73d3f-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="73d3f-105">Этот пакет протестирован с RHEL 7.7 и 8, Fedora 24 и более поздних версий, а также CentOS 7 и 8.</span><span class="sxs-lookup"><span data-stu-id="73d3f-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="73d3f-106">Установка</span><span class="sxs-lookup"><span data-stu-id="73d3f-106">Install</span></span>

1. <span data-ttu-id="73d3f-107">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="73d3f-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="73d3f-108">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="73d3f-109">Выполните установку с помощью команды `yum install`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="73d3f-110">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="73d3f-111">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="73d3f-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="73d3f-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="73d3f-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="73d3f-113">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="73d3f-113">Troubleshooting</span></span>

<span data-ttu-id="73d3f-114">Ниже описаны некоторые распространенные проблемы при установке с помощью `yum`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="73d3f-115">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="73d3f-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="73d3f-116">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="73d3f-116">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="73d3f-117">Вы также можете явным образом настроить `yum`, чтобы использовать этот прокси-сервер все время.</span><span class="sxs-lookup"><span data-stu-id="73d3f-117">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="73d3f-118">Убедитесь, что следующие строки отображаются в разделе `[main]` в `/etc/yum.conf`:</span><span class="sxs-lookup"><span data-stu-id="73d3f-118">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="73d3f-119">Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:</span><span class="sxs-lookup"><span data-stu-id="73d3f-119">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="73d3f-120">Установка в RHEL 7.6 или других системах без Python 3</span><span class="sxs-lookup"><span data-stu-id="73d3f-120">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="73d3f-121">По возможности обновите систему до версии с официальной поддержкой пакета `python3`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-121">If you can, please upgrade your system to a verison with official support for `python3` package.</span></span> <span data-ttu-id="73d3f-122">В противном случае необходимо сначала установить пакет `python3`, а также выполнить [сборку из источника](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) или выполнить установку из определенного [дополнительного репозитория](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span><span class="sxs-lookup"><span data-stu-id="73d3f-122">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="73d3f-123">Затем можно выполнить [инструкции по установке вручную](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="73d3f-123">Then you can follow the [manual install instructions](install-azure-cli-linux.md).</span></span>

<span data-ttu-id="73d3f-124">Самый предпочтительный вариант — по-прежнему использовать Python 2 и следовать [инструкциям по установке вручную](install-azure-cli-linux.md), так как поддержка Python 2 будет прекращена 1 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="73d3f-124">The least recommended option is to still use Python 2 and follow the [manual install instructions](install-azure-cli-linux.md) since Python 2 is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="73d3f-125">В следующей версии Azure CLI поддержка Python 2.7 будет прекращена.</span><span class="sxs-lookup"><span data-stu-id="73d3f-125">A future version of Azure CLI will drop support for Python 2.7.</span></span>

## <a name="update"></a><span data-ttu-id="73d3f-126">Обновление</span><span class="sxs-lookup"><span data-stu-id="73d3f-126">Update</span></span>

<span data-ttu-id="73d3f-127">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="73d3f-127">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="73d3f-128">Удаление</span><span class="sxs-lookup"><span data-stu-id="73d3f-128">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="73d3f-129">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="73d3f-129">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="73d3f-130">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="73d3f-130">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="73d3f-131">Если вы не используете другие пакеты Майкрософт, удалите ключ подписывания.</span><span class="sxs-lookup"><span data-stu-id="73d3f-131">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="73d3f-132">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="73d3f-132">Next Steps</span></span>

<span data-ttu-id="73d3f-133">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="73d3f-133">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="73d3f-134">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="73d3f-134">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
