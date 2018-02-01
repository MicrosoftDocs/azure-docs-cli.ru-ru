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
# <a name="install-azure-cli-20-with-docker"></a><span data-ttu-id="52941-104">Установка Azure CLI 2.0 с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="52941-104">Install Azure CLI 2.0 with Docker</span></span>

<span data-ttu-id="52941-105">Docker можно использовать для установки изолированного контейнера Linux с предварительно установленным Azure CLI версии 2.0.</span><span class="sxs-lookup"><span data-stu-id="52941-105">You can use Docker to install a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="52941-106">Так вы сможете быстро начать работу со средой и CLI, чтобы решить, подходит ли это средство для вас, либо с базовым образом.</span><span class="sxs-lookup"><span data-stu-id="52941-106">This lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or allows you to use this as a base image.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="52941-107">Установка с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="52941-107">Install with Docker</span></span>

<span data-ttu-id="52941-108">Установите CLI с помощью команды `docker run`.</span><span class="sxs-lookup"><span data-stu-id="52941-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli:<version>
   ```

<span data-ttu-id="52941-109">См. доступные версии на странице с [тегами Docker](https://hub.docker.com/r/microsoft/azure-cli/tags/).</span><span class="sxs-lookup"><span data-stu-id="52941-109">See our [Docker tags](https://hub.docker.com/r/microsoft/azure-cli/tags/) for available versions.</span></span>

<span data-ttu-id="52941-110">CLI устанавливается в образ как команда `az` в папку `/usr/local/bin`.</span><span class="sxs-lookup"><span data-stu-id="52941-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="52941-111">Если вы хотите взять ключи SSH из среды пользователя, можно использовать `-v ${HOME}:/root`, чтобы подключить $HOME как `/root`.</span><span class="sxs-lookup"><span data-stu-id="52941-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli:<version>
> ```

### <a name="update-with-docker"></a><span data-ttu-id="52941-112">Обновление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="52941-112">Update with Docker</span></span>

<span data-ttu-id="52941-113">Для обновления с помощью Docker требуется извлечь новый образ и повторно создать существующие контейнеры.</span><span class="sxs-lookup"><span data-stu-id="52941-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="52941-114">По этой причине не следует использовать контейнер, в котором размещается CLI, в качестве хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="52941-114">For this reason you should try and avoid using a container which hosts the CLI as a data store.</span></span>

1. <span data-ttu-id="52941-115">Обновите локальный образ с помощью команды `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="52941-115">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull microsoft/azure-cli
   ```

2. <span data-ttu-id="52941-116">Получите данные о контейнерах, которые используют образ CLI.</span><span class="sxs-lookup"><span data-stu-id="52941-116">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

  > [!NOTE]
  > <span data-ttu-id="52941-117">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="52941-117">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="52941-118">Остановите и заново создайте контейнеры.</span><span class="sxs-lookup"><span data-stu-id="52941-118">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run microsoft/azure-cli
   ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="52941-119">Удаление с помощью Docker</span><span class="sxs-lookup"><span data-stu-id="52941-119">Uninstall with Docker</span></span>

<span data-ttu-id="52941-120">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="52941-120">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="52941-121">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="52941-121">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="52941-122">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="52941-122">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="52941-123">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="52941-123">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="52941-124">Чтобы удалить образ Docker CLI, вам нужно сначала удалить все контейнеры, на которых он запущен, а затем — локальный образ.</span><span class="sxs-lookup"><span data-stu-id="52941-124">To properly uninstall the CLI Docker image you need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="52941-125">Получите данные о контейнерах, на которых запущен образ azure-cli.</span><span class="sxs-lookup"><span data-stu-id="52941-125">Get the containers running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=microsoft/azure-cli'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        microsoft/azure-cli:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```
  > [!NOTE]
  > <span data-ttu-id="52941-126">Если вы установили определенную версию образа, вам нужно добавить `:<version>` в конец имени образа.</span><span class="sxs-lookup"><span data-stu-id="52941-126">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

2. <span data-ttu-id="52941-127">Удалите все контейнеры с образом CLI.</span><span class="sxs-lookup"><span data-stu-id="52941-127">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="52941-128">Удалите локально установленный образ CLI.</span><span class="sxs-lookup"><span data-stu-id="52941-128">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi microsoft/azure-cli
   ```

