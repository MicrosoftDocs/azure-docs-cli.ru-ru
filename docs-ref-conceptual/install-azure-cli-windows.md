---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff4ed838351167410c75c046dc8f615faa0930f5
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593223"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="37cd8-103">Установка Azure CLI в Windows</span><span class="sxs-lookup"><span data-stu-id="37cd8-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="37cd8-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="37cd8-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="37cd8-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="37cd8-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="37cd8-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="37cd8-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="37cd8-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="37cd8-107">Install or update</span></span>

<span data-ttu-id="37cd8-108">Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.</span><span class="sxs-lookup"><span data-stu-id="37cd8-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="37cd8-109">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="37cd8-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="37cd8-110">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="37cd8-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="37cd8-111">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="37cd8-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="37cd8-112">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="37cd8-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="37cd8-113">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="37cd8-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="37cd8-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="37cd8-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="37cd8-115">Удаление</span><span class="sxs-lookup"><span data-stu-id="37cd8-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="37cd8-116">Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".</span><span class="sxs-lookup"><span data-stu-id="37cd8-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="37cd8-117">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="37cd8-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a><span data-ttu-id="37cd8-118">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="37cd8-118">Next Steps</span></span>

<span data-ttu-id="37cd8-119">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="37cd8-119">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="37cd8-120">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="37cd8-120">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
