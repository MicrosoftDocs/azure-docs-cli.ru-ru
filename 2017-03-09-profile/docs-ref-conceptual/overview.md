---
title: "Azure CLI 2.0"
description: "Общие сведения об Azure CLI 2.0."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 2f4f9950dd663ae85f41bf4efe114b15770ace5d
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: ru-RU
---
# <a name="azure-cli-20"></a><span data-ttu-id="2f52d-104">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="2f52d-104">Azure CLI 2.0</span></span>

<span data-ttu-id="2f52d-105">Azure CLI 2.0 — это новый интерфейс командной строки Azure для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="2f52d-105">The Azure CLI 2.0 is Azure's new command-line experience for managing Azure resources.</span></span>  <span data-ttu-id="2f52d-106">Его можно использовать в Windows, Linux и macOS.</span><span class="sxs-lookup"><span data-stu-id="2f52d-106">It can be used on macOS, Linux, and Windows.</span></span> 

<span data-ttu-id="2f52d-107">Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="2f52d-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="2f52d-108">С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:</span><span class="sxs-lookup"><span data-stu-id="2f52d-108">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="2f52d-109">См. статью об [установке](install-azure-cli.md), чтобы установить и запустить Azure CLI 2.0 на компьютере.</span><span class="sxs-lookup"><span data-stu-id="2f52d-109">Review the [Install article](install-azure-cli.md) to get Azure CLI 2.0 up and running on your system.</span></span> <span data-ttu-id="2f52d-110">Прежде чем начать использовать эту среду, прочтите статью о [начале работы](get-started-with-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2f52d-110">Then read the [Get Started](get-started-with-azure-cli.md) article to begin using it.</span></span>
<span data-ttu-id="2f52d-111">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2f52d-111">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="2f52d-112">Приведенные ниже примеры помогут вам понять, как реализовать типичные сценарии с помощью Azure CLI 2.0:</span><span class="sxs-lookup"><span data-stu-id="2f52d-112">The following samples can help you learn how to perform common scenarios with Azure CLI 2.0:</span></span>
- [<span data-ttu-id="2f52d-113">Виртуальные машины Linux</span><span class="sxs-lookup"><span data-stu-id="2f52d-113">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="2f52d-114">Виртуальные машины Windows</span><span class="sxs-lookup"><span data-stu-id="2f52d-114">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="2f52d-115">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="2f52d-115">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="2f52d-116">База данных SQL</span><span class="sxs-lookup"><span data-stu-id="2f52d-116">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="2f52d-117">В подробной [справочной информации](/cli/azure/) также описаны способы использования каждой отдельной команды Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="2f52d-117">A detailed [reference](/cli/azure/) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="2f52d-118">[Начните использовать](get-started-with-azure-cli.md) Azure CLI 2.0 сейчас.</span><span class="sxs-lookup"><span data-stu-id="2f52d-118">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>


> [!NOTE]
> <span data-ttu-id="2f52d-119">Если вы используете предыдущую версию интерфейса командной строки (Azure CLI), вы можете продолжать использовать ее.</span><span class="sxs-lookup"><span data-stu-id="2f52d-119">If you use the previous version of the CLI (Azure CLI), you can continue to use it.</span></span>
> <span data-ttu-id="2f52d-120">При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="2f52d-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span> 