---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI 2.0 в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 30bdb327601c7d898b5e64a3a472a104dc5db3b4
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388462"
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="93dbf-103">Установка Azure CLI 2.0 в Windows</span><span class="sxs-lookup"><span data-stu-id="93dbf-103">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="93dbf-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="93dbf-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="93dbf-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="93dbf-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="93dbf-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="93dbf-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="93dbf-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="93dbf-107">Install or update</span></span>

<span data-ttu-id="93dbf-108">Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.</span><span class="sxs-lookup"><span data-stu-id="93dbf-108">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="93dbf-109">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="93dbf-109">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="93dbf-110">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="93dbf-110">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="93dbf-111">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="93dbf-111">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="93dbf-112">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="93dbf-112">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="93dbf-113">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="93dbf-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="93dbf-114">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="93dbf-114">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="93dbf-115">Удаление</span><span class="sxs-lookup"><span data-stu-id="93dbf-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="93dbf-116">Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".</span><span class="sxs-lookup"><span data-stu-id="93dbf-116">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="93dbf-117">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="93dbf-117">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)
