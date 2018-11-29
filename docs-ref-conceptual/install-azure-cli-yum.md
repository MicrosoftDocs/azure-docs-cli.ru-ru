---
title: Установка Azure CLI в Linux с помощью yum
description: Как установить Azure CLI с помощью yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7e2c7c5477c8d5a617875eeaed8e3d267d9bcf8c
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450315"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="ca2ea-103">Установка Azure CLI с помощью yum</span><span class="sxs-lookup"><span data-stu-id="ca2ea-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="ca2ea-104">Для дистрибутивов Linux, использующих `yum`, например RHEL, Fedora или CentOS, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="ca2ea-105">Этот пакет протестирован с RHEL 7, Fedora 19 и более поздних версий, а также CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="ca2ea-106">Install</span><span class="sxs-lookup"><span data-stu-id="ca2ea-106">Install</span></span>

1. <span data-ttu-id="ca2ea-107">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="ca2ea-108">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="ca2ea-109">Выполните установку с помощью команды `yum install`.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="ca2ea-110">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ca2ea-111">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="ca2ea-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ca2ea-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ca2ea-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ca2ea-113">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="ca2ea-113">Troubleshooting</span></span>

<span data-ttu-id="ca2ea-114">Ниже описаны некоторые распространенные проблемы при установке с помощью `yum`.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="ca2ea-115">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ca2ea-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="ca2ea-116">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="ca2ea-116">Update</span></span>

<span data-ttu-id="ca2ea-117">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-117">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ca2ea-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="ca2ea-118">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ca2ea-119">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-119">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="ca2ea-120">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-120">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="ca2ea-121">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-121">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="ca2ea-122">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ca2ea-122">Next Steps</span></span>

<span data-ttu-id="ca2ea-123">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="ca2ea-123">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ca2ea-124">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ca2ea-124">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
