---
title: Azure CLI 2.0
description: Общие сведения об Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9b6f7a5c79033c0b0bec2bf8b56eb40831484f1a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306256"
---
# <a name="azure-cli-20"></a><span data-ttu-id="8022f-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="8022f-103">Azure CLI 2.0</span></span>

<span data-ttu-id="8022f-104">Azure CLI 2.0 — это кроссплатформенный интерфейс командной строки Майкрософт для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="8022f-104">The Azure CLI 2.0 is Microsoft's cross-platform command line experience for managing Azure resources.</span></span>
<span data-ttu-id="8022f-105">Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.</span><span class="sxs-lookup"><span data-stu-id="8022f-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="8022f-106">Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="8022f-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="8022f-107">С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:</span><span class="sxs-lookup"><span data-stu-id="8022f-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="8022f-108">Запускайте интерфейс командной строки в браузере с помощью [Cloud Shell](/azure/cloud-shell/overview) либо [установите](install-azure-cli.md) его на платформе macOS, Linux или Windows.</span><span class="sxs-lookup"><span data-stu-id="8022f-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="8022f-109">Прежде чем начать использовать интерфейс командной строки, прочтите статью о [начале работы](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8022f-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="8022f-110">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8022f-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="8022f-111">Следующие примеры помогут вам приступить к выполнению распространенных задач в Azure CLI 2.0:</span><span class="sxs-lookup"><span data-stu-id="8022f-111">The following samples help you get started with common tasks in Azure CLI 2.0:</span></span>
- [<span data-ttu-id="8022f-112">Виртуальные машины Linux</span><span class="sxs-lookup"><span data-stu-id="8022f-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- <span data-ttu-id="8022f-113">Интерактивное руководство: [Создание Виртуальных машин Linux](https://docs.microsoft.com/learn/azure-cli-2-0/index)</span><span class="sxs-lookup"><span data-stu-id="8022f-113">Interactive: [Create Linux Virtual Machines](https://docs.microsoft.com/learn/azure-cli-2-0/index)</span></span>
- [<span data-ttu-id="8022f-114">Виртуальные машины Windows</span><span class="sxs-lookup"><span data-stu-id="8022f-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="8022f-115">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="8022f-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="8022f-116">База данных SQL</span><span class="sxs-lookup"><span data-stu-id="8022f-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="8022f-117">В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="8022f-117">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="8022f-118">[Начните использовать](get-started-with-azure-cli.md) Azure CLI 2.0 сейчас.</span><span class="sxs-lookup"><span data-stu-id="8022f-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>

> [!NOTE]
> <span data-ttu-id="8022f-119">Если вы используете предыдущую версию интерфейса командной строки (Azure CLI 1.0), вы можете продолжать использовать ее.</span><span class="sxs-lookup"><span data-stu-id="8022f-119">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="8022f-120">Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="8022f-120">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="8022f-121">При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="8022f-121">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
