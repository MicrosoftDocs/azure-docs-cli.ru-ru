---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI в Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240540"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="b9bf4-103">Установка Azure CLI в Windows</span><span class="sxs-lookup"><span data-stu-id="b9bf4-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="b9bf4-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="b9bf4-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="b9bf4-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b9bf4-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="b9bf4-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="b9bf4-107">Install or update</span></span>

<span data-ttu-id="b9bf4-108">Распространяемый MSI-файл используется для установки или обновления Azure CLI в Windows.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="b9bf4-109">Удалять текущие версии перед использованием установщика MSI не нужно.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="b9bf4-110">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="b9bf4-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="b9bf4-111">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="b9bf4-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="b9bf4-112">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="b9bf4-113">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="b9bf4-114">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="b9bf4-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="b9bf4-115">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b9bf4-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="b9bf4-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="b9bf4-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="b9bf4-117">Удалите Azure CLI из списка "Приложения и возможности" в Windows.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="b9bf4-118">Для удаления сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="b9bf4-118">To uninstall:</span></span>

| <span data-ttu-id="b9bf4-119">платформа</span><span class="sxs-lookup"><span data-stu-id="b9bf4-119">Platform</span></span> | <span data-ttu-id="b9bf4-120">Указания</span><span class="sxs-lookup"><span data-stu-id="b9bf4-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="b9bf4-121">Windows 10</span><span class="sxs-lookup"><span data-stu-id="b9bf4-121">Windows 10</span></span> | <span data-ttu-id="b9bf4-122">"Пуск" > "Параметры" > "Приложения"</span><span class="sxs-lookup"><span data-stu-id="b9bf4-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="b9bf4-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="b9bf4-123">Windows 8</span></span><br/><span data-ttu-id="b9bf4-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="b9bf4-124">Windows 7</span></span> | <span data-ttu-id="b9bf4-125">"Пуск" > "Панель управления" > "Программы" > "Удаление программы"</span><span class="sxs-lookup"><span data-stu-id="b9bf4-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="b9bf4-126">На этом экране введите __Azure CLI__ в строке поиска программы.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="b9bf4-127">Программа для удаления называется __Microsoft CLI 2.0 для Azure__.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="b9bf4-128">Выберите это приложение, а затем нажмите кнопку `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9bf4-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b9bf4-129">Next Steps</span></span>

<span data-ttu-id="b9bf4-130">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="b9bf4-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="b9bf4-131">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b9bf4-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
