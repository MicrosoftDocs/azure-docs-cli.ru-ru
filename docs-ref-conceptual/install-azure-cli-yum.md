---
title: "Установка Azure CLI 2.0 с помощью yum"
description: "Как установить Azure CLI 2.0 с помощью yum"
keywords: Azure CLI,Install Azure CLI,azure yum,azure rhel, azure fedora, azure centos
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
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="7678b-104">Установка Azure CLI 2.0 с помощью yum</span><span class="sxs-lookup"><span data-stu-id="7678b-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="7678b-105">Если вы используете дистрибутив, который поставляется с диспетчером пакетов `yum`, например RHEL, Fedora или CentOS, в системе можно установить доступный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="7678b-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="7678b-106">Install</span><span class="sxs-lookup"><span data-stu-id="7678b-106">Install</span></span>

1. <span data-ttu-id="7678b-107">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="7678b-107">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="7678b-108">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="7678b-108">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="7678b-109">Обновите индекс пакета `yum` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="7678b-109">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="7678b-110">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="7678b-110">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="7678b-111">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="7678b-111">Update</span></span>

<span data-ttu-id="7678b-112">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="7678b-112">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="7678b-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="7678b-113">Uninstall</span></span>

<span data-ttu-id="7678b-114">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="7678b-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="7678b-115">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="7678b-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="7678b-116">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="7678b-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="7678b-117">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="7678b-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="7678b-118">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="7678b-118">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="7678b-119">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="7678b-119">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="7678b-120">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="7678b-120">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
