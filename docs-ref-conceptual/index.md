---
title: Общие сведения об Azure CLI 2.0
description: Общие сведения об Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388394"
---
# <a name="azure-cli-20"></a><span data-ttu-id="02b89-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="02b89-103">Azure CLI 2.0</span></span>

<span data-ttu-id="02b89-104">Azure CLI 2.0 — это кроссплатформенный интерфейс командной строки от Майкрософт для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="02b89-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="02b89-105">Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.</span><span class="sxs-lookup"><span data-stu-id="02b89-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="02b89-106">Начать работу с Azure CLI 2.0 очень просто. Этот инструмент лучше всего подходит для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="02b89-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="02b89-107">С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:</span><span class="sxs-lookup"><span data-stu-id="02b89-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="02b89-108">Запуск или установка</span><span class="sxs-lookup"><span data-stu-id="02b89-108">Run or Install</span></span>

<span data-ttu-id="02b89-109">CLI можно установить локально, запустить в контейнере Docker или браузере с помощью Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="02b89-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="02b89-110">Сведения о запуске Azure Cloud Shell в браузере см. в статье [Краткое руководство по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart) или [Краткое руководство по использованию PowerShell в Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="02b89-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="02b89-111">Сведения об установке CLI см. в статье [Установка Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="02b89-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="02b89-112">Сведения о запуске в контейнере Docker см. в статье [Запуск Azure CLI 2.0 в контейнере Docker](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="02b89-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="02b89-113">Начало работы</span><span class="sxs-lookup"><span data-stu-id="02b89-113">Get started</span></span>

<span data-ttu-id="02b89-114">Основные сведения о CLI см. в статье о [начале работы](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="02b89-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="02b89-115">В следующих примерах показаны некоторые из распространенных вариантов использования:</span><span class="sxs-lookup"><span data-stu-id="02b89-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="02b89-116">Виртуальные машины Linux</span><span class="sxs-lookup"><span data-stu-id="02b89-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="02b89-117">Виртуальные машины Windows</span><span class="sxs-lookup"><span data-stu-id="02b89-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="02b89-118">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="02b89-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="02b89-119">База данных SQL</span><span class="sxs-lookup"><span data-stu-id="02b89-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="02b89-120">В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="02b89-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="02b89-121">Если вы используете предыдущую версию интерфейса командной строки (Azure CLI 1.0), вы можете продолжать использовать ее.</span><span class="sxs-lookup"><span data-stu-id="02b89-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="02b89-122">Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="02b89-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="02b89-123">При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="02b89-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>
