---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI 2.0 в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 27284520d923524c5f772c82246889b2f1e6cb8b
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="17572-103">Установка Azure CLI 2.0 в Windows</span><span class="sxs-lookup"><span data-stu-id="17572-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="17572-104">В Windows двоичный файл Azure CLI устанавливается с помощью установщика MSI, который предоставляет доступ к CLI через командную строку Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17572-104">On Windows the Azure CLI binary is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="17572-105">При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для вашего дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="17572-105">If you are running Windows Subsystem for Linux (WSL), there are packages available for your Linux distribution.</span></span> <span data-ttu-id="17572-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="17572-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="17572-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="17572-107">Install or update</span></span>

<span data-ttu-id="17572-108">Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.</span><span class="sxs-lookup"><span data-stu-id="17572-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="17572-109">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="17572-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="17572-110">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="17572-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="17572-111">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17572-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="17572-112">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="17572-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="17572-113">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="17572-113">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="17572-114">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="17572-114">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="17572-115">Удаление</span><span class="sxs-lookup"><span data-stu-id="17572-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="17572-116">Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".</span><span class="sxs-lookup"><span data-stu-id="17572-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="17572-117">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="17572-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
