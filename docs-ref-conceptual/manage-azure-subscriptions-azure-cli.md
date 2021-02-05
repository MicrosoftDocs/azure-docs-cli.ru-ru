---
title: Управление подписками Azure с помощью Azure CLI
description: Сведения о клиентах, пользователях и подписках Azure. Управляйте подписками, блокируйте их и создавайте группы управления с помощью Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6a980c45627c79c9e3f8c6c920944cc3dc62281f
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "99495233"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a><span data-ttu-id="cbeef-104">Работа с подписками Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cbeef-104">Use Azure subscriptions with Azure CLI</span></span>

<span data-ttu-id="cbeef-105">В Azure у вас может быть несколько подписок.</span><span class="sxs-lookup"><span data-stu-id="cbeef-105">You might have multiple subscriptions within Azure.</span></span> <span data-ttu-id="cbeef-106">Вы можете работать с несколькими организациями, или в вашей организации доступ к определенным ресурсам может быть разделен между группами.</span><span class="sxs-lookup"><span data-stu-id="cbeef-106">You can be part of more than one organization or your organization might divide access to certain resources across groupings.</span></span> <span data-ttu-id="cbeef-107">Azure CLI поддерживает выбор подписки как глобально, так и для отдельных команд.</span><span class="sxs-lookup"><span data-stu-id="cbeef-107">The Azure CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="cbeef-108">См. подробнее о [подписках, выставлении счетов и управлении затратами](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="cbeef-108">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="cbeef-109">Клиенты, пользователи и подписки</span><span class="sxs-lookup"><span data-stu-id="cbeef-109">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="cbeef-110">_Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию.</span><span class="sxs-lookup"><span data-stu-id="cbeef-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="cbeef-111">В клиенте одна или более _подписок_ и один или более _пользователей_.</span><span class="sxs-lookup"><span data-stu-id="cbeef-111">A tenant has one or more _subscription_ and _user_.</span></span> <span data-ttu-id="cbeef-112">Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает.</span><span class="sxs-lookup"><span data-stu-id="cbeef-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="cbeef-113">Пользователи — это учетные записи для входа в Azure, которые используются, чтобы создавать, использовать и администрировать ресурсы.</span><span class="sxs-lookup"><span data-stu-id="cbeef-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span> <span data-ttu-id="cbeef-114">Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure.</span><span class="sxs-lookup"><span data-stu-id="cbeef-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="cbeef-115">Каждый ресурс связан с подпиской.</span><span class="sxs-lookup"><span data-stu-id="cbeef-115">Every resource is associated with a subscription.</span></span>

* <span data-ttu-id="cbeef-116">Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="cbeef-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
* <span data-ttu-id="cbeef-117">Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Связывание или добавление подписки Azure в клиент Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="cbeef-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
* <span data-ttu-id="cbeef-118">Сведения о том, как выполнить вход от имени определенного клиента, см. в статье [Вход с помощью Azure CLI](./authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="cbeef-118">To learn how to sign in to a specific tenant, see [Sign in with the Azure CLI](./authenticate-azure-cli.md).</span></span>

## <a name="commands-in-a-subscription"></a><span data-ttu-id="cbeef-119">Работа с командами в подписке</span><span class="sxs-lookup"><span data-stu-id="cbeef-119">Commands in a subscription</span></span>

<span data-ttu-id="cbeef-120">Многие команды Azure CLI работают в рамках подписки.</span><span class="sxs-lookup"><span data-stu-id="cbeef-120">Many Azure CLI commands act within a subscription.</span></span> <span data-ttu-id="cbeef-121">Вы всегда можете указать, в какой подписке будете работать, используя параметр **subscription** в команде.</span><span class="sxs-lookup"><span data-stu-id="cbeef-121">You can always specify which subscription to work in by using the **subscription** parameter in your command.</span></span> <span data-ttu-id="cbeef-122">Это необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cbeef-122">That parameter is optional.</span></span> <span data-ttu-id="cbeef-123">Если подписка не указана, в команде используется текущая активная подписка.</span><span class="sxs-lookup"><span data-stu-id="cbeef-123">If you don't specify a subscription, the command uses your current, active subscription.</span></span>

<span data-ttu-id="cbeef-124">Чтобы просмотреть текущую подписку, выполните команду [az account show](/cli/azure/account#az_account_show):</span><span class="sxs-lookup"><span data-stu-id="cbeef-124">To see the subscription you're currently using, run the [az account show](/cli/azure/account#az_account_show) command:</span></span>

```azurecli
az account show --output table
```

> [!TIP]
> <span data-ttu-id="cbeef-125">Параметр `--output` является глобальным, то есть доступным для всех команд.</span><span class="sxs-lookup"><span data-stu-id="cbeef-125">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="cbeef-126">Значение **table** позволяет получить выходные данные в удобном формате.</span><span class="sxs-lookup"><span data-stu-id="cbeef-126">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="cbeef-127">Дополнительные сведения см. в статье [Форматы выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="cbeef-127">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="cbeef-128">Подписки содержат группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cbeef-128">Subscriptions contain resource groups.</span></span> <span data-ttu-id="cbeef-129">Группа ресурсов Azure — это контейнер, содержащий связанные ресурсы для решения Azure.</span><span class="sxs-lookup"><span data-stu-id="cbeef-129">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="cbeef-130">Если команда работает с ресурсами в активной подписке, `--subscription` указывать не нужно.</span><span class="sxs-lookup"><span data-stu-id="cbeef-130">If your command works with resources in your active subscription, you don't need to specify `--subscription`.</span></span>

<span data-ttu-id="cbeef-131">Эта команда позволяет создать учетную запись хранения в указанной группе ресурсов:</span><span class="sxs-lookup"><span data-stu-id="cbeef-131">This command creates a storage account in the specified resource group:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

<span data-ttu-id="cbeef-132">Если группа хранения не входит в вашу текущую активную подписку, эта команда завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cbeef-132">If the storage group isn't part of your current active subscription, this command fails.</span></span>

<span data-ttu-id="cbeef-133">При необходимости измените активную подписку, как описано в следующем разделе, или укажите подписку в команде:</span><span class="sxs-lookup"><span data-stu-id="cbeef-133">If necessary, change the active subscription, as described in the next section, or specify the subscription in the command:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a><span data-ttu-id="cbeef-134">Изменение активной подписки</span><span class="sxs-lookup"><span data-stu-id="cbeef-134">Change the active subscription</span></span>

<span data-ttu-id="cbeef-135">Вы можете изменить активную подписку с помощью команды [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="cbeef-135">You can change your active subscription by using the [az account set](/cli/azure/account#az-account-set) command.</span></span>

<span data-ttu-id="cbeef-136">Получите список своих подписок с помощью команды [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="cbeef-136">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli
az account list --output table
```

<span data-ttu-id="cbeef-137">Эта команда позволяет вывести список всех подписок, к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="cbeef-137">This command lists all the subscriptions you can access.</span></span> <span data-ttu-id="cbeef-138">Активная подписка помечается как `True` в столбце `IsDefault`.</span><span class="sxs-lookup"><span data-stu-id="cbeef-138">Your active subscription is marked as `True` in the `IsDefault` column.</span></span> <span data-ttu-id="cbeef-139">Если ожидаемая подписка не отображается, добавьте параметр `--refresh`, чтобы получить актуальный список подписок.</span><span class="sxs-lookup"><span data-stu-id="cbeef-139">If you don't see a subscription you expect, add the `--refresh` parameter to get the most current list of subscriptions.</span></span>

<span data-ttu-id="cbeef-140">Чтобы переключиться на другую подписку, используйте [az account set](/cli/azure/account#az-account-set) с идентификатором подписки или именем, на которое вам нужно переключиться.</span><span class="sxs-lookup"><span data-stu-id="cbeef-140">To switch to a different subscription, use [az account set](/cli/azure/account#az-account-set) with the subscription ID or name you want to switch to.</span></span>

```azurecli
az account set --subscription "My Demos"
```

<span data-ttu-id="cbeef-141">У ваших подписок есть и имя, и идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="cbeef-141">Your subscriptions have both a name and an ID, which is a GUID.</span></span> <span data-ttu-id="cbeef-142">Для этих команд можно использовать любое из этих значений.</span><span class="sxs-lookup"><span data-stu-id="cbeef-142">You can use either for these commands.</span></span> <span data-ttu-id="cbeef-143">Если в имени есть пробелы, используйте кавычки.</span><span class="sxs-lookup"><span data-stu-id="cbeef-143">If you use a name that includes spaces, use quotation marks.</span></span>

<span data-ttu-id="cbeef-144">При повторном выполнении команды [az account list](/cli/azure/account#az-account-list) в столбце `IsDefault` отображается текущая активная подписка.</span><span class="sxs-lookup"><span data-stu-id="cbeef-144">If you run the [az account list](/cli/azure/account#az-account-list) command again, the `IsDefault` column shows your current active subscription.</span></span>

## <a name="create-management-groups"></a><span data-ttu-id="cbeef-145">Создание групп управления</span><span class="sxs-lookup"><span data-stu-id="cbeef-145">Create management groups</span></span>

<span data-ttu-id="cbeef-146">Группы управления Azure содержат подписки.</span><span class="sxs-lookup"><span data-stu-id="cbeef-146">Azure management groups contain subscriptions.</span></span> <span data-ttu-id="cbeef-147">Группы управления предоставляют возможность управления доступом, политиками и соответствием для этих подписок.</span><span class="sxs-lookup"><span data-stu-id="cbeef-147">Management groups provide a way to manage access, policies, and compliance for those subscriptions.</span></span> <span data-ttu-id="cbeef-148">Дополнительные сведения см. в статье [Что такое группы управления Azure?](/azure/governance/management-groups/overview)</span><span class="sxs-lookup"><span data-stu-id="cbeef-148">For more information, see [What are Azure management groups](/azure/governance/management-groups/overview).</span></span>

<span data-ttu-id="cbeef-149">Создавать и администрировать группы управления Azure можно с помощью команд [az account management-group](/cli/azure/account/management-group).</span><span class="sxs-lookup"><span data-stu-id="cbeef-149">Use the [az account management-group](/cli/azure/account/management-group) commands to create and manage Azure Management Groups.</span></span>

<span data-ttu-id="cbeef-150">Группу управления для нескольких подписок можно создать с помощью команды [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create):</span><span class="sxs-lookup"><span data-stu-id="cbeef-150">You can create a management group for several of your subscriptions by using the [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) command:</span></span>

```azurecli
az account management-group create --name Contoso01
```

<span data-ttu-id="cbeef-151">Чтобы просмотреть все группы управления, воспользуйтесь командой [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):</span><span class="sxs-lookup"><span data-stu-id="cbeef-151">To see all your management groups, use the [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) command:</span></span>

```azurecli
az account management-group list
```

<span data-ttu-id="cbeef-152">Добавьте подписки в новую группу с помощью команды [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add):</span><span class="sxs-lookup"><span data-stu-id="cbeef-152">Add subscriptions to your new group by using the [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) command:</span></span>

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

<span data-ttu-id="cbeef-153">Чтобы удалить подписку, используйте команду [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):</span><span class="sxs-lookup"><span data-stu-id="cbeef-153">To remove a subscription, use the [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) command:</span></span>

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

<span data-ttu-id="cbeef-154">Чтобы удалить группу управления, выполните команду [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete):</span><span class="sxs-lookup"><span data-stu-id="cbeef-154">To remove a management group, run the [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) command:</span></span>

```azurecli
az account management-group delete --name Contoso01
```

<span data-ttu-id="cbeef-155">При удалении подписки или группы управления подписка не удаляется без возможности восстановления и не деактивируется.</span><span class="sxs-lookup"><span data-stu-id="cbeef-155">Removing a subscription or deleting a management group doesn't delete or deactivate a subscription.</span></span>

## <a name="set-a-subscription-lock"></a><span data-ttu-id="cbeef-156">Настройка блокировки подписки</span><span class="sxs-lookup"><span data-stu-id="cbeef-156">Set a subscription lock</span></span>

<span data-ttu-id="cbeef-157">Администратору может потребоваться заблокировать подписку, чтобы запретить пользователям удалять или изменять ее.</span><span class="sxs-lookup"><span data-stu-id="cbeef-157">As an administrator, you may need to lock a subscription to prevent users from deleting or modifying it.</span></span> <span data-ttu-id="cbeef-158">Дополнительные сведения см. в статье [Блокировка ресурсов для предотвращения непредвиденных изменений](/azure/azure-resource-manager/management/lock-resources).</span><span class="sxs-lookup"><span data-stu-id="cbeef-158">For more information, see [Lock resources to prevent unexpected changes](/azure/azure-resource-manager/management/lock-resources).</span></span>

<span data-ttu-id="cbeef-159">В Azure CLI используйте команды [az account lock](/cli/azure/account/lock).</span><span class="sxs-lookup"><span data-stu-id="cbeef-159">In Azure CLI, use the [az account lock](/cli/azure/account/lock) commands.</span></span> <span data-ttu-id="cbeef-160">Например, с помощью команды [az account lock create](/cli/azure/account/lock#az_account_lock_create) можно запретить удаление подписки пользователями:</span><span class="sxs-lookup"><span data-stu-id="cbeef-160">For instance, the [az account lock create](/cli/azure/account/lock#az_account_lock_create) command can prevent users from deleting a subscription:</span></span>

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> <span data-ttu-id="cbeef-161">Для создания или изменения блокировок нужны соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="cbeef-161">You need to have appropriate permissions to create or change locks.</span></span>

<span data-ttu-id="cbeef-162">Чтобы просмотреть текущие блокировки в подписке, воспользуйтесь командой [az account lock list](/cli/azure/account/lock#az_account_lock_list):</span><span class="sxs-lookup"><span data-stu-id="cbeef-162">To see the current locks on your subscription, use the [az account lock list](/cli/azure/account/lock#az_account_lock_list) command:</span></span>

```azurecli
az account lock list --output table
```

<span data-ttu-id="cbeef-163">Если сделать учетную запись доступной только для чтения, результат будет подобен назначению разрешений роли читателя всем пользователям.</span><span class="sxs-lookup"><span data-stu-id="cbeef-163">If you make an account read-only, the result resembles assigning permissions of the Reader role to all users.</span></span> <span data-ttu-id="cbeef-164">Дополнительные сведения о настройке разрешений для отдельных пользователей и ролей см. в статье [Добавление и удаление назначений ролей Azure с помощью Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span><span class="sxs-lookup"><span data-stu-id="cbeef-164">To learn about setting permissions for individual users and roles, see [Add or remove Azure role assignments using Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span></span>

<span data-ttu-id="cbeef-165">Чтобы просмотреть сведения о блокировке, воспользуйтесь командой [az account lock show](/cli/azure/account/lock#az_account_lock_show):</span><span class="sxs-lookup"><span data-stu-id="cbeef-165">To see details for a lock, use the [az account lock show](/cli/azure/account/lock#az_account_lock_show) command:</span></span>

```azurecli
az account lock show --name "Cannot delete subscription"
```

<span data-ttu-id="cbeef-166">Снять блокировку можно с помощью команды [az account lock delete](/cli/azure/account/lock#az_account_lock_delete):</span><span class="sxs-lookup"><span data-stu-id="cbeef-166">You can remove a lock by using the [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) command:</span></span>

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a><span data-ttu-id="cbeef-167">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="cbeef-167">See also</span></span>

* [<span data-ttu-id="cbeef-168">Словарь терминов Azure, связанных с облаком</span><span class="sxs-lookup"><span data-stu-id="cbeef-168">Azure cloud terminology dictionary</span></span>](/azure/azure-glossary-cloud-terminology)
* <span data-ttu-id="cbeef-169">[Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory) (Связывание или добавление подписки Azure в клиент Azure Active Directory)</span><span class="sxs-lookup"><span data-stu-id="cbeef-169">[Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory)</span></span>
* [<span data-ttu-id="cbeef-170">Вход с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cbeef-170">Sign in with Azure CLI</span></span>](./authenticate-azure-cli.md)
