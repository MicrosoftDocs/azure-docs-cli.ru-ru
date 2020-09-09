---
title: Запуск Azure CLI в контейнере Docker
description: Как запустить контейнер Docker, в котором размещен Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 369a886c260177d86762dc736a596a262ad2739f
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563082"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="6708f-103">Запуск Azure CLI в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="6708f-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="6708f-104">Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="6708f-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="6708f-105">Docker позволяет быстро начать работу, используя изолированную среду для запуска CLI.</span><span class="sxs-lookup"><span data-stu-id="6708f-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="6708f-106">Этот образ также можно использовать в качестве основы для ваших собственных развертываний.</span><span class="sxs-lookup"><span data-stu-id="6708f-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="6708f-107">Запуск в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="6708f-107">Run in a Docker container</span></span>

> [!NOTE]
> <span data-ttu-id="6708f-108">Интерфейс командной строки Azure перенесен в [Реестр контейнеров](https://azure.microsoft.com/services/container-registry).</span><span class="sxs-lookup"><span data-stu-id="6708f-108">The Azure CLI has migrated to [Microsoft Container Registry](https://azure.microsoft.com/services/container-registry).</span></span> <span data-ttu-id="6708f-109">Существующие теги в Docker Hub по-прежнему поддерживаются, но новые выпуски будут доступны только в виде mcr.microsoft.com/azure-cli.</span><span class="sxs-lookup"><span data-stu-id="6708f-109">Existing tags on Docker Hub are still supported, but new releases will only be available as mcr.microsoft.com/azure-cli.</span></span>

<span data-ttu-id="6708f-110">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="6708f-110">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it mcr.microsoft.com/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="6708f-111">Если вы хотите извлечь ключи SSH из пользовательской среды, можно использовать `-v ${HOME}/.ssh:/root/.ssh`, чтобы подключить ключи SSH в этой среде.</span><span class="sxs-lookup"><span data-stu-id="6708f-111">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh mcr.microsoft.com/azure-cli
> ```

<span data-ttu-id="6708f-112">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="6708f-112">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="6708f-113">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="6708f-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6708f-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6708f-114">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="6708f-115">Обновление образа Docker</span><span class="sxs-lookup"><span data-stu-id="6708f-115">Update Docker image</span></span>

<span data-ttu-id="6708f-116">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="6708f-116">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="6708f-117">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="6708f-117">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="6708f-118">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="6708f-118">Update your local image with `docker pull`.</span></span>

```bash
docker pull mcr.microsoft.com/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="6708f-119">Удаление образа Docker</span><span class="sxs-lookup"><span data-stu-id="6708f-119">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6708f-120">После остановки любого контейнера под управлением образа CLI удалите образ.</span><span class="sxs-lookup"><span data-stu-id="6708f-120">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi mcr.microsoft.com/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="6708f-121">Next Steps</span><span class="sxs-lookup"><span data-stu-id="6708f-121">Next Steps</span></span>

<span data-ttu-id="6708f-122">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="6708f-122">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6708f-123">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6708f-123">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
