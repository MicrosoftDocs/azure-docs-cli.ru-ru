---
title: "Установка Azure CLI 2.0 в Linux с использованием yum"
description: "Как установить Azure CLI 2.0 с помощью yum"
keywords: Azure CLI,Install Azure CLI,azure yum,azure rhel, azure fedora, azure centos
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 9d11c3cf5d9e7ba58c3e2edd830e0d12669f5b91
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-yum"></a>Установка Azure CLI 2.0 с помощью yum

Если используется дистрибутив в составе `yum`, например RHEL, Fedora или CentOS, вы можете работать с доступным пакетом для Azure CLI. Этот пакет протестирован с RHEL 7, Fedora 19 и более поздних версий, а также CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Install

1. Импортируйте ключ репозитория Майкрософт:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Создайте сведения о локальном репозитории `azure-cli`:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Обновите индекс пакета `yum` и выполните установку:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

Обновите Azure CLI с помощью команды `az`.

## <a name="update"></a>Блокировка изменений

Обновите Azure CLI, воспользовавшись командой `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Удалите пакет из системы.

   ```bash
   sudo yum remove azure-cli
   ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
