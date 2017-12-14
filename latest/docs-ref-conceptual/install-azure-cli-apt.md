---
title: "Установка Azure CLI 2.0 с помощью apt"
description: "Как установить Azure CLI 2.0 с помощью apt"
keywords: Azure CLI,Install Azure CLI,azure apt, azure debian, azure ubuntu
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 75c531a13a4b730158cd2e874cb6c5d581a27598
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="ac2fd-104">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="ac2fd-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="ac2fd-105">Если вы используете дистрибутив, который поставляется с диспетчером пакетов `apt`, например Ubuntu или Debian, в системе можно установить доступный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="ac2fd-106">Установить</span><span class="sxs-lookup"><span data-stu-id="ac2fd-106">Install</span></span>

1. <span data-ttu-id="ac2fd-107">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-107">Modify your sources list:</span></span>

   - <span data-ttu-id="ac2fd-108">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="ac2fd-108">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="ac2fd-109">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="ac2fd-109">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="ac2fd-110">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="ac2fd-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="ac2fd-111">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="ac2fd-112">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="ac2fd-112">Update</span></span>

<span data-ttu-id="ac2fd-113">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-113">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="ac2fd-114">В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-114">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="ac2fd-115">Чтобы обновить только CLI, используйте команду `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-115">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="ac2fd-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="ac2fd-116">Uninstall</span></span>

<span data-ttu-id="ac2fd-117">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-117">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="ac2fd-118">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-118">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="ac2fd-119">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-119">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="ac2fd-120">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ac2fd-120">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="ac2fd-121">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-121">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="ac2fd-122">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-122">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="ac2fd-123">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="ac2fd-123">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
