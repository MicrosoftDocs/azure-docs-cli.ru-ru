---
title: Установка Azure CLI для Linux вручную
description: Как установить Azure CLI в Linux вручную
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
zone_pivot_group_filename: azure/zone-pivot-groups.json
zone_pivot_groups: cli-linux-installation-method
ms.openlocfilehash: 03c7e7e4915f48dce70d2bc2cab16b4688f8b5fd
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631031"
---
# <a name="install-the-azure-cli-on-linux"></a><span data-ttu-id="a194f-103">Установка Azure CLI в Linux</span><span class="sxs-lookup"><span data-stu-id="a194f-103">Install the Azure CLI on Linux</span></span>

<span data-ttu-id="a194f-104">Рекомендуется устанавливать Azure CLI с помощью диспетчера пакетов соответствующего дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="a194f-104">It is recommended to install the Azure CLI using your Linux distribution's package manager.</span></span> <span data-ttu-id="a194f-105">Выберите диспетчер пакетов из приведенных выше вариантов.</span><span class="sxs-lookup"><span data-stu-id="a194f-105">Select the appropriate package manager for your distribution from the options above.</span></span>  <span data-ttu-id="a194f-106">Если у вас нет ни одного из перечисленных диспетчеров пакетов, можно вручную установить Azure CLI, выбрав вариант *Скрипт установки*.</span><span class="sxs-lookup"><span data-stu-id="a194f-106">If you do not have one of the listed package managers, you may manually install the Azure CLI by selecting the *Install script* option.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="dnf"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-dnf.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a><span data-ttu-id="a194f-107">Next Steps</span><span class="sxs-lookup"><span data-stu-id="a194f-107">Next Steps</span></span>

<span data-ttu-id="a194f-108">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="a194f-108">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a194f-109">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a194f-109">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
