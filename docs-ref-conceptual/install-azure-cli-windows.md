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
ms.openlocfilehash: 40810b25bf776025c82b48ba7aa424369483ceeb
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516273"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="5cf52-103">Установка Azure CLI в Windows</span><span class="sxs-lookup"><span data-stu-id="5cf52-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="5cf52-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5cf52-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="5cf52-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="5cf52-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="5cf52-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5cf52-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="5cf52-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="5cf52-107">Install or update</span></span>

<span data-ttu-id="5cf52-108">Распространяемый MSI-файл используется для установки или обновления Azure CLI в Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf52-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="5cf52-109">Удалять текущие версии перед использованием установщика MSI не нужно.</span><span class="sxs-lookup"><span data-stu-id="5cf52-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5cf52-110">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="5cf52-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="5cf52-111">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="5cf52-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="5cf52-112">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5cf52-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="5cf52-113">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf52-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="5cf52-114">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="5cf52-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="5cf52-115">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="5cf52-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5cf52-116">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5cf52-116">Troubleshooting</span></span>

<span data-ttu-id="5cf52-117">Ниже описаны некоторые распространенные проблемы с установкой в Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf52-117">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="5cf52-118">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="5cf52-118">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="5cf52-119">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="5cf52-119">Proxy blocks connection</span></span>

<span data-ttu-id="5cf52-120">Если вы не можете скачать установщик MSI, так как прокси-сервер блокирует подключение, убедитесь, что этот прокси-сервер правильно настроен.</span><span class="sxs-lookup"><span data-stu-id="5cf52-120">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="5cf52-121">В Windows 10 управление этими параметрами осуществляется в области `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="5cf52-121">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="5cf52-122">Чтобы настроить обязательные параметры или решить вопросы, связанные с компьютером, который управляется с помощью конфигурации или для которого требуется расширенная настройка, обратитесь к системному администратору.</span><span class="sxs-lookup"><span data-stu-id="5cf52-122">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5cf52-123">Эти параметры также требуются для доступа к службам Azure с помощью CLI, PowerShell или командной строки.</span><span class="sxs-lookup"><span data-stu-id="5cf52-123">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="5cf52-124">В PowerShell выполните для этого следующую команду:</span><span class="sxs-lookup"><span data-stu-id="5cf52-124">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="5cf52-125">Чтобы вы могли получить MSI, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="5cf52-125">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="5cf52-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="5cf52-126">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="5cf52-127">Удалите Azure CLI из списка "Приложения и возможности" в Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf52-127">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="5cf52-128">Для удаления сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="5cf52-128">To uninstall:</span></span>

| <span data-ttu-id="5cf52-129">платформа</span><span class="sxs-lookup"><span data-stu-id="5cf52-129">Platform</span></span> | <span data-ttu-id="5cf52-130">Указания</span><span class="sxs-lookup"><span data-stu-id="5cf52-130">Instructions</span></span> |
|---|---|
| <span data-ttu-id="5cf52-131">Windows 10</span><span class="sxs-lookup"><span data-stu-id="5cf52-131">Windows 10</span></span> | <span data-ttu-id="5cf52-132">"Пуск" > "Параметры" > "Приложения"</span><span class="sxs-lookup"><span data-stu-id="5cf52-132">Start > Settings > Apps</span></span> |
| <span data-ttu-id="5cf52-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="5cf52-133">Windows 8</span></span><br/><span data-ttu-id="5cf52-134">Windows 7</span><span class="sxs-lookup"><span data-stu-id="5cf52-134">Windows 7</span></span> | <span data-ttu-id="5cf52-135">"Пуск" > "Панель управления" > "Программы" > "Удаление программы"</span><span class="sxs-lookup"><span data-stu-id="5cf52-135">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="5cf52-136">На этом экране введите __Azure CLI__ в строке поиска программы.</span><span class="sxs-lookup"><span data-stu-id="5cf52-136">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="5cf52-137">Программа для удаления называется __Microsoft CLI 2.0 для Azure__.</span><span class="sxs-lookup"><span data-stu-id="5cf52-137">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="5cf52-138">Выберите это приложение, а затем нажмите кнопку `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="5cf52-138">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5cf52-139">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5cf52-139">Next Steps</span></span>

<span data-ttu-id="5cf52-140">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="5cf52-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="5cf52-141">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5cf52-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
