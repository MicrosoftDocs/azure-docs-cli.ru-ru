---
title: "Вход с помощью Azure CLI 2.0"
description: "Вход с помощью Azure CLI 2.0 на виртуальные машины Mac, Windows или Linux."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 3ba1dd840102c738ccd9eb62a0b9db612cec48d1
ms.sourcegitcommit: 5cfbea569fef193044da712708bc6957d3fb557c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2017
---
# <a name="log-in-with-azure-cli-20"></a><span data-ttu-id="69f95-104">Вход с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="69f95-104">Log in with Azure CLI 2.0</span></span>

<span data-ttu-id="69f95-105">Используя Azure CLI, можно входить и выполнять проверку подлинности несколькими способами.</span><span class="sxs-lookup"><span data-stu-id="69f95-105">There are several ways to log in and authenticate with the Azure CLI.</span></span> <span data-ttu-id="69f95-106">Проще всего начать со входа в интерактивном режиме из браузера или командной строки.</span><span class="sxs-lookup"><span data-stu-id="69f95-106">The simplest way to get started is to log in interactively through your browser, or to log in at the command line.</span></span> <span data-ttu-id="69f95-107">Рекомендуется использовать субъекты-службы. Они позволяют создавать неинтерактивные учетные записи, которые можно использовать для управления ресурсами.</span><span class="sxs-lookup"><span data-stu-id="69f95-107">Our recommended approach is to use service principals, which provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="69f95-108">Предоставляя только нужные разрешения, необходимые для субъекта-службы, вы можете обеспечить безопасность скриптов службы автоматизации.</span><span class="sxs-lookup"><span data-stu-id="69f95-108">By granting just the appropriate permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span> 

<span data-ttu-id="69f95-109">Учетные данные являются конфиденциальными и не хранятся локально.</span><span class="sxs-lookup"><span data-stu-id="69f95-109">None of your private credential information is stored locally.</span></span> <span data-ttu-id="69f95-110">Маркер проверки подлинности создается и сохраняется в Azure.</span><span class="sxs-lookup"><span data-stu-id="69f95-110">Instead, an authentication token is generated by Azure and stored.</span></span> <span data-ttu-id="69f95-111">После входа в систему локальный маркер для входа остается действительным в течение 14 дней без использования.</span><span class="sxs-lookup"><span data-stu-id="69f95-111">After logging in, your local login token is valid until it goes for 14 days without being used.</span></span> <span data-ttu-id="69f95-112">На этом этапе необходимо пройти повторную аутентификацию.</span><span class="sxs-lookup"><span data-stu-id="69f95-112">At that point, you will need to re-authenticate.</span></span>

<span data-ttu-id="69f95-113">Команды, которые вы выполняете с помощью интерфейса командной строки, выполняются в вашей подписке по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="69f95-113">Commands that you run with the CLI are run against your default subscription.</span></span>  <span data-ttu-id="69f95-114">Если у вас несколько подписок, может потребоваться [подтвердить подписку по умолчанию](manage-azure-subscriptions-azure-cli.md) и изменить ее соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="69f95-114">If you have more than one subscription, you may want to [confirm your default subscription](manage-azure-subscriptions-azure-cli.md) and change it appropriately.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="69f95-115">Интерактивный вход</span><span class="sxs-lookup"><span data-stu-id="69f95-115">Interactive log-in</span></span>

<span data-ttu-id="69f95-116">Выполните интерактивный вход из веб-браузера.</span><span class="sxs-lookup"><span data-stu-id="69f95-116">Log in interactively from your web browser.</span></span>

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a><span data-ttu-id="69f95-117">Команда</span><span class="sxs-lookup"><span data-stu-id="69f95-117">Command line</span></span>

<span data-ttu-id="69f95-118">Укажите свои учетные данные в командной строке.</span><span class="sxs-lookup"><span data-stu-id="69f95-118">Provide your credentials on the command line.</span></span>

> [!Note]
> <span data-ttu-id="69f95-119">Этот способ не работает с учетными записями Майкрософт или с учетными записями, которые используют двухфакторную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="69f95-119">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a><span data-ttu-id="69f95-120">Вход с использованием субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="69f95-120">Logging in with a service principal</span></span>

<span data-ttu-id="69f95-121">Субъекты-службы похожи на учетные записи пользователей, к которым можно применять правила, используя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="69f95-121">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span>
<span data-ttu-id="69f95-122">Проверка подлинности с помощью субъекта-службы — это самый безопасный способ использования ресурсов Azure из сценариев или приложений, которые работают с ресурсами.</span><span class="sxs-lookup"><span data-stu-id="69f95-122">Authenticating with a service principal is the best way to secure the usage of your Azure resources from either your scripts or applications that manipulate resources.</span></span>
<span data-ttu-id="69f95-123">Вы можете определить роли пользователей с помощью набора команд `az role`.</span><span class="sxs-lookup"><span data-stu-id="69f95-123">You define the roles you want your users to have via the `az role` set of commands.</span></span>
<span data-ttu-id="69f95-124">Дополнительные сведения и примеры ролей субъекта-службы см. в [справочных статьях о ролях az](https://docs.microsoft.com/cli/azure/role.md).</span><span class="sxs-lookup"><span data-stu-id="69f95-124">You can learn more and see examples of service principal roles in our [az role reference articles](https://docs.microsoft.com/cli/azure/role.md).</span></span>

1. <span data-ttu-id="69f95-125">Если у вас еще нет субъекта-службы, [создайте](create-an-azure-service-principal-azure-cli.md) его.</span><span class="sxs-lookup"><span data-stu-id="69f95-125">If you don't already have a service principal, [create one](create-an-azure-service-principal-azure-cli.md).</span></span>

1. <span data-ttu-id="69f95-126">Войдите с помощью субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="69f95-126">Log in with the service principal.</span></span>

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   <span data-ttu-id="69f95-127">Чтобы получить свой клиент, войдите в интерактивном режиме, а затем получите идентификатор из подписки.</span><span class="sxs-lookup"><span data-stu-id="69f95-127">To get your tenant, log in interactively and then get the tenantId from your subscription.</span></span>

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```