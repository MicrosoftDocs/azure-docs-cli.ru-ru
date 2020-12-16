---
title: Обновление Azure CLI
description: Справочник по обновлению Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 475b58bca5ec9dca52a70416cb89860dcbd39278
ms.sourcegitcommit: e1faf297ba2cdf2ba7e821fbeedff9c9a724c975
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "97576791"
---
# <a name="update-the-azure-cli"></a><span data-ttu-id="e1578-103">Обновление Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e1578-103">Update the Azure CLI</span></span>

<span data-ttu-id="e1578-104">Для обновления локальной установки Azure CLI в средах Windows, macOS и Linux (см. раздел `Update` в инструкциях по установке для конкретной платформы) можно использовать диспетчер пакетов.</span><span class="sxs-lookup"><span data-stu-id="e1578-104">You can rely on package managers to update a local install of the Azure CLI on Windows, macOS and Linux environments (see the `Update` section in each platform-specific install instruction).</span></span> <span data-ttu-id="e1578-105">CLI также предоставляет встроенные команды для обновления вручную или автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="e1578-105">The CLI also provides in-tool commands to upgrade manually or automatically.</span></span>

## <a name="manual-update"></a><span data-ttu-id="e1578-106">Обновление вручную</span><span class="sxs-lookup"><span data-stu-id="e1578-106">Manual Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="e1578-107">`az upgrade` поддерживается в Windows, macOS и некоторых дистрибутивах Linux, если поддерживается сама установка.</span><span class="sxs-lookup"><span data-stu-id="e1578-107">`az upgrade` is supported on Windows, macOS and some Linux distros as long as installation is supported.</span></span> <span data-ttu-id="e1578-108">При этом можно выполнить только обновление до последней версии.</span><span class="sxs-lookup"><span data-stu-id="e1578-108">It only supports upgrading to the latest version.</span></span> <span data-ttu-id="e1578-109">Если вы используете Azure CLI в Azure Cloud Shell, скорее всего, вы уже используете самую последнюю установку Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="e1578-109">If you are running the Azure CLI through Azure Cloud Shell, you are most likely already using the most recent Azure CLI install.</span></span> <span data-ttu-id="e1578-110">Кроме ситуаций с исправлением незначительной ошибки в дополнительной версии, необходимо дождаться выпуска следующей сборки Azure Cloud Shell, так как Azure Cloud Shell не поддерживает `az upgrade`.</span><span class="sxs-lookup"><span data-stu-id="e1578-110">If not due to cases like ad-hoc release of a minor bug fix version, you need to wait for the next build of Azure Cloud Shell as `az upgrade` is not supported in Azure Cloud Shell.</span></span>

<span data-ttu-id="e1578-111">Если `azure-cli` уже является последней версией, при выполнении `az upgrade` будут проверены и обновлены все установленные [расширения](azure-cli-extensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e1578-111">When `azure-cli` is already the latest version, running `az upgrade` will check and update all installed [extensions](azure-cli-extensions-overview.md).</span></span>

## <a name="automatic-update"></a><span data-ttu-id="e1578-112">Автоматическое обновление</span><span class="sxs-lookup"><span data-stu-id="e1578-112">Automatic Update</span></span>

<span data-ttu-id="e1578-113">По умолчанию автоматическое обновление для Azure CLI отключено.</span><span class="sxs-lookup"><span data-stu-id="e1578-113">By default, auto-upgrade for Azure CLI is disabled.</span></span> <span data-ttu-id="e1578-114">Чтобы включить автоматическое обновление до последней версии, нужно изменить [конфигурацию](/cli/azure/config).</span><span class="sxs-lookup"><span data-stu-id="e1578-114">If you would like to keep up with the latest version, you can enable auto-upgrade through [configuration](/cli/azure/config).</span></span>

```azurecli
az config set auto-upgrade.enable=yes
```

<span data-ttu-id="e1578-115">Azure CLI будет регулярно проверять наличие новых версий и предлагать вам обновить систему после выполнения любой команды, когда обновление станет доступным.</span><span class="sxs-lookup"><span data-stu-id="e1578-115">The Azure CLI will check new versions regularly and prompt you to upgrade after any command finishes running once the update is available.</span></span>

<span data-ttu-id="e1578-116">Появление сообщения с запросом или выходных сообщений во время обновления может привести к прерыванию выполнения команды, если она назначена переменной или выполняется в потоке автоматически.</span><span class="sxs-lookup"><span data-stu-id="e1578-116">The prompt message and output messages during upgrade may interrupt your command result if it is assigned to some variable or in an automated flow.</span></span> <span data-ttu-id="e1578-117">Чтобы избежать прерывания, можно использовать приведенную ниже конфигурацию. Она обеспечит автоматическое обновление без подтверждения. Во время обновления будут отображаться только предупреждения и сообщения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="e1578-117">To avoid interruption, you can use the following configuration to allow the update to happen automatically without confirmation and only show warnings and errors during the upgrade.</span></span>

```azurecli
az config set auto-upgrade.prompt=no
```

<span data-ttu-id="e1578-118">По умолчанию все установленные расширения также будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="e1578-118">By default, all installed extensions will also be updated.</span></span> <span data-ttu-id="e1578-119">Вы можете отключить обновление расширений, изменив конфигурацию.</span><span class="sxs-lookup"><span data-stu-id="e1578-119">You can disable extension update through configuration.</span></span>

```azurecli
az config set auto-upgrade.all=no
```

> [!NOTE]
> <span data-ttu-id="e1578-120">Дождитесь завершения выполнения `az upgrade`, прежде чем переходить к следующему набору команд. Иначе новые версии CLI (и расширения) могут включать критические изменения.</span><span class="sxs-lookup"><span data-stu-id="e1578-120">Please wait for `az upgrade` to complete before proceeding to the next set of commands, else the new versions of the CLI (+extensions) may have breaking changes.</span></span>

<span data-ttu-id="e1578-121">Если вы решили не использовать функцию автоматического обновления (например, если вам нужно сохранить стабильное выполнение командных скриптов), ее можно отключить, изменив конфигурацию.</span><span class="sxs-lookup"><span data-stu-id="e1578-121">If you decide not to use the automatic update feature any more for cases like keeping command scripts running stably, you can turn it off through configuration.</span></span>
```azurecli
az config set auto-upgrade.enable=no
```
