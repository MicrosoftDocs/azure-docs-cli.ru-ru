---
title: "Установка Azure CLI 2.0 в Linux с помощью zypper"
description: "Как установить Azure CLI 2.0 с помощью zypper"
keywords: azure cli, azure cli install, azure cli zypper, azure cli opensuse, azure cli sle
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: c0b566f96e47d34d20f7bf85db0fae32913ed596
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>Установка Azure CLI 2.0 с помощью zypper

Если используется дистрибутив в составе `zypper`, например openSUSE или SLES, вы можете работать с доступным пакетом для Azure CLI. Этот пакет протестирован с openSUSE 42.2 и пакетом обновления 2 для SLES 12.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Install

1. Установите `curl`:

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Импортируйте ключ репозитория Майкрософт:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Создайте сведения о локальном репозитории `azure-cli`:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. Обновите индекс пакета `zypper` и выполните установку:

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

Запустить CLI можно с помощью команды `az`.

## <a name="update"></a>Блокировка изменений

Можно обновить пакет, воспользовавшись командой `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Удалите пакет из системы.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Если вы удалили сведения о репозитории, также удалите ключ подписи Microsoft GPG.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

