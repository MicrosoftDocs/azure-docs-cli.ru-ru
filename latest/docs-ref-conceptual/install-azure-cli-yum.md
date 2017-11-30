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
ms.openlocfilehash: de695454c6f3109679b9eb9f6c0d77348d354518
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="04f52-104">Установка Azure CLI 2.0 с помощью yum</span><span class="sxs-lookup"><span data-stu-id="04f52-104">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="04f52-105">Если вы используете дистрибутив, который поставляется с диспетчером пакетов `yum`, например RHEL, Fedora или CentOS, в системе можно установить доступный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="04f52-105">If you are running a distirbution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is an available package for the Azure CLI that you can install on your system.</span></span>

> [!NOTE]
> <span data-ttu-id="04f52-106">Для работы с CLI необходимо установить Python 2.7.x или Python 3.x.</span><span class="sxs-lookup"><span data-stu-id="04f52-106">You must have Python 2.7.x or Python 3.x in order to use the CLI.</span></span> <span data-ttu-id="04f52-107">Если в дистрибутиве нет соответствующих пакетов, [установите Python](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="04f52-107">If your distribution does not have a package for either, [install Python](https://www.python.org/downloads/).</span></span>

## <a name="install"></a><span data-ttu-id="04f52-108">Установить</span><span class="sxs-lookup"><span data-stu-id="04f52-108">Install</span></span> 

1. <span data-ttu-id="04f52-109">Импортируйте ключ репозитория Майкрософт:</span><span class="sxs-lookup"><span data-stu-id="04f52-109">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="04f52-110">Создайте сведения о локальном репозитории `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="04f52-110">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="04f52-111">Обновите индекс пакета `yum` и выполните установку:</span><span class="sxs-lookup"><span data-stu-id="04f52-111">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

<span data-ttu-id="04f52-112">Обновите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="04f52-112">Run the Azure CLI with the `az` command.</span></span>

## <a name="update"></a><span data-ttu-id="04f52-113">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="04f52-113">Update</span></span>

<span data-ttu-id="04f52-114">Обновите Azure CLI, воспользовавшись командой `yum update`.</span><span class="sxs-lookup"><span data-stu-id="04f52-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="04f52-115">Удаление</span><span class="sxs-lookup"><span data-stu-id="04f52-115">Uninstall</span></span>

<span data-ttu-id="04f52-116">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="04f52-116">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="04f52-117">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="04f52-117">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="04f52-118">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="04f52-118">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="04f52-119">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="04f52-119">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

1. <span data-ttu-id="04f52-120">Удалите пакет из системы.</span><span class="sxs-lookup"><span data-stu-id="04f52-120">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="04f52-121">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.</span><span class="sxs-lookup"><span data-stu-id="04f52-121">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="04f52-122">Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.</span><span class="sxs-lookup"><span data-stu-id="04f52-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
