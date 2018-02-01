---
title: "Установка Azure CLI с помощью Docker"
description: "Как установить контейнер Docker с помощью Azure CLI 2.0"
keywords: Azure CLI,Install Azure CLI,azure docker,azure docker image,
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 7a12da712cd2aad5bb5fb56e27267a8e05df34a6
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2018
---
# <a name="install-azure-cli-20-with-docker"></a>Установка Azure CLI 2.0 с помощью Docker

Docker можно использовать для установки изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0. Так вы сможете быстро начать работу со средой и CLI, чтобы решить, подходит ли это средство для вас, либо с базовым образом.

## <a name="install-with-docker"></a>Установка с помощью Docker

Установите CLI с помощью команды `docker run`.

   ```bash
   docker run -it microsoft/azure-cli:<version>
   ```

См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/microsoft/azure-cli/tags/).

CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.

> [!NOTE]
> Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli:<version>
> ```

### <a name="update-with-docker"></a>Обновление с помощью Docker

Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры. По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.

1. Обновите локальный образ с помощью команды `docker pull`.

   ```bash
   docker pull microsoft/azure-cli
   ```

2. Получите данные о контейнерах, которые используют образ CLI.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.

3. Остановите и заново создайте контейнеры.

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run microsoft/azure-cli
   ```

### <a name="uninstall-with-docker"></a>Удаление с помощью Docker

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

Чтобы удалить образ Docker CLI, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.

1. Получите данные о контейнерах, на которых запущен образ azure-cli.

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.

2. Удалите все контейнеры с образом CLI.

   ```bash
   docker rm 34a868beb2ab
   ```

3. Удалите локально установленный образ CLI.

   ```bash
   docker rmi microsoft/azure-cli
   ```

