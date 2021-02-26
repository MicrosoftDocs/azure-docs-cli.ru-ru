---
title: Создание запроса на поддержку Azure в Azure CLI
description: Узнайте, как с помощью команд az support в Azure CLI создавать и обновлять запросы на поддержку Azure, а также управлять ими.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to
ms.openlocfilehash: 446fe0d3a6d7c726167d07e8eb5f4cfa2321d9b7
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631173"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a><span data-ttu-id="8a331-103">Создание запроса на поддержку Azure в Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8a331-103">Create an Azure support request in Azure CLI</span></span>

<span data-ttu-id="8a331-104">Azure CLI позволяет создавать запросы на поддержку Azure и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="8a331-104">The Azure CLI enables you to create and manage Azure support tickets.</span></span>

- <span data-ttu-id="8a331-105">Отправка в службу поддержки запросов, касающихся выставления счетов, управления подписками, а также ограничений (квот) на подписки и службы.</span><span class="sxs-lookup"><span data-stu-id="8a331-105">Open a technical, billing, subscription management, or subscription and service limits (quota) support ticket.</span></span>
- <span data-ttu-id="8a331-106">Получение списка запросов в службу поддержки и подробных сведений о каждом запросе.</span><span class="sxs-lookup"><span data-stu-id="8a331-106">Get a list of support tickets and detailed information about each ticket.</span></span> <span data-ttu-id="8a331-107">Вы можете уменьшить область поиска запросов в службу поддержки, отфильтровав их по состоянию или дате создания.</span><span class="sxs-lookup"><span data-stu-id="8a331-107">Narrow your search for support tickets by status or created date.</span></span>
- <span data-ttu-id="8a331-108">Обновление сведений о серьезности, состоянии и контактной информации для запроса в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="8a331-108">Update severity, ticket status, and contact information for a support ticket.</span></span>
- <span data-ttu-id="8a331-109">Добавление новой операции взаимодействия к запросу в службу поддержки или получение списка всех операций взаимодействия для запроса в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="8a331-109">Add a new communication to a support ticket or get a list of all communications for a support ticket.</span></span> <span data-ttu-id="8a331-110">Вы можете уменьшить область поиска списков операций взаимодействия, отфильтровав их дате создания или типу взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="8a331-110">Narrow your search of communication lists by created date or communication type.</span></span>

