---
title: Установка Azure CLI 2.0 в Linux с использованием yum
description: Как установить Azure CLI 2.0 с помощью yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b3c82825af3d1d2420b0111d1a370a17f37d9426
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-with-yum"></a>Установка Azure CLI 2.0 с помощью yum

Если используется дистрибутив в составе `yum`, например RHEL, Fedora или CentOS, вы можете работать с доступным пакетом для Azure CLI. Этот пакет протестирован с RHEL 7, Fedora 19 и более поздних версий, а также CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Install

1. Импортируйте ключ репозитория Майкрософт.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Создайте сведения о локальном репозитории `azure-cli`.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Выполните установку с помощью команды `yum install`. 

   ```bash
   sudo yum install azure-cli
   ```

Запустите Azure CLI с помощью команды `az`. Для входа выполните команду `az login`.

```azurecli
az login
```

Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="update"></a>Блокировка изменений

Обновите Azure CLI, воспользовавшись командой `yum update`.

```bash
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
