---
title: "Установка Azure CLI 2.0 в Linux с помощью apt"
description: "Как установить Azure CLI 2.0 с помощью apt"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 840e5e7d6531fe92d30235f621e381589266d1d3
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/19/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="b0fe3-103">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="b0fe3-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="b0fe3-104">Если вы используете дистрибутив, который поставляется с `apt`, например Ubuntu или Debian, можно применить 64-разрядный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="b0fe3-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="b0fe3-105">This package has been tested with:</span></span>

* <span data-ttu-id="b0fe3-106">Ubuntu wheezy, xenial и artful</span><span class="sxs-lookup"><span data-stu-id="b0fe3-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="b0fe3-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="b0fe3-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="b0fe3-108">Install</span><span class="sxs-lookup"><span data-stu-id="b0fe3-108">Install</span></span>

1. <span data-ttu-id="b0fe3-109">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="b0fe3-110">Выполните следующие команды sudo:</span><span class="sxs-lookup"><span data-stu-id="b0fe3-110">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="b0fe3-111">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-111">You can run the Azure CLI with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b0fe3-112">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b0fe3-112">Troubleshooting</span></span>

<span data-ttu-id="b0fe3-113">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-113">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="b0fe3-114">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="b0fe3-114">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="b0fe3-115">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="b0fe3-115">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="b0fe3-116">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="b0fe3-116">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="b0fe3-117">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-117">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="b0fe3-118">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-118">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

## <a name="update"></a><span data-ttu-id="b0fe3-119">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="b0fe3-119">Update</span></span>

<span data-ttu-id="b0fe3-120">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-120">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="b0fe3-121">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-121">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="b0fe3-122">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-122">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="b0fe3-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="b0fe3-123">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b0fe3-124">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-124">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="b0fe3-125">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-125">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="b0fe3-126">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="b0fe3-126">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