<span data-ttu-id="8a331-111">Чтобы создать запрос на поддержку, необходимо быть [владельцем](/azure/role-based-access-control/built-in-roles#owner) или [участником](/azure/role-based-access-control/built-in-roles#contributor) либо быть назначенным роли [Участник запроса на поддержку](/azure/role-based-access-control/built-in-roles#support-request-contributor) на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="8a331-111">To create a support request, you must be an [Owner](/azure/role-based-access-control/built-in-roles#owner) or [Contributor](/azure/role-based-access-control/built-in-roles#contributor), or be assigned to the [Support Request Contributor](/azure/role-based-access-control/built-in-roles#support-request-contributor) role at the subscription level.</span></span> <span data-ttu-id="8a331-112">Для создания запроса в службу поддержки без подписки, например в сценарии Azure Active Directory, необходимо быть [администратором](/azure/active-directory/roles/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a331-112">To create a support request without a subscription, such as an Azure Active Directory scenario, you must be an [Admin](/azure/active-directory/roles/permissions-reference).</span></span>

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a><span data-ttu-id="8a331-113">Создание запроса в службу поддержки</span><span class="sxs-lookup"><span data-stu-id="8a331-113">Create a support ticket</span></span>

1. <span data-ttu-id="8a331-114">Чтобы получить список служб, используйте команду [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):</span><span class="sxs-lookup"><span data-stu-id="8a331-114">To obtain a list of services, use the [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) command:</span></span>

   ```azurecli
   az support services list --output table
   ```

   <span data-ttu-id="8a331-115">Для этого примера найдите значение для **виртуальной машины под управлением Windows**. Это должно быть значение **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span><span class="sxs-lookup"><span data-stu-id="8a331-115">For this example, find the value for **Virtual Machine running Windows**, which is **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span></span>

1. <span data-ttu-id="8a331-116">Чтобы узнать тип и подтип проблемы, которые описывают вашу проблему, выполните команду [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list):</span><span class="sxs-lookup"><span data-stu-id="8a331-116">To get the problem type and problem subtype that describes your problem, run the [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) command:</span></span>

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   <span data-ttu-id="8a331-117">Для этого примера найдите сообщение об ошибке **Cannot connect to my VM / I have an issue with my public IP** (Не удается подключиться к виртуальной машине / Возникла проблема с общедоступным IP-адресом).</span><span class="sxs-lookup"><span data-stu-id="8a331-117">For this example, find **Cannot connect to my VM / I have an issue with my public IP**.</span></span> <span data-ttu-id="8a331-118">Этот тип имеет значение **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span><span class="sxs-lookup"><span data-stu-id="8a331-118">That type has a value of **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span></span>

1. <span data-ttu-id="8a331-119">Создайте запрос в службу поддержки с помощью команды [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create):</span><span class="sxs-lookup"><span data-stu-id="8a331-119">Create a ticket by using the [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) command:</span></span>

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

<span data-ttu-id="8a331-120">Инженер службы поддержки свяжется с вами, используя предпочитаемый вами канал связи.</span><span class="sxs-lookup"><span data-stu-id="8a331-120">A support engineer will contact you using the method you indicated.</span></span> <span data-ttu-id="8a331-121">Сведения об ожидаемом времени ответа см. на странице [Ограничения поддержки и время ответа на обращение в поддержку](/support/plans/response/).</span><span class="sxs-lookup"><span data-stu-id="8a331-121">For information about initial response times, see [Support scope and responsiveness](/support/plans/response/).</span></span>

## <a name="manage-support-tickets"></a><span data-ttu-id="8a331-122">Управление запросами в службу поддержки</span><span class="sxs-lookup"><span data-stu-id="8a331-122">Manage support tickets</span></span>

<span data-ttu-id="8a331-123">Чтобы просмотреть свои запросы в службу поддержки для текущей подписки, выполните команду [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list):</span><span class="sxs-lookup"><span data-stu-id="8a331-123">To see your support tickets for your current subscription, run the [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) command:</span></span>

```azurecli
az support tickets list
```

<span data-ttu-id="8a331-124">Чтобы просмотреть запросы в службу поддержки для другой подписки, измените текущую подписку с помощью команды [az account set](/cli/azure/account#az_account_set), а затем выполните приведенную выше команду.</span><span class="sxs-lookup"><span data-stu-id="8a331-124">To see support tickets in another subscription, run the [az account set](/cli/azure/account#az_account_set) command to change your current subscription, and then run the command.</span></span>

<span data-ttu-id="8a331-125">Можно также обновить запрос в службу поддержки с помощью команды [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update):</span><span class="sxs-lookup"><span data-stu-id="8a331-125">You can also update a ticket by using the [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) command:</span></span>

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a><span data-ttu-id="8a331-126">Отправка сообщений о запросе в службу поддержки</span><span class="sxs-lookup"><span data-stu-id="8a331-126">Communicate about your ticket</span></span>

<span data-ttu-id="8a331-127">Вы не можете удалить запрос в службу поддержки, созданный с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="8a331-127">You can't delete a support ticket created by using Azure CLI.</span></span> <span data-ttu-id="8a331-128">Вместо этого отправьте сообщение, чтобы закрыть этот запрос.</span><span class="sxs-lookup"><span data-stu-id="8a331-128">Instead, send a message to close a ticket.</span></span> <span data-ttu-id="8a331-129">Если вам нужно повторно открыть закрытый запрос на поддержку, создайте новое сообщение, после чего запрос будет автоматически открыт повторно.</span><span class="sxs-lookup"><span data-stu-id="8a331-129">If you need to reopen a closed support request, create a new message, which automatically reopens the request.</span></span>

<span data-ttu-id="8a331-130">Чтобы отправить сообщение о своем запросе, выполните команду [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create):</span><span class="sxs-lookup"><span data-stu-id="8a331-130">To communicate about your ticket, run the [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) command:</span></span>

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

<span data-ttu-id="8a331-131">Чтобы просмотреть все сообщения для запроса, используйте команду [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):</span><span class="sxs-lookup"><span data-stu-id="8a331-131">To see all the communications for a ticket, use the [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) command:</span></span>

```azurecli
az support tickets communications list --ticket-name VM012
```

<span data-ttu-id="8a331-132">Для этой команды есть параметр `--filters`, который позволяет отфильтровать ответы.</span><span class="sxs-lookup"><span data-stu-id="8a331-132">This command offers a `--filters` parameter to narrow your responses.</span></span>

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a><span data-ttu-id="8a331-133">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8a331-133">Next steps</span></span>

- [<span data-ttu-id="8a331-134">Часто задаваемые вопросы о поддержке Azure</span><span class="sxs-lookup"><span data-stu-id="8a331-134">Azure Support FAQs</span></span>](/support/faq/)
- [<span data-ttu-id="8a331-135">Понятие серьезности проблемы и ее уровни согласно классификации Azure</span><span class="sxs-lookup"><span data-stu-id="8a331-135">Azure severity and levels</span></span>](/support/plans/response/)
- [<span data-ttu-id="8a331-136">Как создать запрос в службу поддержки на портале Azure</span><span class="sxs-lookup"><span data-stu-id="8a331-136">How to create a support ticket via Azure portal</span></span>](/azure/azure-portal/supportability/how-to-create-azure-support-request)
