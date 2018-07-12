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
ms.openlocfilehash: ffa435f8c6ee5aa82d2efe2e09d7bcb1f1dc434b
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967696"
---
# <a name="azure-cli-20"></a><span data-ttu-id="9e123-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="9e123-103">Azure CLI 2.0</span></span>

<span data-ttu-id="9e123-104">Azure CLI 2.0 — это кроссплатформенный интерфейс командной строки Майкрософт для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="9e123-104">The Azure CLI 2.0 is Microsoft's cross-platform command line experience for managing Azure resources.</span></span>
<span data-ttu-id="9e123-105">Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.</span><span class="sxs-lookup"><span data-stu-id="9e123-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="9e123-106">Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9e123-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="9e123-107">С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:</span><span class="sxs-lookup"><span data-stu-id="9e123-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="9e123-108">Запускайте интерфейс командной строки в браузере с помощью [Cloud Shell](/azure/cloud-shell/overview) либо [установите](install-azure-cli.md) его на платформе macOS, Linux или Windows.</span><span class="sxs-lookup"><span data-stu-id="9e123-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="9e123-109">Прежде чем начать использовать интерфейс командной строки, прочтите статью о [начале работы](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9e123-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="9e123-110">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9e123-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="9e123-111">Следующие примеры помогут вам приступить к выполнению распространенных задач в Azure CLI 2.0:</span><span class="sxs-lookup"><span data-stu-id="9e123-111">The following samples help you get started with common tasks in Azure CLI 2.0:</span></span>

- [<span data-ttu-id="9e123-112">Виртуальные машины Linux</span><span class="sxs-lookup"><span data-stu-id="9e123-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9e123-113">Виртуальные машины Windows</span><span class="sxs-lookup"><span data-stu-id="9e123-113">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9e123-114">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="9e123-114">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="9e123-115">База данных SQL</span><span class="sxs-lookup"><span data-stu-id="9e123-115">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="9e123-116">В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="9e123-116">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="9e123-117">[Начните использовать](get-started-with-azure-cli.md) Azure CLI 2.0 сейчас.</span><span class="sxs-lookup"><span data-stu-id="9e123-117">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>

> [!NOTE]
> <span data-ttu-id="9e123-118">Если вы используете предыдущую версию интерфейса командной строки (Azure CLI 1.0), вы можете продолжать использовать ее.</span><span class="sxs-lookup"><span data-stu-id="9e123-118">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="9e123-119">Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="9e123-119">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="9e123-120">При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="9e123-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
