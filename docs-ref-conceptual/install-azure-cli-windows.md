---
title: "Установка Azure CLI для Windows"
description: "Как установить Azure CLI 2.0 в Windows"
keywords: Azure CLI,Install Azure CLI,azure install windows, azure cli windows, azure windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-windows"></a><span data-ttu-id="99e96-104">Установка Azure CLI 2.0 в Windows</span><span class="sxs-lookup"><span data-stu-id="99e96-104">Install Azure CLI 2.0 on Windows</span></span>

<span data-ttu-id="99e96-105">В Windows вы можете установить собственный двоичный файл из MSI-файла, который затем можно использовать с помощью командной строки Windows и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="99e96-105">On Windows, you can install a native binary from an MSI, which you can use through the Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="99e96-106">При запуске подсистемы Windows для Linux (WSL) можно работать с пакетами, доступными для используемого вами дистрибутива.</span><span class="sxs-lookup"><span data-stu-id="99e96-106">If you are running Windows Subsystem for Linux (WSL) there are packages available for the distribution you are running.</span></span> <span data-ttu-id="99e96-107">Список поддерживаемых диспетчеров пакетов и сведения об установке в WSL вручную см. на [главной странице установки](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="99e96-107">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

## <a name="install-or-update-with-msi"></a><span data-ttu-id="99e96-108">Установка или обновление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="99e96-108">Install or update with MSI</span></span>

<span data-ttu-id="99e96-109">Распространяемый MSI-файл используется для установки, обновления и удаления команды `az` в Windows.</span><span class="sxs-lookup"><span data-stu-id="99e96-109">The MSI distributable is used for installing, updating, and uninstalling the `az` command on Windows.</span></span> <span data-ttu-id="99e96-110">Вы можете [скачать установщик MSI](https://aka.ms/InstallAzureCliWindows) и запустить его для установки или обновления.</span><span class="sxs-lookup"><span data-stu-id="99e96-110">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) and then run it to install or update.</span></span>

<span data-ttu-id="99e96-111">Если программа установки запрашивает разрешения на внесение изменений на вашем компьютере, установите флажок "Да".</span><span class="sxs-lookup"><span data-stu-id="99e96-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="99e96-112">Теперь можно запустить Azure CLI с помощью команды `az` из командной строки Windows или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="99e96-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span>

## <a name="uninstall-with-msi"></a><span data-ttu-id="99e96-113">Удаление с помощью MSI-файла</span><span class="sxs-lookup"><span data-stu-id="99e96-113">Uninstall with MSI</span></span>

<span data-ttu-id="99e96-114">Нам будет очень жаль, если вы решите удалить Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="99e96-114">If you ever decide to uninstall the Azure CLI, we're sorry to see you go.</span></span> <span data-ttu-id="99e96-115">Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт.</span><span class="sxs-lookup"><span data-stu-id="99e96-115">Before you uninstall, use the `az feedback` command to give us some reasons why you chose to uninstall and how we could improve the CLI experience.</span></span> <span data-ttu-id="99e96-116">Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании.</span><span class="sxs-lookup"><span data-stu-id="99e96-116">We want to make sure that the Azure CLI is as bug-free and user-friendly as we can make it.</span></span> <span data-ttu-id="99e96-117">Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="99e96-117">You can also [file a github issue](https://github.com/Azure/azure-cli/issues).</span></span>

<span data-ttu-id="99e96-118">Выполнить удаление можно в ходе повторного запуска MSI-файла и выбора команды "Удалить".</span><span class="sxs-lookup"><span data-stu-id="99e96-118">Uninstalling can be done by running the MSI again, and choosing the "Uninstall" option.</span></span> <span data-ttu-id="99e96-119">Вы можете [скачать установщик MSI](https://aka.ms/InstallAzureCliWindows), если у вас его нет.</span><span class="sxs-lookup"><span data-stu-id="99e96-119">You can [download the MSI installer](https://aka.ms/InstallAzureCliWindows) if you no longer have it available.</span></span>
