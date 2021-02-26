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
# <a name="create-an-azure-support-request-in-azure-cli"></a>Создание запроса на поддержку Azure в Azure CLI

Azure CLI позволяет создавать запросы на поддержку Azure и управлять ими.

- Отправка в службу поддержки запросов, касающихся выставления счетов, управления подписками, а также ограничений (квот) на подписки и службы.
- Получение списка запросов в службу поддержки и подробных сведений о каждом запросе. Вы можете уменьшить область поиска запросов в службу поддержки, отфильтровав их по состоянию или дате создания.
- Обновление сведений о серьезности, состоянии и контактной информации для запроса в службу поддержки.
- Добавление новой операции взаимодействия к запросу в службу поддержки или получение списка всех операций взаимодействия для запроса в службу поддержки. Вы можете уменьшить область поиска списков операций взаимодействия, отфильтровав их дате создания или типу взаимодействия.

Чтобы создать запрос на поддержку, необходимо быть [владельцем](/azure/role-based-access-control/built-in-roles#owner) или [участником](/azure/role-based-access-control/built-in-roles#contributor) либо быть назначенным роли [Участник запроса на поддержку](/azure/role-based-access-control/built-in-roles#support-request-contributor) на уровне подписки. Для создания запроса в службу поддержки без подписки, например в сценарии Azure Active Directory, необходимо быть [администратором](/azure/active-directory/roles/permissions-reference).

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a>Создание запроса в службу поддержки

1. Чтобы получить список служб, используйте команду [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):

   ```azurecli
   az support services list --output table
   ```

   Для этого примера найдите значение для **виртуальной машины под управлением Windows**. Это должно быть значение **6f16735c-b0ae-b275-ad3a-03479cfa1396**.

1. Чтобы узнать тип и подтип проблемы, которые описывают вашу проблему, выполните команду [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list):

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   Для этого примера найдите сообщение об ошибке **Cannot connect to my VM / I have an issue with my public IP** (Не удается подключиться к виртуальной машине / Возникла проблема с общедоступным IP-адресом). Этот тип имеет значение **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.

1. Создайте запрос в службу поддержки с помощью команды [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create):

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

Инженер службы поддержки свяжется с вами, используя предпочитаемый вами канал связи. Сведения об ожидаемом времени ответа см. на странице [Ограничения поддержки и время ответа на обращение в поддержку](/support/plans/response/).

## <a name="manage-support-tickets"></a>Управление запросами в службу поддержки

Чтобы просмотреть свои запросы в службу поддержки для текущей подписки, выполните команду [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list):

```azurecli
az support tickets list
```

Чтобы просмотреть запросы в службу поддержки для другой подписки, измените текущую подписку с помощью команды [az account set](/cli/azure/account#az_account_set), а затем выполните приведенную выше команду.

Можно также обновить запрос в службу поддержки с помощью команды [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update):

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a>Отправка сообщений о запросе в службу поддержки

Вы не можете удалить запрос в службу поддержки, созданный с помощью Azure CLI. Вместо этого отправьте сообщение, чтобы закрыть этот запрос. Если вам нужно повторно открыть закрытый запрос на поддержку, создайте новое сообщение, после чего запрос будет автоматически открыт повторно.

Чтобы отправить сообщение о своем запросе, выполните команду [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create):

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

Чтобы просмотреть все сообщения для запроса, используйте команду [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):

```azurecli
az support tickets communications list --ticket-name VM012
```

Для этой команды есть параметр `--filters`, который позволяет отфильтровать ответы.

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a>Дальнейшие действия

- [Часто задаваемые вопросы о поддержке Azure](/support/faq/)
- [Понятие серьезности проблемы и ее уровни согласно классификации Azure](/support/plans/response/)
- [Как создать запрос в службу поддержки на портале Azure](/azure/azure-portal/supportability/how-to-create-azure-support-request)
