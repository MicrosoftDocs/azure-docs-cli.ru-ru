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
ms.openlocfilehash: e8103b8b235c7ac003b2434c72e69839a39f4a9f
ms.sourcegitcommit: e672284b83a9dbb46cbc54be17f5cd8512310e0a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "98594189"
---
# <a name="install-azure-cli-on-windows"></a>Установка Azure CLI в Windows

Azure CLI для Windows устанавливается с помощью MSI. Это предоставляет доступ к CLI из командной строки Windows (CMD) или PowerShell.
При установке подсистемы Windows для Linux (WSL) пакеты доступны для дистрибутива Linux. Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Установка или обновление

Распространяемый MSI-файл используется для установки или обновления Azure CLI в Windows. Вам не нужно удалять текущие версии перед использованием установщика MSI, так как MSI обновит существующую версию.

# <a name="microsoft-installer-msi"></a>[Установщик Майкрософт (MSI)](#tab/azure-cli)

Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".

### <a name="azure-cli-current-version"></a>Текущая версия Azure CLI

Скачайте и установите текущий выпуск Azure CLI.  

> [!div class="nextstepaction"]
> [Текущий выпуск Azure CLI](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a>Бета-версия Azure CLI

Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию. Бета-версия обеспечивает миграцию из выпущенной версии Azure CLI так как платформа проверки подлинности AAD (версия 1.0) является устаревшей.  [Платформа удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview) — это новый метод проверки подлинности, используемый бета-версией Azure CLI.  Мы рекомендуем опробовать бета-версию заранее.  

Дополнительные сведения о бета-версии Azure CLI см. в [заметках о выпуске](./release-notes-azure-cli.md?tabs=azure-cli-beta).

> [!IMPORTANT]
>
> Бета-версия не гарантирует высокое качество продукта, поэтому ее не следует использовать в рабочей среде.

Скачайте и установите бета-версию Azure CLI.

> [!div class="nextstepaction"]
> [Бета-версия Azure CLI](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-command"></a>[Установщик Майкрософт (MSI) с командой](#tab/azure-powershell)

### <a name="powershell-command"></a>Команда Powershell

Azure CLI также можно установить с помощью PowerShell. Запустите PowerShell с правами администратора и выполните следующую команду:

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

Будет скачана и установлена последняя версия Azure CLI для Windows. Если у вас уже установлена определенная версия, установщик обновит ее. По завершении установки необходимо снова открыть PowerShell, чтобы использовать Azure CLI.

### <a name="azure-cli-command-for-update-only"></a>Команда Azure CLI (только для обновления)
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a>Запуск Azure CLI

Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell. В PowerShell реализовано несколько функций заполнения нажатием клавиши TAB, которые недоступны в командной строке Windows. Чтобы войти, выполните команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы с установкой в Windows. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Прокси-сервер блокирует подключения

Если вы не можете скачать установщик MSI, так как прокси-сервер блокирует подключение, убедитесь, что этот прокси-сервер правильно настроен. В Windows 10 управление этими параметрами осуществляется в области `Settings > Network & Internet > Proxy`. Чтобы настроить обязательные параметры или решить вопросы, связанные с компьютером, который управляется с помощью конфигурации или для которого требуется расширенная настройка, обратитесь к системному администратору.

> [!IMPORTANT]
> Эти параметры также требуются для доступа к службам Azure с помощью CLI, PowerShell или командной строки. В PowerShell выполните для этого следующую команду:
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

Чтобы вы могли получить MSI, ваш прокси-сервер должен разрешать HTTPS-подключения по следующим адресам:

* `https://aka.ms/`
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Удалите Azure CLI из списка "Приложения и возможности" в Windows. Для удаления сделайте следующее:

| Платформа | Instructions |
|---|---|
| Windows 10 | Пуск > Параметры > Приложения |
| Windows 8 и Windows 7 | Пуск > Панель управления > Программы > Удалить программу |

На этом экране введите __Azure CLI__ в строке поиска программы. Программа для удаления называется __Microsoft CLI 2.0 для Azure__. Выберите это приложение, а затем нажмите кнопку `Uninstall`.

## <a name="next-steps"></a>Next Steps

Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.

> [!div class="nextstepaction"]
> [Начало работы с Azure CLI](get-started-with-azure-cli.md)