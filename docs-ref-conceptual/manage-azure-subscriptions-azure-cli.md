---
title: "Manage Azure subscriptions with Azure CLI 2.0 (Управление подписками Azure с помощью Azure CLI 2.0)"
description: "Manage Azure subscriptions with Azure CLI 2.0 on Linux, Mac, or Windows (Управление подписками Azure с помощью Azure CLI 2.0 на платформах Windows, Mac или Linux)."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b0c0b3f5e4d9bc651ad4781cb0906dc98d8531a3
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2018
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="3ac03-103">Управление несколькими подписками Azure</span><span class="sxs-lookup"><span data-stu-id="3ac03-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="3ac03-104">Большинство пользователей Azure обычно используют только одну подписку.</span><span class="sxs-lookup"><span data-stu-id="3ac03-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="3ac03-105">Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, это значит, что у вас, скорее всего, есть несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="3ac03-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="3ac03-106">Для управления несколькими подписками можно использовать CLI, а для выполнения операций достаточно выбрать нужную подписку.</span><span class="sxs-lookup"><span data-stu-id="3ac03-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="3ac03-107">Клиенты, пользователи и подписки</span><span class="sxs-lookup"><span data-stu-id="3ac03-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="3ac03-108">При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница.</span><span class="sxs-lookup"><span data-stu-id="3ac03-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="3ac03-109">В общих чертах, _клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию.</span><span class="sxs-lookup"><span data-stu-id="3ac03-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="3ac03-110">Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="3ac03-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="3ac03-111">Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает.</span><span class="sxs-lookup"><span data-stu-id="3ac03-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="3ac03-112">У всех пользователей есть учетные записи, с помощью которых они входят в Azure, подготавливают и используют ресурсы.</span><span class="sxs-lookup"><span data-stu-id="3ac03-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="3ac03-113">Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure.</span><span class="sxs-lookup"><span data-stu-id="3ac03-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="3ac03-114">Каждый ресурс связан с подпиской.</span><span class="sxs-lookup"><span data-stu-id="3ac03-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="3ac03-115">Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="3ac03-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="3ac03-116">Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="3ac03-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="3ac03-117">При работе с несколькими клиентами вам может понадобиться войти в какой-то определенный клиент.</span><span class="sxs-lookup"><span data-stu-id="3ac03-117">When working with multiple tenants, you may need to log into a specific tenant.</span></span> <span data-ttu-id="3ac03-118">Сведения о том, как это сделать, см. в статье [Вход с помощью Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="3ac03-118">To do this, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="3ac03-119">Использование нескольких подписок</span><span class="sxs-lookup"><span data-stu-id="3ac03-119">Working with multiple subscriptions</span></span>

<span data-ttu-id="3ac03-120">Чтобы получить доступ к ресурсам, содержащимся в другой подписке, необходимо переключиться на нее с активной подписки.</span><span class="sxs-lookup"><span data-stu-id="3ac03-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="3ac03-121">Все операции с подписками выполняются с помощью команды `az account`. Эта команда связана с соглашением об обслуживании, которое представляет подписка, а не с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ac03-121">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="3ac03-122">Чтобы начать работу с подписками, отобразите список доступных подписок в вашей учетной записи:</span><span class="sxs-lookup"><span data-stu-id="3ac03-122">To start working with your available subscriptions, get a list of those available in your account:</span></span>

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

<span data-ttu-id="3ac03-123">Чтобы сменить активную подписку, можно использовать команду `az account set`:</span><span class="sxs-lookup"><span data-stu-id="3ac03-123">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="3ac03-124">Для выбора подписки можно указать имя или идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="3ac03-124">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
