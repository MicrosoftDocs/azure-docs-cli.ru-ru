---
title: Установка Azure CLI для Windows
description: Как установить Azure CLI в Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 26e7f55d661928af78e645e820990a3617724644
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625386"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="129bf-103">Установка Azure CLI в Windows</span><span class="sxs-lookup"><span data-stu-id="129bf-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="129bf-104">Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="129bf-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="129bf-105">При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux.</span><span class="sxs-lookup"><span data-stu-id="129bf-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="129bf-106">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="129bf-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="129bf-107">Установка или обновление</span><span class="sxs-lookup"><span data-stu-id="129bf-107">Install or update</span></span>

<span data-ttu-id="129bf-108">Распространяемый MSI-файл используется для установки или обновления Azure CLI в Windows.</span><span class="sxs-lookup"><span data-stu-id="129bf-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="129bf-109">Вам не нужно удалять текущие версии перед использованием установщика MSI, так как MSI обновит существующую версию.</span><span class="sxs-lookup"><span data-stu-id="129bf-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="129bf-110">Установщик Майкрософт (MSI)</span><span class="sxs-lookup"><span data-stu-id="129bf-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="129bf-111">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="129bf-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="129bf-112">Текущая версия Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-112">Azure CLI current version</span></span>

<span data-ttu-id="129bf-113">Скачайте и установите текущий выпуск Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="129bf-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="129bf-114">Текущий выпуск Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="129bf-115">Бета-версия Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-115">Azure CLI beta version</span></span>

