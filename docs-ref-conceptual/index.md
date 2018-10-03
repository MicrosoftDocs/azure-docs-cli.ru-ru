---
title: Общие сведения об Azure CLI
description: Общие сведения об Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 047a953a0ab8ccaf145d56e4d774d2bf9852ed6f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177731"
---
# <a name="azure-cli"></a><span data-ttu-id="24eef-103">Инфраструктура CLI Azure</span><span class="sxs-lookup"><span data-stu-id="24eef-103">Azure CLI</span></span>

<span data-ttu-id="24eef-104">Azure CLI — это кроссплатформенный интерфейс командной строки от Майкрософт для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="24eef-104">The Azure CLI is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="24eef-105">Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.</span><span class="sxs-lookup"><span data-stu-id="24eef-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="24eef-106">Начать работу с Azure CLI очень просто. Этот инструмент лучше всего подходит для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="24eef-106">The Azure CLI is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="24eef-107">С помощью Azure CLI можно легко создавать виртуальные машины в Azure простым вводом следующей команды:</span><span class="sxs-lookup"><span data-stu-id="24eef-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="24eef-108">Запуск или установка</span><span class="sxs-lookup"><span data-stu-id="24eef-108">Run or Install</span></span>

<span data-ttu-id="24eef-109">CLI можно установить локально, запустить в контейнере Docker или браузере с помощью Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="24eef-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="24eef-110">Сведения о запуске Azure Cloud Shell в браузере см. в статье [Краткое руководство по Bash в Azure Cloud Shell](/azure/cloud-shell/quickstart) или [Краткое руководство по использованию PowerShell в Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="24eef-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="24eef-111">Сведения об установке CLI см. в статье [Установка Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="24eef-111">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="24eef-112">Сведения о запуске в контейнере Docker см. в статье [Запуск Azure CLI в контейнере Docker](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="24eef-112">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="24eef-113">Развитие навыков с помощью Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="24eef-113">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="24eef-114">Управление виртуальными машинами с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="24eef-114">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="24eef-115">Управление службами Azure с помощью CLI</span><span class="sxs-lookup"><span data-stu-id="24eef-115">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="24eef-116">Другие интерактивные руководства</span><span class="sxs-lookup"><span data-stu-id="24eef-116">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="24eef-117">Начало работы</span><span class="sxs-lookup"><span data-stu-id="24eef-117">Get started</span></span>

<span data-ttu-id="24eef-118">Основные сведения о CLI см. в статье о [начале работы](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="24eef-118">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="24eef-119">В следующих примерах показаны некоторые из распространенных вариантов использования:</span><span class="sxs-lookup"><span data-stu-id="24eef-119">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="24eef-120">Виртуальные машины Linux</span><span class="sxs-lookup"><span data-stu-id="24eef-120">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24eef-121">Виртуальные машины Windows</span><span class="sxs-lookup"><span data-stu-id="24eef-121">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24eef-122">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="24eef-122">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="24eef-123">База данных SQL</span><span class="sxs-lookup"><span data-stu-id="24eef-123">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="24eef-124">В подробной [справочной информации](/cli/azure/reference-index) также описаны способы использования каждой отдельной команды Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="24eef-124">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="24eef-125">Если вы используете предыдущую версию интерфейса командной строки (классический интерфейс командной строки Azure), вы можете продолжать использовать ее.</span><span class="sxs-lookup"><span data-stu-id="24eef-125">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="24eef-126">Но для оптимальной работы мы рекомендуем выполнить обновление до последней версии Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="24eef-126">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="24eef-127">Если вы используете обе версии CLI, следует помнить, что команда `azure` вызывает классический интерфейс командной строки, а `az` — последнюю версию CLI.</span><span class="sxs-lookup"><span data-stu-id="24eef-127">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>
