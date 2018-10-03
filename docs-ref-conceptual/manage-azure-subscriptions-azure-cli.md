---
title: Управление подписками Azure с помощью Azure CLI
description: Управление подписками Azure с помощью Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7bffd91fc31452fc745bc572262f10645e4179eb
ms.sourcegitcommit: f7554c00b5d5dca0ec716cbf996eb6654183ec37
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2018
ms.locfileid: "47237601"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="3cd51-103">Использование нескольких подписок Azure</span><span class="sxs-lookup"><span data-stu-id="3cd51-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="3cd51-104">Большинство пользователей Azure обычно используют только одну подписку.</span><span class="sxs-lookup"><span data-stu-id="3cd51-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="3cd51-105">Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, у вас может быть несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="3cd51-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="3cd51-106">CLI поддерживает выбор подписки как глобально, так и для отдельных команд.</span><span class="sxs-lookup"><span data-stu-id="3cd51-106">The CLI supports selecting a subscription both globally and per command.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="3cd51-107">Клиенты, пользователи и подписки</span><span class="sxs-lookup"><span data-stu-id="3cd51-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="3cd51-108">При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница.</span><span class="sxs-lookup"><span data-stu-id="3cd51-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="3cd51-109">_Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию.</span><span class="sxs-lookup"><span data-stu-id="3cd51-109">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="3cd51-110">Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="3cd51-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="3cd51-111">Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает.</span><span class="sxs-lookup"><span data-stu-id="3cd51-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="3cd51-112">Пользователи — это учетные записи для входа в Azure, которые используются, чтобы создавать, использовать и администрировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="3cd51-112">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="3cd51-113">Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure.</span><span class="sxs-lookup"><span data-stu-id="3cd51-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="3cd51-114">Каждый ресурс связан с подпиской.</span><span class="sxs-lookup"><span data-stu-id="3cd51-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="3cd51-115">Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="3cd51-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="3cd51-116">Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="3cd51-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="3cd51-117">Сведения о том, как выполнить вход от имени определенного клиента см. в статье [Вход с помощью Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="3cd51-117">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="3cd51-118">Изменение активной подписки</span><span class="sxs-lookup"><span data-stu-id="3cd51-118">Change the active subscription</span></span> 

<span data-ttu-id="3cd51-119">Для доступа к ресурсам определенной подписки измените активную подписку или используйте аргумент `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="3cd51-119">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="3cd51-120">Изменение подписки для всех команд выполняется с помощью команды [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="3cd51-120">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="3cd51-121">Чтобы изменить активную подписку:</span><span class="sxs-lookup"><span data-stu-id="3cd51-121">To switch your active subscription:</span></span>

1. <span data-ttu-id="3cd51-122">Получите список своих подписок с помощью команды [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="3cd51-122">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="3cd51-123">Выполните команду `az account set`, указав идентификатор подписки или имя, на которое нужно переключиться.</span><span class="sxs-lookup"><span data-stu-id="3cd51-123">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="3cd51-124">Для выполнения только одной команды с другой подпиской, используйте аргумент `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="3cd51-124">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="3cd51-125">Этот аргумент принимает идентификатор или имя подписки:</span><span class="sxs-lookup"><span data-stu-id="3cd51-125">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