<span data-ttu-id="129bf-116">Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию.</span><span class="sxs-lookup"><span data-stu-id="129bf-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="129bf-117">Бета-версия обеспечивает миграцию из выпущенной версии Azure CLI так как платформа проверки подлинности AAD (версия 1.0) является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="129bf-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="129bf-118">[Платформа удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview) — это новый метод проверки подлинности, используемый бета-версией Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="129bf-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="129bf-119">Мы рекомендуем опробовать бета-версию заранее.</span><span class="sxs-lookup"><span data-stu-id="129bf-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="129bf-120">Дополнительные сведения о бета-версии Azure CLI см. в [заметках о выпуске](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="129bf-120">For more information about Azure CLI beta, please see [release notes](./release-notes-azure-cli.md?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="129bf-121">Бета-версия не гарантирует высокое качество продукта, поэтому ее не следует использовать в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="129bf-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="129bf-122">Скачайте и установите бета-версию Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="129bf-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="129bf-123">Бета-версия Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-command"></a>[<span data-ttu-id="129bf-124">Установщик Майкрософт (MSI) с командой</span><span class="sxs-lookup"><span data-stu-id="129bf-124">Microsoft Installer (MSI) with Command</span></span>](#tab/azure-powershell)

### <a name="powershell-command"></a><span data-ttu-id="129bf-125">Команда Powershell</span><span class="sxs-lookup"><span data-stu-id="129bf-125">Powershell Command</span></span>

<span data-ttu-id="129bf-126">Azure CLI также можно установить с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="129bf-126">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="129bf-127">Запустите PowerShell с правами администратора и выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="129bf-127">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="129bf-128">Будет скачана и установлена последняя версия Azure CLI для Windows.</span><span class="sxs-lookup"><span data-stu-id="129bf-128">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="129bf-129">Если у вас уже установлена определенная версия, установщик обновит ее.</span><span class="sxs-lookup"><span data-stu-id="129bf-129">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="129bf-130">По завершении установки необходимо снова открыть PowerShell, чтобы использовать Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="129bf-130">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

### <a name="azure-cli-command-for-update-only"></a><span data-ttu-id="129bf-131">Команда Azure CLI (только для обновления)</span><span class="sxs-lookup"><span data-stu-id="129bf-131">Azure CLI Command (for update only)</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="129bf-132">Запуск Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-132">Run the Azure CLI</span></span>

<span data-ttu-id="129bf-133">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="129bf-133">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="129bf-134">В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows.</span><span class="sxs-lookup"><span data-stu-id="129bf-134">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="129bf-135">Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).</span><span class="sxs-lookup"><span data-stu-id="129bf-135">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="129bf-136">Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="129bf-136">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="129bf-137">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="129bf-137">Troubleshooting</span></span>

<span data-ttu-id="129bf-138">Ниже описаны некоторые распространенные проблемы с установкой в Windows.</span><span class="sxs-lookup"><span data-stu-id="129bf-138">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="129bf-139">Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="129bf-139">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="129bf-140">Прокси-сервер блокирует подключения</span><span class="sxs-lookup"><span data-stu-id="129bf-140">Proxy blocks connection</span></span>

<span data-ttu-id="129bf-141">Если вы не можете скачать установщик MSI, так как прокси-сервер блокирует подключение, убедитесь, что этот прокси-сервер правильно настроен.</span><span class="sxs-lookup"><span data-stu-id="129bf-141">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="129bf-142">В Windows 10 управление этими параметрами осуществляется в области `Settings > Network & Internet > Proxy`.</span><span class="sxs-lookup"><span data-stu-id="129bf-142">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="129bf-143">Чтобы настроить обязательные параметры или решить вопросы, связанные с компьютером, который управляется с помощью конфигурации или для которого требуется расширенная настройка, обратитесь к системному администратору.</span><span class="sxs-lookup"><span data-stu-id="129bf-143">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="129bf-144">Эти параметры также требуются для доступа к службам Azure с помощью CLI, PowerShell или командной строки.</span><span class="sxs-lookup"><span data-stu-id="129bf-144">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="129bf-145">В PowerShell выполните для этого следующую команду:</span><span class="sxs-lookup"><span data-stu-id="129bf-145">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="129bf-146">Чтобы вы могли получить MSI, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:</span><span class="sxs-lookup"><span data-stu-id="129bf-146">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="129bf-147">Удаление</span><span class="sxs-lookup"><span data-stu-id="129bf-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="129bf-148">Удалите Azure CLI из списка "Приложения и возможности" в Windows.</span><span class="sxs-lookup"><span data-stu-id="129bf-148">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="129bf-149">Для удаления сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="129bf-149">To uninstall:</span></span>

| <span data-ttu-id="129bf-150">Платформа</span><span class="sxs-lookup"><span data-stu-id="129bf-150">Platform</span></span> | <span data-ttu-id="129bf-151">Instructions</span><span class="sxs-lookup"><span data-stu-id="129bf-151">Instructions</span></span> |
|---|---|
| <span data-ttu-id="129bf-152">Windows 10</span><span class="sxs-lookup"><span data-stu-id="129bf-152">Windows 10</span></span> | <span data-ttu-id="129bf-153">Пуск > Параметры > Приложения</span><span class="sxs-lookup"><span data-stu-id="129bf-153">Start > Settings > Apps</span></span> |
| <span data-ttu-id="129bf-154">Windows 8 и Windows 7</span><span class="sxs-lookup"><span data-stu-id="129bf-154">Windows 8 and Windows 7</span></span> | <span data-ttu-id="129bf-155">Пуск > Панель управления > Программы > Удалить программу</span><span class="sxs-lookup"><span data-stu-id="129bf-155">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="129bf-156">На этом экране введите __Azure CLI__ в строке поиска программы.</span><span class="sxs-lookup"><span data-stu-id="129bf-156">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="129bf-157">Программа для удаления называется __Microsoft CLI 2.0 для Azure__.</span><span class="sxs-lookup"><span data-stu-id="129bf-157">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="129bf-158">Выберите это приложение, а затем нажмите кнопку `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="129bf-158">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="129bf-159">Next Steps</span><span class="sxs-lookup"><span data-stu-id="129bf-159">Next Steps</span></span>

<span data-ttu-id="129bf-160">Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.</span><span class="sxs-lookup"><span data-stu-id="129bf-160">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="129bf-161">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="129bf-161">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)