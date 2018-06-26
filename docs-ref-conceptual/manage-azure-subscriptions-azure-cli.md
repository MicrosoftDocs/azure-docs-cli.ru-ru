---
title: Управление подписками Azure с помощью Azure CLI
description: Управление подписками Azure с помощью Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: fdc8ffca38a6a581ae63b0518df72f6e09110d07
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262715"
---
# <a name="manage-multiple-azure-subscriptions"></a>Управление несколькими подписками Azure

Большинство пользователей Azure обычно используют только одну подписку. Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, это значит, что у вас, скорее всего, есть несколько подписок Azure. Несколькими подписками можно легко управлять с помощью CLI, либо задав глобальную подписку для всех команд, либо выбирая подписку для каждой команды.

## <a name="tenants-users-and-subscriptions"></a>Клиенты, пользователи и подписки

При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница. _Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию. Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_. Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает. У всех пользователей есть учетные записи, с помощью которых они входят в Azure, подготавливают и используют ресурсы.
Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure. Каждый ресурс связан с подпиской.

Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).  Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
При работе с несколькими клиентами вам может понадобиться войти в какой-то определенный клиент. Сведения о том, как это сделать, см. в статье о [входе с помощью Azure CLI](/cli/azure/authenticate-azure-cli).

## <a name="work-with-multiple-subscriptions"></a>Использование нескольких подписок

Чтобы получить доступ к ресурсам, содержащимся в другой подписке, необходимо переключиться на нее с активной подписки. Переключить подписку можно для всех команд Azure CLI с помощью команды [az account set](/cli/azure/account#az-account-set) либо же для каждой команды в отдельности с помощью аргумента `--subscription`.

Для начала вам потребуется список доступных подписок. Чтобы получить его, используйте команду [az account list](/cli/azure/account#az-account-list):

```azurecli-interactive
az account list --output table
```

Чтобы изменить активную подписку для всех команд, используйте `az account set` вместе с идентификатором или именем подписки:

```azurecli-interactive
az account set --subscription "My Demos"
```

Чтобы указать определенную подписку для команды, просто используйте аргумент `--subscription`. Этот аргумент принимает идентификатор или имя подписки:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
