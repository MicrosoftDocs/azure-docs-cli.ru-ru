---
title: Установка Azure CLI 2.0 в Linux с помощью zypper
description: Как установить Azure CLI 2.0 с помощью zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: a862cca17adb1bfa0201af250819158081c29813
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512977"
---
# <a name="install-azure-cli-20-with-zypper"></a><span data-ttu-id="ee4ca-103">Установка Azure CLI 2.0 с помощью zypper</span><span class="sxs-lookup"><span data-stu-id="ee4ca-103">Install Azure CLI 2.0 with zypper</span></span>

<span data-ttu-id="ee4ca-104">Если используется дистрибутив в составе `zypper`, например openSUSE или SLES, вы можете работать с доступным пакетом для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-104">If you are running a distribution that comes with `zypper`, such as openSUSE or SLES, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="ee4ca-105">Этот пакет протестирован с openSUSE 42.2 и пакетом обновления 2 для SLES 12.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="ee4ca-106">Install</span><span class="sxs-lookup"><span data-stu-id="ee4ca-106">Install</span></span>

1. <span data-ttu-id="ee4ca-107">Установите `curl`:</span><span class="sxs-lookup"><span data-stu-id="ee4ca-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="ee4ca-108">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="ee4ca-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="ee4ca-109">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="ee4ca-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="ee4ca-110">Обновите индекс пакета `zypper` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="ee4ca-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="ee4ca-111">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ee4ca-112">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-112">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="ee4ca-113">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ee4ca-113">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="ee4ca-114">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="ee4ca-114">Update</span></span>

<span data-ttu-id="ee4ca-115">Можно обновить пакет, воспользовавшись командой `zypper update`.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-115">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="ee4ca-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="ee4ca-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="ee4ca-117">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-117">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="ee4ca-118">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-118">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

  ```bash
  sudo zypper removerepo azure-cli
  ```

3. <span data-ttu-id="ee4ca-119">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="ee4ca-119">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

