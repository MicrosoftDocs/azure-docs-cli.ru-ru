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
ms.openlocfilehash: f5fdfba785d849b1fd4f5919870ec9c341bb9c7d
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967815"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="b3f90-103">Управление несколькими подписками Azure</span><span class="sxs-lookup"><span data-stu-id="b3f90-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="b3f90-104">Большинство пользователей Azure обычно используют только одну подписку.</span><span class="sxs-lookup"><span data-stu-id="b3f90-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="b3f90-105">Но если вы работаете в нескольких организациях или если доступ к определенным ресурсам в вашей организации разделен по группам, это значит, что у вас, скорее всего, есть несколько подписок Azure.</span><span class="sxs-lookup"><span data-stu-id="b3f90-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="b3f90-106">Несколькими подписками можно легко управлять с помощью CLI, либо задав глобальную подписку для всех команд, либо выбирая подписку для каждой команды.</span><span class="sxs-lookup"><span data-stu-id="b3f90-106">Multiple subscriptions can be easily managed with the CLI either by setting a global subscription for all commands, or selecting a subscription on a per-command basis.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="b3f90-107">Клиенты, пользователи и подписки</span><span class="sxs-lookup"><span data-stu-id="b3f90-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="b3f90-108">При определении различий между клиентами, пользователями и подписками в Azure может возникнуть путаница.</span><span class="sxs-lookup"><span data-stu-id="b3f90-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="b3f90-109">_Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию.</span><span class="sxs-lookup"><span data-stu-id="b3f90-109">A _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="b3f90-110">Клиент предполагает наличие минимум одной _подписки_ и одного _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="b3f90-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="b3f90-111">Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает.</span><span class="sxs-lookup"><span data-stu-id="b3f90-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="b3f90-112">У всех пользователей есть учетные записи, с помощью которых они входят в Azure, подготавливают и используют ресурсы.</span><span class="sxs-lookup"><span data-stu-id="b3f90-112">Users are those accounts which sign in to Azure to provision and use resources.</span></span>
<span data-ttu-id="b3f90-113">Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure.</span><span class="sxs-lookup"><span data-stu-id="b3f90-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="b3f90-114">Каждый ресурс связан с подпиской.</span><span class="sxs-lookup"><span data-stu-id="b3f90-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="b3f90-115">Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="b3f90-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="b3f90-116">Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Как добавить подписку Azure в Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="b3f90-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="b3f90-117">При работе с несколькими клиентами вам может понадобиться войти в какой-то определенный клиент.</span><span class="sxs-lookup"><span data-stu-id="b3f90-117">When working with multiple tenants, you may need to sign in to a specific tenant.</span></span> <span data-ttu-id="b3f90-118">Сведения о том, как это сделать, см. в статье о [входе с помощью Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="b3f90-118">To do this, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="work-with-multiple-subscriptions"></a><span data-ttu-id="b3f90-119">Использование нескольких подписок</span><span class="sxs-lookup"><span data-stu-id="b3f90-119">Work with multiple subscriptions</span></span>

<span data-ttu-id="b3f90-120">Чтобы получить доступ к ресурсам, содержащимся в другой подписке, необходимо переключиться на нее с активной подписки.</span><span class="sxs-lookup"><span data-stu-id="b3f90-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="b3f90-121">Переключить подписку можно для всех команд Azure CLI с помощью команды [az account set](/cli/azure/account#az-account-set) либо же для каждой команды в отдельности с помощью аргумента `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="b3f90-121">Switching your subscription can be done for all Azure CLI commands with [az account set](/cli/azure/account#az-account-set), or done on a per-command basis by using the `--subscription` argument.</span></span>

<span data-ttu-id="b3f90-122">Для начала вам потребуется список доступных подписок.</span><span class="sxs-lookup"><span data-stu-id="b3f90-122">To start, you will need a list of your available subscriptions.</span></span> <span data-ttu-id="b3f90-123">Чтобы получить его, используйте команду [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="b3f90-123">To get it, use the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli-interactive
az account list --output table
```

<span data-ttu-id="b3f90-124">Чтобы изменить активную подписку для всех команд, используйте `az account set` вместе с идентификатором или именем подписки:</span><span class="sxs-lookup"><span data-stu-id="b3f90-124">To change the active subscription globally, use `az account set` along with either the subscription ID or subscription name:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="b3f90-125">Чтобы указать определенную подписку для команды, просто используйте аргумент `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="b3f90-125">To use a specific subscription for a command, just use the `--subscription` argument.</span></span> <span data-ttu-id="b3f90-126">Этот аргумент принимает идентификатор или имя подписки:</span><span class="sxs-lookup"><span data-stu-id="b3f90-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
