---
title: "Установка Azure CLI 2.0 в Linux с помощью zypper"
description: "Как установить Azure CLI 2.0 с помощью zypper"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6ee3aff74f43fab0c80c58c7fe57c9fa74a6ef2f
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="0a062-103">Установка Azure CLI 2.0 с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="0a062-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="0a062-104">Если используется дистрибутив в составе `zypper`, например openSUSE или SLES, вы можете работать с доступным пакетом для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="0a062-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="0a062-105">Этот пакет протестирован с openSUSE 42.2 и пакетом обновления 2 для SLES 12.</span><span class="sxs-lookup"><span data-stu-id="0a062-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="0a062-106">Install</span><span class="sxs-lookup"><span data-stu-id="0a062-106">Install</span></span>

1. <span data-ttu-id="0a062-107">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="0a062-107">Install `curl`:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="0a062-108">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="0a062-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="0a062-109">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="0a062-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. <span data-ttu-id="0a062-110">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="0a062-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

<span data-ttu-id="0a062-111">Запустить CLI можно с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="0a062-111">You can run the CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="0a062-112">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="0a062-112">Update</span></span>

<span data-ttu-id="0a062-113">Можно обновить пакет, воспользовавшись командой `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="0a062-113">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="0a062-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="0a062-114">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="0a062-115">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="0a062-115">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="0a062-116">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="0a062-116">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. <span data-ttu-id="0a062-117">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="0a062-117">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

