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
# <a name="working-with-resource-groups-in-azure-cli"></a><span data-ttu-id="6be16-104">Работа с группами ресурсов Azure в Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6be16-104">Working with resource groups in Azure CLI</span></span>

<span data-ttu-id="6be16-105">Группа ресурсов Azure — это контейнер, содержащий связанные ресурсы для решения Azure.</span><span class="sxs-lookup"><span data-stu-id="6be16-105">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="6be16-106">Группа ресурсов может содержать хранилище, виртуальные машины, приложения, панели мониторинга, службы, то есть практически все ресурсы, с которыми вы работаете в Azure.</span><span class="sxs-lookup"><span data-stu-id="6be16-106">A resource group might contain storage, virtual machines, apps, dashboards, services, or almost anything you deal with in Azure.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="6be16-107">Создание группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="6be16-107">Create a resource group</span></span>

<span data-ttu-id="6be16-108">Чтобы создать группу ресурсов, используйте команду [az group create](/cli/azure/group#az_group_create):</span><span class="sxs-lookup"><span data-stu-id="6be16-108">To create a resource group, use the [az group create](/cli/azure/group#az_group_create) command:</span></span>

```azurecli
az group create --name MyResourceGroup --location eastus
```

<span data-ttu-id="6be16-109">Группа ресурсов находится в одном расположении.</span><span class="sxs-lookup"><span data-stu-id="6be16-109">A resource group belongs to a single location.</span></span> <span data-ttu-id="6be16-110">Чтобы просмотреть все расположения, поддерживаемые текущей подпиской, выполните команду [az account list-locations](/cli/azure/account#az_account_list_locations).</span><span class="sxs-lookup"><span data-stu-id="6be16-110">To see all the locations supported in your current subscription, run the [az account list-locations](/cli/azure/account#az_account_list_locations) command:</span></span>

```azurecli
az account list-locations
```

<span data-ttu-id="6be16-111">Чтобы просмотреть все группы ресурсов для текущей подписки, воспользуйтесь командой [az group list](/cli/azure/group#az_group_list).</span><span class="sxs-lookup"><span data-stu-id="6be16-111">To see all the resource groups for your current subscription, use the [az group list](/cli/azure/group#az_group_list) command:</span></span>

```azurecli
az group list --output table
```

> [!TIP]
> <span data-ttu-id="6be16-112">Параметр `--output` является глобальным, то есть доступным для всех команд.</span><span class="sxs-lookup"><span data-stu-id="6be16-112">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="6be16-113">Значение **table** позволяет получить выходные данные в удобном формате.</span><span class="sxs-lookup"><span data-stu-id="6be16-113">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="6be16-114">Дополнительные сведения см. в статье [Форматы выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="6be16-114">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="6be16-115">Ресурсы создаются в группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6be16-115">When you create a resource, you create it in a resource group.</span></span> <span data-ttu-id="6be16-116">В следующем примере показано создание учетной записи хранения с использованием команды [az storage account create](/cli/azure/storage/account#az_storage_account_create):</span><span class="sxs-lookup"><span data-stu-id="6be16-116">The following example shows a storage account created by using the [az storage account create](/cli/azure/storage/account#az_storage_account_create) command:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

<span data-ttu-id="6be16-117">Чтобы удалить группу ресурсов, выполните команду [az group delete](/cli/azure/group#az_group_delete).</span><span class="sxs-lookup"><span data-stu-id="6be16-117">To remove a resource group, run the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
```

<span data-ttu-id="6be16-118">При удалении группы ресурсов удаляются все относящиеся к ней ресурсы.</span><span class="sxs-lookup"><span data-stu-id="6be16-118">When you remove a resource group, you delete all the resources that belong to it.</span></span> <span data-ttu-id="6be16-119">Отменить удаление ресурсов невозможно.</span><span class="sxs-lookup"><span data-stu-id="6be16-119">There's no option to undelete resources.</span></span> <span data-ttu-id="6be16-120">Если вы выполняете любую команду из этой статьи, удаление созданных групп ресурсов очистит учетную запись.</span><span class="sxs-lookup"><span data-stu-id="6be16-120">If you try any of the commands in this article, deleting the resource groups you create cleans up your account.</span></span>

## <a name="persist-a-resource-group"></a><span data-ttu-id="6be16-121">Сохранение группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="6be16-121">Persist a resource group</span></span>

<span data-ttu-id="6be16-122">Сохраняемость параметров позволяет повторно использовать значения для определенных параметров, включая группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6be16-122">Parameter persistence allows you to reuse values for certain parameters, including resource groups.</span></span>

<span data-ttu-id="6be16-123">Сначала включите функцию сохраняемости с помощью команды [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):</span><span class="sxs-lookup"><span data-stu-id="6be16-123">First, turn on the persistence feature by using the [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) command:</span></span>

```azurecli
az config param-persist on
```

<span data-ttu-id="6be16-124">После этого создайте еще одну группу ресурсов:</span><span class="sxs-lookup"><span data-stu-id="6be16-124">After turning on persistence, create another resource group:</span></span>

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

<span data-ttu-id="6be16-125">Так как функция сохраняемости включена, вы можете не включать параметр `--resource-group` в будущие команды.</span><span class="sxs-lookup"><span data-stu-id="6be16-125">As long as persistence is on, your can leave the `--resource-group` parameter out of future commands.</span></span> <span data-ttu-id="6be16-126">Следующая команда создает учетную запись хранения в группе **OtherResourceGroup**:</span><span class="sxs-lookup"><span data-stu-id="6be16-126">The following command creates a storage account in the **OtherResourceGroup** group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="6be16-127">Если в команде указана группа ресурсов, приоритет будет отдаваться этой группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6be16-127">If you specify a resource group in the command, that takes precedence.</span></span> <span data-ttu-id="6be16-128">Следующая команда создает группу хранения в группе ресурсов **StorageGroups**:</span><span class="sxs-lookup"><span data-stu-id="6be16-128">The following command creates a storage group in a resource group called **StorageGroups**:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

<span data-ttu-id="6be16-129">Но если в качестве значения вы укажете другую группу ресурсов, Azure CLI сбросит сохраненное значение.</span><span class="sxs-lookup"><span data-stu-id="6be16-129">Once you specify another resource group as a value, however, Azure CLI resets the persisted value.</span></span> <span data-ttu-id="6be16-130">В новых командах будет использоваться группа ресурсов **StorageGroups**.</span><span class="sxs-lookup"><span data-stu-id="6be16-130">New commands use **StorageGroups** as the resource group.</span></span> <span data-ttu-id="6be16-131">Сохраненные значения можно просмотреть с помощью команды [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show).</span><span class="sxs-lookup"><span data-stu-id="6be16-131">You can see the persisted values by using the [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) command:</span></span>

```azurecli
az config param-persist show
```

<span data-ttu-id="6be16-132">Эта команда позволяет получить текущие сохраненные значения.</span><span class="sxs-lookup"><span data-stu-id="6be16-132">This command shows you the current persisted values.</span></span> <span data-ttu-id="6be16-133">Эти значения хранятся в файле с именем *local_context_\<username>* в скрытом каталоге *.azure*.</span><span class="sxs-lookup"><span data-stu-id="6be16-133">These values are stored in a file called *local_context_\<username>* in a hidden directory called *.azure*.</span></span> <span data-ttu-id="6be16-134">Azure CLI создает каталог в текущем расположении, когда вы впервые создаете сохраняемое значение.</span><span class="sxs-lookup"><span data-stu-id="6be16-134">Azure CLI creates the directory in your current location when you first create a persistent value.</span></span>

<span data-ttu-id="6be16-135">Завершив работу с сохраненными параметрами, выполните команду [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off).</span><span class="sxs-lookup"><span data-stu-id="6be16-135">When you're done using persisted parameters, run the [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) command:</span></span>

```azurecli
az config param-persist off
```

<span data-ttu-id="6be16-136">Azure CLI сохранит сохраненные значения.</span><span class="sxs-lookup"><span data-stu-id="6be16-136">Azure CLI saves your persisted values.</span></span> <span data-ttu-id="6be16-137">Вы можете просмотреть эти значения в файле локального контекста.</span><span class="sxs-lookup"><span data-stu-id="6be16-137">You can see them in the local context file.</span></span> <span data-ttu-id="6be16-138">Если вы повторно включите функцию сохраняемости параметров, вы увидите, что эти значения уже заданы.</span><span class="sxs-lookup"><span data-stu-id="6be16-138">If you turn on parameter persistence again, those values are already set.</span></span>

<span data-ttu-id="6be16-139">Дополнительные сведения об использовании команд [az config param-persist](/cli/azure/config/param-persist) см. в руководстве [Использование сохраненных параметров для упрощения работы с последовательными командами Azure CLI](/cli/azure/param-persist-tutorial).</span><span class="sxs-lookup"><span data-stu-id="6be16-139">For more information about using the [az config param-persist](/cli/azure/config/param-persist) commands, see [Use persisted parameters to simplify sequential Azure CLI commands](/cli/azure/param-persist-tutorial).</span></span>

## <a name="set-a-default-resource-group"></a><span data-ttu-id="6be16-140">Определение группы ресурсов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6be16-140">Set a default resource group</span></span>

<span data-ttu-id="6be16-141">Вы можете задать группу ресурсов по умолчанию для всех команд, выполняемых в локальном интерфейсе Azure CLI или в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="6be16-141">You can set a default resource group for all the commands that you run from your local Azure CLI or from Azure Cloud Shell.</span></span> <span data-ttu-id="6be16-142">Azure CLI сохраняет эту конфигурацию локально в файле *config*.</span><span class="sxs-lookup"><span data-stu-id="6be16-142">Azure CLI stores this configuration locally in a *config* file.</span></span> <span data-ttu-id="6be16-143">Чтобы просмотреть текущую конфигурацию, выполните команду [az config get](/cli/azure/config#az_config_get).</span><span class="sxs-lookup"><span data-stu-id="6be16-143">To see your current configuration, run the [az config get](/cli/azure/config#az_config_get) command:</span></span>

```azurecli
az config get
```

<span data-ttu-id="6be16-144">В результатах отобразятся группы ресурсов по умолчанию и другие значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6be16-144">The result shows default resource groups and other default values.</span></span> <span data-ttu-id="6be16-145">Если вы используете Azure CLI впервые, область результатов может быть пуста.</span><span class="sxs-lookup"><span data-stu-id="6be16-145">If you're using Azure CLI for the first time, the results might be empty.</span></span>

<span data-ttu-id="6be16-146">Чтобы задать группу ресурсов по умолчанию для установленного интерфейса Azure CLI, выполните команду [az config set](/cli/azure/config#az_config_set):</span><span class="sxs-lookup"><span data-stu-id="6be16-146">To set a default resource group for your Azure CLI installation, run the [az config set](/cli/azure/config#az_config_set) command:</span></span>

```azurecli
az config set defaults.group=MyResourceGroup
```

<span data-ttu-id="6be16-147">Команда задает значение для указанного ключа, в нашем случае — для `defaults.group`.</span><span class="sxs-lookup"><span data-stu-id="6be16-147">The command sets a value for a specified key, in this case `defaults.group`.</span></span> <span data-ttu-id="6be16-148">Доступные варианты конфигурации см. в статье [Конфигурация Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="6be16-148">For available configuration options, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

> [!NOTE]
> <span data-ttu-id="6be16-149">Команда [az config set](/cli/azure/config#az_config_set) не проверяет, существует ли указанная группа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6be16-149">The [az config set](/cli/azure/config#az_config_set) command does not validate the existence of the resource group you enter.</span></span> <span data-ttu-id="6be16-150">Эта команда просто сохраняет пару "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="6be16-150">The command simply stores the key-value pair.</span></span>

<span data-ttu-id="6be16-151">Когда вы выполните предыдущую команду, следующие две команды выведут один тот же результат:</span><span class="sxs-lookup"><span data-stu-id="6be16-151">After you run the command, the following two commands would give you the same result:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

<span data-ttu-id="6be16-152">Группа ресурсов относится к подписке.</span><span class="sxs-lookup"><span data-stu-id="6be16-152">A resource group belongs to a subscription.</span></span> <span data-ttu-id="6be16-153">Если в вашей организации используется несколько подписок, необходимо указать нужную подписку перед началом работы с группой ресурсов в подписке.</span><span class="sxs-lookup"><span data-stu-id="6be16-153">If your organization has more than one subscription, you need to set that subscription before working with a resource group in the subscription.</span></span> <span data-ttu-id="6be16-154">Если значение по умолчанию для группы ресурсов не связано с текущей подпиской, возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="6be16-154">If the default value of a resource group does not belong to your current subscription, an error results.</span></span> <span data-ttu-id="6be16-155">Дополнительные сведения о нескольких подписках см. в статье [Использование подписок с помощью Azure CLI](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6be16-155">For more information about multiple subscriptions, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="6be16-156">Вам не нужно сбрасывать значения по умолчанию, чтобы использовать другие группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6be16-156">You don't have to reset the default to use other resource groups.</span></span> <span data-ttu-id="6be16-157">Вместо этого просто укажите группу ресурсов:</span><span class="sxs-lookup"><span data-stu-id="6be16-157">Instead, specify the resource group:</span></span>

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

<span data-ttu-id="6be16-158">Значение по умолчанию используете только вы.</span><span class="sxs-lookup"><span data-stu-id="6be16-158">The default value is for you only.</span></span> <span data-ttu-id="6be16-159">Оно не повлияет на других пользователей или на изменения, внесенные на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6be16-159">It won't affect other users or changes you make through the Azure portal.</span></span>

<span data-ttu-id="6be16-160">Если используются сохраненные значения параметров, как описано в этой статье, эти значения будут иметь приоритет над значениями по умолчанию, заданными в файле *config*.</span><span class="sxs-lookup"><span data-stu-id="6be16-160">If you are using persisted parameter values, as described in this article, those values take precedence over defaults set in the *config* file.</span></span>

## <a name="clean-up-resources"></a><span data-ttu-id="6be16-161">Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="6be16-161">Clean up resources</span></span>

<span data-ttu-id="6be16-162">После выполнения команд из этой статьи вы можете удалить все созданные ресурсы с помощью команды [az group delete](/cli/azure/group#az_group_delete).</span><span class="sxs-lookup"><span data-stu-id="6be16-162">If you tried any of the commands in this article, you can remove any resources you created by using the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

<span data-ttu-id="6be16-163">Эта команда удаляет группу ресурсов со всеми ресурсами, которые она содержит.</span><span class="sxs-lookup"><span data-stu-id="6be16-163">This command removes the group and all the resources that it contains at once.</span></span>

<span data-ttu-id="6be16-164">Вы можете удалить сохраненные параметры, выполнив команду [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete):</span><span class="sxs-lookup"><span data-stu-id="6be16-164">You can remove the persistent parameters by running the [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) command:</span></span>

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a><span data-ttu-id="6be16-165">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="6be16-165">See also</span></span>

[<span data-ttu-id="6be16-166">Настройка Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6be16-166">Azure CLI configuration</span></span>](/cli/azure/azure-cli-configuration)

[<span data-ttu-id="6be16-167">Руководство по использованию сохраненных параметров для упрощения выполнения последовательных команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6be16-167">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>](/cli/azure/param-persist-tutorial)

[<span data-ttu-id="6be16-168">Использование нескольких подписок Azure</span><span class="sxs-lookup"><span data-stu-id="6be16-168">Use multiple Azure subscriptions</span></span>](manage-azure-subscriptions-azure-cli.md)
