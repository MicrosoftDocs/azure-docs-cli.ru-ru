---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI в Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5e9118a04b0dc608309093866307fdc7083f591
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417839"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="45cb9-103">Установка Azure CLI в Windows</span><span class="sxs-lookup"><span data-stu-id="45cb9-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="45cb9-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="45cb9-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="45cb9-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="45cb9-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="45cb9-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="45cb9-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="45cb9-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="45cb9-107">Install or update</span></span>

<span data-ttu-id="45cb9-108">Распространяемый MSI-файл используется для установки или обновления Azure CLI в Windows.</span><span class="sxs-lookup"><span data-stu-id="45cb9-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="45cb9-109">Удалять текущие версии перед использованием установщика MSI не нужно.</span><span class="sxs-lookup"><span data-stu-id="45cb9-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="45cb9-110">Скачать установщик MSI</span><span class="sxs-lookup"><span data-stu-id="45cb9-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="45cb9-111">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="45cb9-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="45cb9-112">Azure CLI также можно установить с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="45cb9-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="45cb9-113">Запустите PowerShell с правами администратора и выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="45cb9-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```
<span data-ttu-id="45cb9-114">Будет скачана и установлена последняя версия Azure CLI для Windows.</span><span class="sxs-lookup"><span data-stu-id="45cb9-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="45cb9-115">Если у вас уже установлена определенная версия, она будет обновлена до последней.</span><span class="sxs-lookup"><span data-stu-id="45cb9-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="45cb9-116">По завершении установки необходимо снова открыть PowerShell, чтобы использовать Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="45cb9-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="45cb9-117">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="45cb9-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="45cb9-118">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="45cb9-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="45cb9-119">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="45cb9-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="45cb9-120">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="45cb9-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="45cb9-121">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="45cb9-121">Troubleshooting</span></span>

<span data-ttu-id="45cb9-122">Ниже описаны некоторые распространенные проблемы с установкой в Windows.</span><span class="sxs-lookup"><span data-stu-id="45cb9-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="45cb9-123">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="45cb9-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="45cb9-124">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="45cb9-124">Proxy blocks connection</span></span>

<span data-ttu-id="45cb9-125">Если вы не можете скачать установщик MSI, так как прокси-сервер блокирует подключение, убедитесь, что этот прокси-сервер правильно настроен.</span><span class="sxs-lookup"><span data-stu-id="45cb9-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="45cb9-126">В Windows 10 управление этими параметрами осуществляется в области `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="45cb9-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="45cb9-127">Чтобы настроить обязательные параметры или решить вопросы, связанные с компьютером, который управляется с помощью конфигурации или для которого требуется расширенная настройка, обратитесь к системному администратору.</span><span class="sxs-lookup"><span data-stu-id="45cb9-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="45cb9-128">Эти параметры также требуются для доступа к службам Azure с помощью CLI, PowerShell или командной строки.</span><span class="sxs-lookup"><span data-stu-id="45cb9-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="45cb9-129">В PowerShell выполните для этого следующую команду:</span><span class="sxs-lookup"><span data-stu-id="45cb9-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="45cb9-130">Чтобы вы могли получить MSI, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="45cb9-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="45cb9-131">Удаление</span><span class="sxs-lookup"><span data-stu-id="45cb9-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="45cb9-132">Удалите Azure CLI из списка "Приложения и возможности" в Windows.</span><span class="sxs-lookup"><span data-stu-id="45cb9-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="45cb9-133">Для удаления сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="45cb9-133">To uninstall:</span></span>

| <span data-ttu-id="45cb9-134">Платформа</span><span class="sxs-lookup"><span data-stu-id="45cb9-134">Platform</span></span> | <span data-ttu-id="45cb9-135">Instructions</span><span class="sxs-lookup"><span data-stu-id="45cb9-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="45cb9-136">Windows 10</span><span class="sxs-lookup"><span data-stu-id="45cb9-136">Windows 10</span></span> | <span data-ttu-id="45cb9-137">Пуск > Параметры > Приложения</span><span class="sxs-lookup"><span data-stu-id="45cb9-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="45cb9-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="45cb9-138">Windows 8</span></span><br/><span data-ttu-id="45cb9-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="45cb9-139">Windows 7</span></span> | <span data-ttu-id="45cb9-140">Пуск > Панель управления > Программы > Удалить программу</span><span class="sxs-lookup"><span data-stu-id="45cb9-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="45cb9-141">На этом экране введите __Azure CLI__ в строке поиска программы.</span><span class="sxs-lookup"><span data-stu-id="45cb9-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="45cb9-142">Программа для удаления называется __Microsoft CLI 2.0 для Azure__.</span><span class="sxs-lookup"><span data-stu-id="45cb9-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="45cb9-143">Выберите это приложение, а затем нажмите кнопку `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="45cb9-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="45cb9-144">Next Steps</span><span class="sxs-lookup"><span data-stu-id="45cb9-144">Next Steps</span></span>

<span data-ttu-id="45cb9-145">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="45cb9-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="45cb9-146">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="45cb9-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
