---
title: "Установка Azure CLI 2.0 с помощью zypper"
description: "Как установить Azure CLI 2.0 с помощью zypper"
keywords: azure cli, azure cli install, azure cli zypper, azure cli opensuse, azure cli sle
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
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a>Установка Azure CLI 2.0 с помощью zypper

Если вы используете дистрибутив, который поставляется с диспетчером пакетов `zypper`, например OpenSUSE или SLE, в системе можно установить доступный пакет для Azure CLI.

> [!NOTE]
> Для работы с CLI необходимо установить Python 2.7.x или Python 3.x. Если в дистрибутиве нет соответствующих пакетов, [установите Python](https://www.python.org/downloads/).

## <a name="install"></a>Установить 

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

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

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

