---
title: Запуск Azure CLI 2.0 в контейнере Docker
description: Как запустить контейнер Docker, в котором размещен Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 277d9d3423af4941fb7f7fb57130fa1b7af7d32e
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388343"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Запуск Azure CLI 2.0 в контейнере Docker

Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0. Docker позволяет быстро начать работу, используя изолированную среду для запуска CLI. Этот образ также можно использовать в качестве основы для ваших собственных развертываний.

## <a name="run-in-a-docker-container"></a>Запуск в контейнере Docker

Установите CLI с помощью команды `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Если вы хотите извлечь ключи SSH из пользовательской среды, можно использовать `-v ${HOME}/.ssh:/root/.ssh`, чтобы подключить ключи SSH в этой среде.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`. Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).

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
