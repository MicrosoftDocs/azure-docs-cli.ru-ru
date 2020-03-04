---
title: Управление подписками Azure с помощью Azure CLI
description: Управление подписками Azure с помощью Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: dad217dff159baa39bd1361258fb308eea872564
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "77780066"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="d01f2-103">Использование нескольких подписок Azure</span><span class="sxs-lookup"><span data-stu-id="d01f2-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="d01f2-104">Большинство пользователей Azure обычно используют только одну подписку.</span><span class="sxs-lookup"><span data-stu-id="d01f2-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="d01f2-105">Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, у вас может быть несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="d01f2-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="d01f2-106">CLI поддерживает выбор подписки как глобально, так и для отдельных команд.</span><span class="sxs-lookup"><span data-stu-id="d01f2-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="d01f2-107">См. подробнее о [подписках, выставлении счетов и управлении затратами](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="d01f2-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="d01f2-108">Клиенты, пользователи и подписки</span><span class="sxs-lookup"><span data-stu-id="d01f2-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="d01f2-109">При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница.</span><span class="sxs-lookup"><span data-stu-id="d01f2-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="d01f2-110">_Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию.</span><span class="sxs-lookup"><span data-stu-id="d01f2-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="d01f2-111">Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="d01f2-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="d01f2-112">Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает.</span><span class="sxs-lookup"><span data-stu-id="d01f2-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="d01f2-113">Пользователи — это учетные записи для входа в Azure, которые используются, чтобы создавать, использовать и администрировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="d01f2-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="d01f2-114">Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure.</span><span class="sxs-lookup"><span data-stu-id="d01f2-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="d01f2-115">Каждый ресурс связан с подпиской.</span><span class="sxs-lookup"><span data-stu-id="d01f2-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="d01f2-116">Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="d01f2-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="d01f2-117">Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="d01f2-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="d01f2-118">Сведения о том, как выполнить вход от имени определенного клиента см. в статье [Вход с помощью Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="d01f2-118">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="d01f2-119">Изменение активной подписки</span><span class="sxs-lookup"><span data-stu-id="d01f2-119">Change the active subscription</span></span>

<span data-ttu-id="d01f2-120">Для доступа к ресурсам определенной подписки измените активную подписку или используйте аргумент `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="d01f2-120">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="d01f2-121">Изменение подписки для всех команд выполняется с помощью команды [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="d01f2-121">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="d01f2-122">Чтобы изменить активную подписку:</span><span class="sxs-lookup"><span data-stu-id="d01f2-122">To switch your active subscription:</span></span>

1. <span data-ttu-id="d01f2-123">Получите список своих подписок с помощью команды [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="d01f2-123">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="d01f2-124">Выполните команду `az account set`, указав идентификатор подписки или имя, на которое нужно переключиться.</span><span class="sxs-lookup"><span data-stu-id="d01f2-124">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="d01f2-125">Для выполнения только одной команды с другой подпиской, используйте аргумент `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="d01f2-125">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="d01f2-126">Этот аргумент принимает идентификатор или имя подписки:</span><span class="sxs-lookup"><span data-stu-id="d01f2-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
