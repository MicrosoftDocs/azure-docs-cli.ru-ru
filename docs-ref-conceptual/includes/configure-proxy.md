---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516236"
---
<span data-ttu-id="45876-101">Если вы не можете подключиться к внешнему ресурсу из-за прокси-сервера, убедитесь, что вы правильно задали переменные `HTTP_PROXY` и `HTTPS_PROXY` в оболочке.</span><span class="sxs-lookup"><span data-stu-id="45876-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="45876-102">Обратитесь к системному администратору, чтобы узнать, какие узлы и порты использовать для этих прокси-серверов.</span><span class="sxs-lookup"><span data-stu-id="45876-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="45876-103">Эти значения учитываются многими программами Linux, включая те, которые используются в процессе установки.</span><span class="sxs-lookup"><span data-stu-id="45876-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="45876-104">Чтобы задать эти значения, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="45876-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="45876-105">Если вы работаете за прокси-сервером, эти переменные оболочки должны быть заданы для подключения к службам Azure с помощью CLI.</span><span class="sxs-lookup"><span data-stu-id="45876-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="45876-106">Если вы не используете обычную аутентификацию, рекомендуется экспортировать эти переменные в файл `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="45876-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="45876-107">Всегда следуйте корпоративным политикам безопасности и учитывайте требования системного администратора.</span><span class="sxs-lookup"><span data-stu-id="45876-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>
