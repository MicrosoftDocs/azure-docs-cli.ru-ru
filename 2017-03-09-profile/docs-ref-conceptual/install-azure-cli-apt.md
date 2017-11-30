---
title: "Установка Azure CLI 2.0 с помощью apt"
description: "Как установить Azure CLI 2.0 с помощью apt"
keywords: Azure CLI,Install Azure CLI,azure apt, azure debian, azure ubuntu
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
ms.openlocfilehash: 93d947d91973def1c05e2f5b2e7511bc1c5704a2
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-apt"></a>Установка Azure CLI 2.0 с помощью apt

Если вы используете дистрибутив, который поставляется с диспетчером пакетов `apt`, например Ubuntu или Debian, в системе можно установить доступный пакет для Azure CLI.

> [!NOTE]
> Для работы с CLI необходимо установить Python 2.7.x или Python 3.x. Если в дистрибутиве нет соответствующих пакетов, [установите Python](https://www.python.org/downloads/).

## <a name="install"></a>Установить

1. Измените список источников.
 
   - 32-разрядная система:

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - 64-разрядная система:

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. Выполните следующие команды sudo:

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

Запустите Azure CLI с помощью команды `az`.

## <a name="update"></a>Блокировка изменений

Используйте `apt-get upgrade`, чтобы обновить пакет CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> В результате обновятся все установленные в системе пакеты, зависимости которых не были изменены.
> Чтобы обновить только CLI, используйте команду `apt-get install`.
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="uninstall"></a>Удаление

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

1. Удалите CLI с помощью команды `apt-get remove`.

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Удалите все ненужные пакеты.

   ```bash
   sudo apt autoremove
   ```
