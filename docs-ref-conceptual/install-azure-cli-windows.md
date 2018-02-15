---
title: "Установка Azure CLI для Windows"
description: "Как установить Azure CLI 2.0 в Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3e732ea7fae118ddb1564bed28d54d15bab4f7f0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="57b14-103">Установка Azure CLI 2.0 в Windows</span><span class="sxs-lookup"><span data-stu-id="57b14-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="57b14-104">В Windows двоичный файл Azure CLI устанавливается с помощью установщика MSI, который предоставляет доступ к CLI через командную строку Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="57b14-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="57b14-105">При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="57b14-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="57b14-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="57b14-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="57b14-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="57b14-107">Install or update</span></span>

<span data-ttu-id="57b14-108">Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.</span><span class="sxs-lookup"><span data-stu-id="57b14-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="57b14-109">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="57b14-109">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

<span data-ttu-id="57b14-110">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="57b14-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="57b14-111">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="57b14-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="57b14-112">PowerShell предоставляет несколько функций заполнения нажатием клавиши TAB, которые недоступны в CMD.</span><span class="sxs-lookup"><span data-stu-id="57b14-112">PowerShell offers some tab completion features not available from CMD.</span></span>

## <a name="uninstall"></a><span data-ttu-id="57b14-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="57b14-113">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="57b14-114">Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".</span><span class="sxs-lookup"><span data-stu-id="57b14-114">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="57b14-115">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="57b14-115">Download the MSI installer</span></span>](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
