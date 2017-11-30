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
ms.openlocfilehash: 93d947d91973def1c05e2f5b2e7511bc1c5704a2
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="55c34-104">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="55c34-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="55c34-105">Если вы используете дистрибутив, который поставляется с диспетчером пакетов `apt`, например Ubuntu или Debian, в системе можно установить доступный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="55c34-105">If you are running a distirbution that comes with `apt`, such as Ubuntu or Debian, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="55c34-106">Для работы с CLI необходимо установить Python 2.7.x или Python 3.x.</span><span class="sxs-lookup"><span data-stu-id="55c34-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="55c34-107">Если в дистрибутиве нет соответствующих пакетов, [установите Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="55c34-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="55c34-108">Установить</span><span class="sxs-lookup"><span data-stu-id="55c34-108">Install</span></span>

1. <span data-ttu-id="55c34-109">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="55c34-109">Modify your sources list:</span></span>
 
   - <span data-ttu-id="55c34-110">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="55c34-110">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="55c34-111">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="55c34-111">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="55c34-112">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="55c34-112">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="55c34-113">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="55c34-113">You can run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="55c34-114">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="55c34-114">Update</span></span>

<span data-ttu-id="55c34-115">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="55c34-115">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="55c34-116">В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="55c34-116">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="55c34-117">Чтобы обновить только CLI, используйте команду `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="55c34-117">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a><span data-ttu-id="55c34-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="55c34-118">Uninstall</span></span>

<span data-ttu-id="55c34-119">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="55c34-119">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="55c34-120">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="55c34-120">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="55c34-121">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="55c34-121">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="55c34-122">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="55c34-122">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="55c34-123">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="55c34-123">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="55c34-124">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="55c34-124">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="55c34-125">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="55c34-125">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
