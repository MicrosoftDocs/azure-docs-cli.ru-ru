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
# <a name="use-azure-subscriptions-with-azure-cli"></a>Работа с подписками Azure с помощью Azure CLI

В Azure у вас может быть несколько подписок. Вы можете работать с несколькими организациями, или в вашей организации доступ к определенным ресурсам может быть разделен между группами. Azure CLI поддерживает выбор подписки как глобально, так и для отдельных команд.

См. подробнее о [подписках, выставлении счетов и управлении затратами](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Клиенты, пользователи и подписки

_Клиент_ — это сущность Azure Active Directory, которая условно представляет всю организацию. В клиенте одна или более _подписок_ и один или более _пользователей_. Пользователь — это человек, который связан только с одним клиентом — организацией, в которой он работает. Пользователи — это учетные записи для входа в Azure, которые используются, чтобы создавать, использовать и администрировать ресурсы. Пользователь может иметь доступ к нескольким _подпискам_. Подписки — это соглашения с корпорацией Майкрософт на использование облачных служб, в том числе Azure. Каждый ресурс связан с подпиской.

* Дополнительные сведения о различиях между клиентами, пользователями и подписками см. в [словаре терминов, связанных с облачной платформой Azure](/azure/azure-glossary-cloud-terminology).
* Чтобы узнать, как добавить новую подписку в клиент Azure Active Directory, см. статью [Связывание или добавление подписки Azure в клиент Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
* Сведения о том, как выполнить вход от имени определенного клиента, см. в статье [Вход с помощью Azure CLI](./authenticate-azure-cli.md).

## <a name="commands-in-a-subscription"></a>Работа с командами в подписке

Многие команды Azure CLI работают в рамках подписки. Вы всегда можете указать, в какой подписке будете работать, используя параметр **subscription** в команде. Это необязательный параметр. Если подписка не указана, в команде используется текущая активная подписка.

Чтобы просмотреть текущую подписку, выполните команду [az account show](/cli/azure/account#az_account_show):

```azurecli
az account show --output table
```

> [!TIP]
> Параметр `--output` является глобальным, то есть доступным для всех команд. Значение **table** позволяет получить выходные данные в удобном формате. Дополнительные сведения см. в статье [Форматы выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).

Подписки содержат группы ресурсов. Группа ресурсов Azure — это контейнер, содержащий связанные ресурсы для решения Azure. Если команда работает с ресурсами в активной подписке, `--subscription` указывать не нужно.

Эта команда позволяет создать учетную запись хранения в указанной группе ресурсов:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

Если группа хранения не входит в вашу текущую активную подписку, эта команда завершится с ошибкой.

При необходимости измените активную подписку, как описано в следующем разделе, или укажите подписку в команде:

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a>Изменение активной подписки

Вы можете изменить активную подписку с помощью команды [az account set](/cli/azure/account#az-account-set).

Получите список своих подписок с помощью команды [az account list](/cli/azure/account#az-account-list):

```azurecli
az account list --output table
```

Эта команда позволяет вывести список всех подписок, к которым у вас есть доступ. Активная подписка помечается как `True` в столбце `IsDefault`. Если ожидаемая подписка не отображается, добавьте параметр `--refresh`, чтобы получить актуальный список подписок.

Чтобы переключиться на другую подписку, используйте [az account set](/cli/azure/account#az-account-set) с идентификатором подписки или именем, на которое вам нужно переключиться.

```azurecli
az account set --subscription "My Demos"
```

У ваших подписок есть и имя, и идентификатор (GUID). Для этих команд можно использовать любое из этих значений. Если в имени есть пробелы, используйте кавычки.

При повторном выполнении команды [az account list](/cli/azure/account#az-account-list) в столбце `IsDefault` отображается текущая активная подписка.

## <a name="create-management-groups"></a>Создание групп управления

Группы управления Azure содержат подписки. Группы управления предоставляют возможность управления доступом, политиками и соответствием для этих подписок. Дополнительные сведения см. в статье [Что такое группы управления Azure?](/azure/governance/management-groups/overview)

Создавать и администрировать группы управления Azure можно с помощью команд [az account management-group](/cli/azure/account/management-group).

Группу управления для нескольких подписок можно создать с помощью команды [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create):

```azurecli
az account management-group create --name Contoso01
```

Чтобы просмотреть все группы управления, воспользуйтесь командой [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):

```azurecli
az account management-group list
```

Добавьте подписки в новую группу с помощью команды [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add):

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

Чтобы удалить подписку, используйте команду [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

Чтобы удалить группу управления, выполните команду [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete):

```azurecli
az account management-group delete --name Contoso01
```

При удалении подписки или группы управления подписка не удаляется без возможности восстановления и не деактивируется.

## <a name="set-a-subscription-lock"></a>Настройка блокировки подписки

Администратору может потребоваться заблокировать подписку, чтобы запретить пользователям удалять или изменять ее. Дополнительные сведения см. в статье [Блокировка ресурсов для предотвращения непредвиденных изменений](/azure/azure-resource-manager/management/lock-resources).

В Azure CLI используйте команды [az account lock](/cli/azure/account/lock). Например, с помощью команды [az account lock create](/cli/azure/account/lock#az_account_lock_create) можно запретить удаление подписки пользователями:

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> Для создания или изменения блокировок нужны соответствующие разрешения.

Чтобы просмотреть текущие блокировки в подписке, воспользуйтесь командой [az account lock list](/cli/azure/account/lock#az_account_lock_list):

```azurecli
az account lock list --output table
```

Если сделать учетную запись доступной только для чтения, результат будет подобен назначению разрешений роли читателя всем пользователям. Дополнительные сведения о настройке разрешений для отдельных пользователей и ролей см. в статье [Добавление и удаление назначений ролей Azure с помощью Azure CLI](/azure/role-based-access-control/role-assignments-cli).

Чтобы просмотреть сведения о блокировке, воспользуйтесь командой [az account lock show](/cli/azure/account/lock#az_account_lock_show):

```azurecli
az account lock show --name "Cannot delete subscription"
```

Снять блокировку можно с помощью команды [az account lock delete](/cli/azure/account/lock#az_account_lock_delete):

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a>См. также раздел

* [Словарь терминов Azure, связанных с облаком](/azure/azure-glossary-cloud-terminology)
* [Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory) (Связывание или добавление подписки Azure в клиент Azure Active Directory)
* [Вход с помощью Azure CLI](./authenticate-azure-cli.md)
