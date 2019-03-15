---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2018
ms.topic: include
ms.openlocfilehash: ee0b2b0c8c557aa54255f28429bb3a174c0e21a9
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158858"
---
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a><span data-ttu-id="83275-101">Не удается установить или запустить CLI в подсистеме Windows для Linux</span><span class="sxs-lookup"><span data-stu-id="83275-101">CLI fails to install or run on Windows Subsystem for Linux</span></span>

<span data-ttu-id="83275-102">[Подсистема Windows для Linux (WSL)](/windows/wsl/about) — это уровень преобразования системных вызовов поверх платформы Windows, поэтому при попытке установить или запустить Azure CLI вы можете получить сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="83275-102">Since [Windows Subsystem for Linux (WSL)](/windows/wsl/about) is a system call translation layer on top of the Windows platform, you might experience an error when trying to install or run the Azure CLI.</span></span> <span data-ttu-id="83275-103">CLI использует набор функций, которые в WSL могут быть реализованы с ошибками.</span><span class="sxs-lookup"><span data-stu-id="83275-103">The CLI relies on some features that may have a bug in WSL.</span></span> <span data-ttu-id="83275-104">Если независимо от процедуры установки CLI вы получаете сообщение об ошибке, вероятнее всего, проблема связана с WSL, а не с процессом установки CLI.</span><span class="sxs-lookup"><span data-stu-id="83275-104">If you experience an error no matter how you install the CLI, there's a good chance it's an issue with WSL and not with the CLI install process.</span></span>

<span data-ttu-id="83275-105">Чтобы найти причину проблем с установкой в WSL и попытаться устранить ее, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="83275-105">To troubleshoot your WSL installation and possibly resolve issues:</span></span>

* <span data-ttu-id="83275-106">При возможности выполните идентичный процесс установки на компьютере или виртуальной машине с Linux, чтобы проверить успешность установки.</span><span class="sxs-lookup"><span data-stu-id="83275-106">If you can, run an identical install process on a Linux machine or VM to see if it succeeds.</span></span> <span data-ttu-id="83275-107">Если установка прошла успешно, почти наверняка, проблема связана с WSL.</span><span class="sxs-lookup"><span data-stu-id="83275-107">If it does, your issue is almost certainly related to WSL.</span></span> <span data-ttu-id="83275-108">Чтобы запустить виртуальную машину в Azure, см. документацию по [созданию виртуальной машины Linux на портале Azure](/azure/virtual-machines/linux/quick-create-portal).</span><span class="sxs-lookup"><span data-stu-id="83275-108">To start a Linux VM in Azure, see the [create a Linux VM in the Azure Portal](/azure/virtual-machines/linux/quick-create-portal) documentation.</span></span>
* <span data-ttu-id="83275-109">Убедитесь, что вы используете последнюю версию WSL.</span><span class="sxs-lookup"><span data-stu-id="83275-109">Make sure that you're running the latest version of WSL.</span></span> <span data-ttu-id="83275-110">Чтобы получить последнюю версию, [обновите ОС Windows 10 на своем компьютере](https://support.microsoft.com/help/4027667/windows-10-update).</span><span class="sxs-lookup"><span data-stu-id="83275-110">To get the latest version, [update your Windows 10 installation](https://support.microsoft.com/help/4027667/windows-10-update).</span></span>
* <span data-ttu-id="83275-111">Проверьте [отправленные сообщения о проблемах](https://github.com/Microsoft/WSL/issues) с WSL, которые могут иметь отношение к вашему случаю.</span><span class="sxs-lookup"><span data-stu-id="83275-111">Check for any [open issues](https://github.com/Microsoft/WSL/issues) with WSL which might address your problem.</span></span>
  <span data-ttu-id="83275-112">Часто в них можно найти предложения относительно того, как обойти проблему, или сведения о выпуске, в котором проблема будет исправлена.</span><span class="sxs-lookup"><span data-stu-id="83275-112">Often there will be suggestions on how to work around the problem, or information about a release where the issue will be fixed.</span></span>
* <span data-ttu-id="83275-113">Если вы не смогли найти свой случай в существующих сообщениях о проблемах, [сообщите о проблеме с WSL](https://github.com/Microsoft/WSL/issues/new) и включите в сообщение как можно больше сведений.</span><span class="sxs-lookup"><span data-stu-id="83275-113">If there are no existing issues for your problem, [file a new issue with WSL](https://github.com/Microsoft/WSL/issues/new) and make sure that you include as much information as possible.</span></span>

<span data-ttu-id="83275-114">Если у вас по-прежнему наблюдаются проблемы при установке или запуске в WSL, рассмотрите возможность [установки CLI для Windows](../install-azure-cli-windows.md).</span><span class="sxs-lookup"><span data-stu-id="83275-114">If you continue to have issues installing or running on WSL, consider [installing the CLI for Windows](../install-azure-cli-windows.md).</span></span>