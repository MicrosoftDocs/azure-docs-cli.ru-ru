---
title: Запуск Azure CLI в контейнере Docker
description: Как запустить контейнер Docker, в котором размещен Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 2a4515f5301daca68f6e1a161fb2327f6caa0cf5
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593835"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="1653e-103">Запуск Azure CLI в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="1653e-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="1653e-104">Docker можно использовать для запуска изолированного контейнера Linux с предварительно установленным Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1653e-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="1653e-105">Docker позволяет быстро начать работу, используя изолированную среду для запуска CLI.</span><span class="sxs-lookup"><span data-stu-id="1653e-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="1653e-106">Этот образ также можно использовать в качестве основы для ваших собственных развертываний.</span><span class="sxs-lookup"><span data-stu-id="1653e-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="1653e-107">Запуск в контейнере Docker</span><span class="sxs-lookup"><span data-stu-id="1653e-107">Run in a Docker container</span></span>

<span data-ttu-id="1653e-108">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="1653e-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="1653e-109">Если вы хотите извлечь ключи SSH из пользовательской среды, можно использовать `-v ${HOME}/.ssh:/root/.ssh`, чтобы подключить ключи SSH в этой среде.</span><span class="sxs-lookup"><span data-stu-id="1653e-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="1653e-110">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="1653e-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="1653e-111">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="1653e-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="1653e-112">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1653e-112">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="1653e-113">Обновление образа Docker</span><span class="sxs-lookup"><span data-stu-id="1653e-113">Update Docker image</span></span>

<span data-ttu-id="1653e-114">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="1653e-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="1653e-115">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="1653e-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="1653e-116">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="1653e-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="1653e-117">Удаление образа Docker</span><span class="sxs-lookup"><span data-stu-id="1653e-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="1653e-118">После остановки любого контейнера под управлением образа CLI удалите образ.</span><span class="sxs-lookup"><span data-stu-id="1653e-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="1653e-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1653e-119">Next Steps</span></span>

<span data-ttu-id="1653e-120">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="1653e-120">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="1653e-121">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1653e-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
