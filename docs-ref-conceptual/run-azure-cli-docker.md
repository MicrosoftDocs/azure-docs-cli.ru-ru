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
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="51aa5-103">Запуск Azure CLI 2.0 в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="51aa5-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="51aa5-104">Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0.</span><span class="sxs-lookup"><span data-stu-id="51aa5-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="51aa5-105">Docker позволяет быстро начать работу, используя изолированную среду для запуска CLI.</span><span class="sxs-lookup"><span data-stu-id="51aa5-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="51aa5-106">Этот образ также можно использовать в качестве основы для ваших собственных развертываний.</span><span class="sxs-lookup"><span data-stu-id="51aa5-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="51aa5-107">Запуск в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="51aa5-107">Run in a Docker container</span></span>

<span data-ttu-id="51aa5-108">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="51aa5-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="51aa5-109">Если вы хотите извлечь ключи SSH из пользовательской среды, можно использовать `-v ${HOME}/.ssh:/root/.ssh`, чтобы подключить ключи SSH в этой среде.</span><span class="sxs-lookup"><span data-stu-id="51aa5-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="51aa5-110">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="51aa5-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="51aa5-111">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="51aa5-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="51aa5-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="51aa5-112">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="51aa5-113">Обновление образа Docker</span><span class="sxs-lookup"><span data-stu-id="51aa5-113">Update Docker image</span></span>

<span data-ttu-id="51aa5-114">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="51aa5-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="51aa5-115">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="51aa5-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="51aa5-116">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="51aa5-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="51aa5-117">Удаление образа Docker</span><span class="sxs-lookup"><span data-stu-id="51aa5-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="51aa5-118">После остановки любого контейнера под управлением образа CLI удалите образ.</span><span class="sxs-lookup"><span data-stu-id="51aa5-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```
