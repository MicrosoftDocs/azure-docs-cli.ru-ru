---
title: Установка Azure CLI в Linux с помощью zypper
description: Как установить Azure CLI с помощью zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: bb60b807df29833a74b1dab4def6f5ced58c8ffe
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450281"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="32e13-103">Установка Azure CLI с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="32e13-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="32e13-104">Для дистрибутивов Linux, использующих `zypper`, например openSUSE или SLES, доступен пакет Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="32e13-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="32e13-105">Этот пакет протестирован с openSUSE 42.2 и пакетом обновления 2 для SLES 12.</span><span class="sxs-lookup"><span data-stu-id="32e13-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="32e13-106">Install</span><span class="sxs-lookup"><span data-stu-id="32e13-106">Install</span></span>

1. <span data-ttu-id="32e13-107">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="32e13-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="32e13-108">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="32e13-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="32e13-109">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="32e13-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="32e13-110">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="32e13-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="32e13-111">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="32e13-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="32e13-112">Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="32e13-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="32e13-113">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="32e13-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="32e13-114">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="32e13-114">Troubleshooting</span></span>

<span data-ttu-id="32e13-115">Ниже описаны некоторые распространенные проблемы при установке с помощью `zypper`.</span><span class="sxs-lookup"><span data-stu-id="32e13-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="32e13-116">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="32e13-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]


## <a name="update"></a><span data-ttu-id="32e13-117">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="32e13-117">Update</span></span>

<span data-ttu-id="32e13-118">Можно обновить пакет, воспользовавшись командой `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="32e13-118">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="32e13-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="32e13-119">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="32e13-120">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="32e13-120">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="32e13-121">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="32e13-121">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="32e13-122">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="32e13-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
   ## <a name="next-steps"></a><span data-ttu-id="32e13-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="32e13-123">Next Steps</span></span>

<span data-ttu-id="32e13-124">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="32e13-124">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="32e13-125">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="32e13-125">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
