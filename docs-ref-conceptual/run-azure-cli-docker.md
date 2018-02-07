---
title: "Запуск Azure CLI 2.0 в контейнере Docker"
description: "Как запустить контейнер Docker, в котором размещен Azure CLI 2.0"
keywords: Azure CLI,Install Azure CLI,azure docker,azure docker image,
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/18
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 819ff0cdb0df6057a5dff8f8ab015796f06c6a9b
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Запуск Azure CLI 2.0 в контейнере Docker

Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0. Docker позволяет быстро начать работу с окружением, в котором вы можете поработать с CLI, чтобы решить, подходит ли это средство для вас, либо использовать наш образ как основу для собственного развертывания.

## <a name="run-in-a-docker-container"></a>Запуск в контейнере Docker

Установите CLI с помощью команды `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.

> [!NOTE]
> Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a>Обновление образа Docker

Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры. По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.

Обновите локальный образ с помощью команды `docker pull`.

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a>Удаление образа Docker

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

После остановки любого контейнера под управлением образа CLI удалите образ.

```bash
docker rmi microsoft/azure-cli
```
