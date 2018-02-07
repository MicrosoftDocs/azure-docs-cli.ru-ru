---
title: "Установка Azure CLI 2.0 в Linux с помощью apt"
description: "Как установить Azure CLI 2.0 с помощью apt"
keywords: Azure CLI,Install Azure CLI,azure apt, azure debian, azure ubuntu
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: fdd9f0061d5d38ed5a349b11eb0f5f27786bc1ab
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="18b6f-104">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="18b6f-104">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="18b6f-105">Если вы используете дистрибутив, который поставляется с `apt`, например Ubuntu или Debian, можно применить пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="18b6f-105">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="18b6f-106">Этот пакет протестирован с Ubuntu Wheezy и Ubuntu Xenial.</span><span class="sxs-lookup"><span data-stu-id="18b6f-106">This package has been tested with Ubuntu Wheezy and Ubuntu Xenial.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="18b6f-107">Install</span><span class="sxs-lookup"><span data-stu-id="18b6f-107">Install</span></span>

1. <span data-ttu-id="18b6f-108">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="18b6f-108">Modify your sources list:</span></span>

   - <span data-ttu-id="18b6f-109">32-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="18b6f-109">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="18b6f-110">64-разрядная система:</span><span class="sxs-lookup"><span data-stu-id="18b6f-110">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="18b6f-111">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="18b6f-111">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="18b6f-112">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-112">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="18b6f-113">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="18b6f-113">Troubleshooting</span></span>

<span data-ttu-id="18b6f-114">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-114">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="18b6f-115">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="18b6f-115">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="18b6f-116">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="18b6f-116">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="18b6f-117">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="18b6f-117">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="18b6f-118">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-118">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="18b6f-119">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-119">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="18b6f-120">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="18b6f-120">Update</span></span>

<span data-ttu-id="18b6f-121">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="18b6f-121">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="18b6f-122">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="18b6f-122">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="18b6f-123">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-123">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="18b6f-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="18b6f-124">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="18b6f-125">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="18b6f-125">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="18b6f-126">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="18b6f-126">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="18b6f-127">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="18b6f-127">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
