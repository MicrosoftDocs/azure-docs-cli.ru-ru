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
ms.openlocfilehash: dde90e78f3ec53d323ca78c816ceefb8cf65608b
ms.sourcegitcommit: 15d6dfaee2075d0abceb2aa2423f0b6ef7b2ac9b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2018
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
   sudo zypper install --from azure-cli -y azure-cli
   ```

Запустите Azure CLI с помощью команды `az`. Для входа выполните команду `az login`.

```azurecli
az login
```

Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

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

