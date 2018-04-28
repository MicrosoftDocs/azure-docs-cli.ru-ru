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
ms.openlocfilehash: d88dbcec947372aa154bce939edd99f65cd9480f
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="636f2-103">Запуск Azure CLI 2.0 в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="636f2-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="636f2-104">Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0.</span><span class="sxs-lookup"><span data-stu-id="636f2-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="636f2-105">Docker позволяет быстро начать работу с окружением, в котором вы можете поработать с CLI, чтобы решить, подходит ли это средство для вас, либо использовать наш образ как основу для собственного развертывания.</span><span class="sxs-lookup"><span data-stu-id="636f2-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="636f2-106">Запуск в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="636f2-106">Run in a Docker container</span></span>

<span data-ttu-id="636f2-107">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="636f2-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="636f2-108">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="636f2-108">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="636f2-109">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="636f2-109">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="636f2-110">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="636f2-110">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="636f2-111">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="636f2-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="636f2-112">Обновление образа Docker</span><span class="sxs-lookup"><span data-stu-id="636f2-112">Update Docker image</span></span>

<span data-ttu-id="636f2-113">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="636f2-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="636f2-114">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="636f2-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="636f2-115">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="636f2-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="636f2-116">Удаление образа Docker</span><span class="sxs-lookup"><span data-stu-id="636f2-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="636f2-117">После остановки любого контейнера под управлением образа CLI удалите образ.</span><span class="sxs-lookup"><span data-stu-id="636f2-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
