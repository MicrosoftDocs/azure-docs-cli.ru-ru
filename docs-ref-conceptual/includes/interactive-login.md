---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: include
ms.openlocfilehash: 7aae9e9050306ee834858e528504ae87ff605fa0
ms.sourcegitcommit: 488d53525f1c647ea853d9227d95fdce35b9fb85
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "93331122"
---
1. <span data-ttu-id="7261f-101">Выполните команду `login`.</span><span class="sxs-lookup"><span data-stu-id="7261f-101">Run the `login` command.</span></span>

    ```azurecli-interactive
    az login
    ```

    <span data-ttu-id="7261f-102">Если в CLI можно запустить браузер по умолчанию, откроется браузер со страницей входа.</span><span class="sxs-lookup"><span data-stu-id="7261f-102">If the CLI can open your default browser, it will do so and load an Azure sign-in page.</span></span>

    <span data-ttu-id="7261f-103">Если нет, самостоятельно откройте в браузере страницу [https://aka.ms/devicelogin](https://aka.ms/devicelogin) и введите код авторизации, отображаемый в терминале.</span><span class="sxs-lookup"><span data-stu-id="7261f-103">Otherwise, open a browser page at [https://aka.ms/devicelogin](https://aka.ms/devicelogin) and enter the  authorization code displayed in your terminal.</span></span>

    <span data-ttu-id="7261f-104">Если веб-браузер недоступен или его не удается открыть, используйте поток кода устройства с применением **az login --use-device-code**.</span><span class="sxs-lookup"><span data-stu-id="7261f-104">If no web browser is available or the web browser fails to open, use device code flow with **az login --use-device-code**.</span></span>

2. <span data-ttu-id="7261f-105">Выполните вход в браузере с помощью учетных данных.</span><span class="sxs-lookup"><span data-stu-id="7261f-105">Sign in with your account credentials in the browser.</span></span>
