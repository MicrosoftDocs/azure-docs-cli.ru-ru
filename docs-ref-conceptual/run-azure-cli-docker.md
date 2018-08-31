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
ms.openlocfilehash: 7a50682d549f6383e68128f2c2aef02dc2877a8e
ms.sourcegitcommit: 83826ca154c9f32c6091c63ce4b3e480694ba8d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/09/2018
ms.locfileid: "43144906"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="62ed8-103">Запуск Azure CLI 2.0 в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="62ed8-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="62ed8-104">Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0.</span><span class="sxs-lookup"><span data-stu-id="62ed8-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="62ed8-105">Docker позволяет быстро начать работу с окружением, в котором вы можете поработать с CLI, чтобы решить, подходит ли это средство для вас, либо использовать наш образ как основу для собственного развертывания.</span><span class="sxs-lookup"><span data-stu-id="62ed8-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="62ed8-106">Запуск в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="62ed8-106">Run in a Docker container</span></span>

<span data-ttu-id="62ed8-107">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="62ed8-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="62ed8-108">Если вы хотите извлечь ключи SSH из пользовательской среды, можно использовать `-v ${HOME}/.ssh:/root/.ssh`, чтобы подключить ключи SSH в этой среде.</span><span class="sxs-lookup"><span data-stu-id="62ed8-108">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="62ed8-109">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="62ed8-109">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="62ed8-110">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="62ed8-110">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="62ed8-111">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="62ed8-111">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="62ed8-112">Обновление образа Docker</span><span class="sxs-lookup"><span data-stu-id="62ed8-112">Update Docker image</span></span>

<span data-ttu-id="62ed8-113">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="62ed8-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="62ed8-114">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="62ed8-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="62ed8-115">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="62ed8-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="62ed8-116">Удаление образа Docker</span><span class="sxs-lookup"><span data-stu-id="62ed8-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="62ed8-117">После остановки любого контейнера под управлением образа CLI удалите образ.</span><span class="sxs-lookup"><span data-stu-id="62ed8-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
