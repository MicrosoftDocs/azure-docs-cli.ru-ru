---
title: Manage Azure subscriptions with Azure CLI 2.0 (Управление подписками Azure с помощью Azure CLI 2.0)
description: Manage Azure subscriptions with Azure CLI 2.0 on Linux, Mac, or Windows (Управление подписками Azure с помощью Azure CLI 2.0 на платформах Windows, Mac или Linux).
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: 5a27eed40e0666f6a5e57a23ac369d92c3b01dab
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703032"
---
# <a name="manage-multiple-azure-subscriptions"></a>Управление несколькими подписками Azure

Большинство пользователей Azure обычно используют только одну подписку. Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, это значит, что у вас, скорее всего, есть несколько подписок Azure. Для управления несколькими подписками можно использовать CLI, а для выполнения операций достаточно выбрать нужную подписку.

## <a name="tenants-users-and-subscriptions"></a>Клиенты, пользователи и подписки

При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница. В общих чертах, _клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию. Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_. Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает. У всех пользователей есть учетные записи, с помощью которых они входят в Azure, подготавливают и используют ресурсы. Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure. Каждый ресурс связан с подпиской.

Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).
Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
При работе с несколькими клиентами вам может понадобиться войти в какой-то определенный клиент. Сведения о том, как это сделать, см. в статье [Вход с помощью Azure CLI 2.0](/cli/azure/authenticate-azure-cli).

## <a name="working-with-multiple-subscriptions"></a>Использование нескольких подписок

Чтобы получить доступ к ресурсам, содержащимся в другой подписке, необходимо переключиться на нее с активной подписки. Все операции с подписками выполняются с помощью команды `az account`. Эта команда связана с соглашением об обслуживании, которое представляет подписка, а не с учетной записью пользователя.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

Чтобы начать работу с подписками, отобразите список доступных подписок в вашей учетной записи:

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

Чтобы сменить активную подписку, можно использовать команду `az account set`:

```azurecli-interactive
az account set --subscription "My Demos"
```

Для выбора подписки можно указать имя или идентификатор подписки.
