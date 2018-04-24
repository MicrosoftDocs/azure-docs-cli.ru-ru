---
title: Установка Azure CLI 2.0 в Linux с использованием yum
description: Как установить Azure CLI 2.0 с помощью yum
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 6a63d1ccd6b182b0c7144101f7efbf3264a6cb72
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="23f7f-103">Установка Azure CLI 2.0 с помощью yum</span><span class="sxs-lookup"><span data-stu-id="23f7f-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="23f7f-104">Если используется дистрибутив в составе `yum`, например RHEL, Fedora или CentOS, вы можете работать с доступным пакетом для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="23f7f-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="23f7f-105">Этот пакет протестирован с RHEL 7, Fedora 19 и более поздних версий, а также CentOS 7.</span><span class="sxs-lookup"><span data-stu-id="23f7f-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="23f7f-106">Install</span><span class="sxs-lookup"><span data-stu-id="23f7f-106">Install</span></span>

1. <span data-ttu-id="23f7f-107">Импортируйте ключ репозитория Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="23f7f-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="23f7f-108">Создайте сведения о локальном репозитории `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="23f7f-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="23f7f-109">Выполните установку с помощью команды `yum install`.</span><span class="sxs-lookup"><span data-stu-id="23f7f-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="23f7f-110">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="23f7f-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="23f7f-111">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="23f7f-111">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="23f7f-112">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="23f7f-112">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="23f7f-113">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="23f7f-113">Update</span></span>

<span data-ttu-id="23f7f-114">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="23f7f-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="23f7f-115">Удаление</span><span class="sxs-lookup"><span data-stu-id="23f7f-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="23f7f-116">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="23f7f-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="23f7f-117">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="23f7f-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="23f7f-118">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="23f7f-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
