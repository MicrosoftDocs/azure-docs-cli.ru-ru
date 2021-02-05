---
title: Управление группами ресурсов Azure с помощью Azure CLI
description: Сведения о группах ресурсов Azure и управлении ими с помощью Azure CLI. Сведения о сохраненных группах ресурсов и группах ресурсов по умолчанию.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496080"
---
# <a name="working-with-resource-groups-in-azure-cli"></a>Работа с группами ресурсов Azure в Azure CLI

Группа ресурсов Azure — это контейнер, содержащий связанные ресурсы для решения Azure. Группа ресурсов может содержать хранилище, виртуальные машины, приложения, панели мониторинга, службы, то есть практически все ресурсы, с которыми вы работаете в Azure.

## <a name="create-a-resource-group"></a>Создание группы ресурсов

Чтобы создать группу ресурсов, используйте команду [az group create](/cli/azure/group#az_group_create):

```azurecli
az group create --name MyResourceGroup --location eastus
```

Группа ресурсов находится в одном расположении. Чтобы просмотреть все расположения, поддерживаемые текущей подпиской, выполните команду [az account list-locations](/cli/azure/account#az_account_list_locations).

```azurecli
az account list-locations
```

Чтобы просмотреть все группы ресурсов для текущей подписки, воспользуйтесь командой [az group list](/cli/azure/group#az_group_list).

```azurecli
az group list --output table
```

> [!TIP]
> Параметр `--output` является глобальным, то есть доступным для всех команд. Значение **table** позволяет получить выходные данные в удобном формате. Дополнительные сведения см. в статье [Форматы выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).

Ресурсы создаются в группе ресурсов. В следующем примере показано создание учетной записи хранения с использованием команды [az storage account create](/cli/azure/storage/account#az_storage_account_create):

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

Чтобы удалить группу ресурсов, выполните команду [az group delete](/cli/azure/group#az_group_delete).

```azurecli
az group delete --name MyResourceGroup
```

При удалении группы ресурсов удаляются все относящиеся к ней ресурсы. Отменить удаление ресурсов невозможно. Если вы выполняете любую команду из этой статьи, удаление созданных групп ресурсов очистит учетную запись.

## <a name="persist-a-resource-group"></a>Сохранение группы ресурсов

Сохраняемость параметров позволяет повторно использовать значения для определенных параметров, включая группы ресурсов.

Сначала включите функцию сохраняемости с помощью команды [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):

```azurecli
az config param-persist on
```

После этого создайте еще одну группу ресурсов:

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

Так как функция сохраняемости включена, вы можете не включать параметр `--resource-group` в будущие команды. Следующая команда создает учетную запись хранения в группе **OtherResourceGroup**:

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

Если в команде указана группа ресурсов, приоритет будет отдаваться этой группе ресурсов. Следующая команда создает группу хранения в группе ресурсов **StorageGroups**:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

Но если в качестве значения вы укажете другую группу ресурсов, Azure CLI сбросит сохраненное значение. В новых командах будет использоваться группа ресурсов **StorageGroups**. Сохраненные значения можно просмотреть с помощью команды [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show).

```azurecli
az config param-persist show
```

Эта команда позволяет получить текущие сохраненные значения. Эти значения хранятся в файле с именем *local_context_\<username>* в скрытом каталоге *.azure*. Azure CLI создает каталог в текущем расположении, когда вы впервые создаете сохраняемое значение.

Завершив работу с сохраненными параметрами, выполните команду [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off).

```azurecli
az config param-persist off
```

Azure CLI сохранит сохраненные значения. Вы можете просмотреть эти значения в файле локального контекста. Если вы повторно включите функцию сохраняемости параметров, вы увидите, что эти значения уже заданы.

Дополнительные сведения об использовании команд [az config param-persist](/cli/azure/config/param-persist) см. в руководстве [Использование сохраненных параметров для упрощения работы с последовательными командами Azure CLI](/cli/azure/param-persist-tutorial).

## <a name="set-a-default-resource-group"></a>Определение группы ресурсов по умолчанию

Вы можете задать группу ресурсов по умолчанию для всех команд, выполняемых в локальном интерфейсе Azure CLI или в Azure Cloud Shell. Azure CLI сохраняет эту конфигурацию локально в файле *config*. Чтобы просмотреть текущую конфигурацию, выполните команду [az config get](/cli/azure/config#az_config_get).

```azurecli
az config get
```

В результатах отобразятся группы ресурсов по умолчанию и другие значения по умолчанию. Если вы используете Azure CLI впервые, область результатов может быть пуста.

Чтобы задать группу ресурсов по умолчанию для установленного интерфейса Azure CLI, выполните команду [az config set](/cli/azure/config#az_config_set):

```azurecli
az config set defaults.group=MyResourceGroup
```

Команда задает значение для указанного ключа, в нашем случае — для `defaults.group`. Доступные варианты конфигурации см. в статье [Конфигурация Azure CLI](/cli/azure/azure-cli-configuration).

> [!NOTE]
> Команда [az config set](/cli/azure/config#az_config_set) не проверяет, существует ли указанная группа ресурсов. Эта команда просто сохраняет пару "ключ — значение".

Когда вы выполните предыдущую команду, следующие две команды выведут один тот же результат:

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

Группа ресурсов относится к подписке. Если в вашей организации используется несколько подписок, необходимо указать нужную подписку перед началом работы с группой ресурсов в подписке. Если значение по умолчанию для группы ресурсов не связано с текущей подпиской, возникает ошибка. Дополнительные сведения о нескольких подписках см. в статье [Использование подписок с помощью Azure CLI](manage-azure-subscriptions-azure-cli.md).

Вам не нужно сбрасывать значения по умолчанию, чтобы использовать другие группы ресурсов. Вместо этого просто укажите группу ресурсов:

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

Значение по умолчанию используете только вы. Оно не повлияет на других пользователей или на изменения, внесенные на портале Azure.

Если используются сохраненные значения параметров, как описано в этой статье, эти значения будут иметь приоритет над значениями по умолчанию, заданными в файле *config*.

## <a name="clean-up-resources"></a>Очистка ресурсов

После выполнения команд из этой статьи вы можете удалить все созданные ресурсы с помощью команды [az group delete](/cli/azure/group#az_group_delete).

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

Эта команда удаляет группу ресурсов со всеми ресурсами, которые она содержит.

Вы можете удалить сохраненные параметры, выполнив команду [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete):

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a>См. также раздел

[Настройка Azure CLI](/cli/azure/azure-cli-configuration)

[Руководство по использованию сохраненных параметров для упрощения выполнения последовательных команд Azure CLI](/cli/azure/param-persist-tutorial)

[Использование нескольких подписок Azure](manage-azure-subscriptions-azure-cli.md)
