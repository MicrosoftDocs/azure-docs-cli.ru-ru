---
ms.topic: include
ms.date: 09/10/2020
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4835cc399942fba3cbf7408b1309480cd2bcc152
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2021
ms.locfileid: "100631170"
---
## <a name="prerequisites"></a><span data-ttu-id="2cb23-101">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2cb23-101">Prerequisites</span></span>

- <span data-ttu-id="2cb23-102">[Azure Cloud Shell](/azure/cloud-shell/quickstart) можно использовать в среде Bash.</span><span class="sxs-lookup"><span data-stu-id="2cb23-102">Use [Azure Cloud Shell](/azure/cloud-shell/quickstart) using the bash environment.</span></span>

   <span data-ttu-id="2cb23-103">[![Внедрение запуска](https://shell.azure.com/images/launchcloudshell.png "Запуск Azure Cloud Shell")](https://shell.azure.com)</span><span class="sxs-lookup"><span data-stu-id="2cb23-103">[![Embed launch](https://shell.azure.com/images/launchcloudshell.png "Launch Azure Cloud Shell")](https://shell.azure.com)</span></span>   
- <span data-ttu-id="2cb23-104">При необходимости [установите](../install-azure-cli.md) Azure CLI, чтобы выполнять справочные команды CLI.</span><span class="sxs-lookup"><span data-stu-id="2cb23-104">If you prefer, [install](../install-azure-cli.md) the Azure CLI to run CLI reference commands.</span></span>
   - <span data-ttu-id="2cb23-105">Если вы используете локальную установку, выполните вход с помощью команды Azure CLI [az login](/cli/azure/reference-index#az_login).</span><span class="sxs-lookup"><span data-stu-id="2cb23-105">If you're using a local install, sign in with Azure CLI by using the [az login](/cli/azure/reference-index#az_login) command.</span></span>  <span data-ttu-id="2cb23-106">Чтобы выполнить аутентификацию, следуйте инструкциям в окне терминала.</span><span class="sxs-lookup"><span data-stu-id="2cb23-106">To finish the authentication process, follow the steps displayed in your terminal.</span></span>  <span data-ttu-id="2cb23-107">Сведения о дополнительных возможностях, доступных при входе, см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2cb23-107">See [Sign in with Azure CLI](../authenticate-azure-cli.md) for additional sign-in options.</span></span>
  - <span data-ttu-id="2cb23-108">Если появится запрос, установите расширения Azure CLI при первом использовании.</span><span class="sxs-lookup"><span data-stu-id="2cb23-108">When you're prompted, install Azure CLI extensions on first use.</span></span>  <span data-ttu-id="2cb23-109">Дополнительные сведения о расширениях см. в статье [Использование расширений с Azure CLI](../azure-cli-extensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2cb23-109">For more information about extensions, see [Use extensions with Azure CLI](../azure-cli-extensions-overview.md).</span></span>
  - <span data-ttu-id="2cb23-110">Выполните команду [az version](/cli/azure/reference-index#az_version), чтобы узнать установленную версию и зависимые библиотеки.</span><span class="sxs-lookup"><span data-stu-id="2cb23-110">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="2cb23-111">Чтобы обновиться до последней версии, выполните команду [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="2cb23-111">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>
