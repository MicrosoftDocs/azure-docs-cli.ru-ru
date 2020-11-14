---
title: Учебник по использованию хранимых параметров с помощью Azure CLI
description: Учебник по сохранению значений параметров Azure CLI для повторного использования с помощью команды az config param-persis
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 49bf1d852f000dfbe6251cc15bd63e780b3bc91a
ms.sourcegitcommit: 8d514f4147d6edfc02d8d95d5a4243d100a7fcc9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "93423209"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a><span data-ttu-id="f3922-103">Руководство по использованию сохраненных параметров для упрощения выполнения последовательных команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f3922-103">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>

<span data-ttu-id="f3922-104">Azure CLI предлагает функцию хранимых параметров, позволяющую сохранять значения параметров для дальнейшего использования.</span><span class="sxs-lookup"><span data-stu-id="f3922-104">Azure CLI offers persisted parameters that enable you to store parameter values for continued use.</span></span>  <span data-ttu-id="f3922-105">В этом учебнике содержатся сведения о работе с сохраненными значениями и использовании этих локальных значений для эффективного выполнения последовательных команд.</span><span class="sxs-lookup"><span data-stu-id="f3922-105">In this tutorial, you learn how to work with persisted values, and use these local values to efficiently execute sequential commands.</span></span>

<span data-ttu-id="f3922-106">Из этого руководства вы узнаете следующее:</span><span class="sxs-lookup"><span data-stu-id="f3922-106">In this tutorial, you will learn to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="f3922-107">Использование ссылочных команд **az config param-persist**.</span><span class="sxs-lookup"><span data-stu-id="f3922-107">Use **az config param-persist** reference commands</span></span>
> * <span data-ttu-id="f3922-108">Выполнение последовательных команд с помощью хранимых параметров.</span><span class="sxs-lookup"><span data-stu-id="f3922-108">Execute sequential commands using persisted parameters</span></span>

<span data-ttu-id="f3922-109">В рамках этого учебника использованы следующие команды Azure CLI:</span><span class="sxs-lookup"><span data-stu-id="f3922-109">This tutorial uses the following Azure CLI commands</span></span>

- [<span data-ttu-id="f3922-110">az config param-persist delete</span><span class="sxs-lookup"><span data-stu-id="f3922-110">az config param-persist delete</span></span>](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [<span data-ttu-id="f3922-111">az config param-persist off</span><span class="sxs-lookup"><span data-stu-id="f3922-111">az config param-persist off</span></span>](/cli/azure/config/param-persist#az_config_param_persist_off)
- [<span data-ttu-id="f3922-112">az config param-persist on</span><span class="sxs-lookup"><span data-stu-id="f3922-112">az config param-persist on</span></span>](/cli/azure/config/param-persist#az_config_param_persist_on)
- [<span data-ttu-id="f3922-113">az config param-persist show</span><span class="sxs-lookup"><span data-stu-id="f3922-113">az config param-persist show</span></span>](/cli/azure/config/param-persist#az_config_param_persist_show)
- [<span data-ttu-id="f3922-114">az function app create</span><span class="sxs-lookup"><span data-stu-id="f3922-114">az function app create</span></span>](/cli/azure/functionapp#az_functionapp_create)
- [<span data-ttu-id="f3922-115">az group create</span><span class="sxs-lookup"><span data-stu-id="f3922-115">az group create</span></span>](/cli/azure/group#az_group_create)
- [<span data-ttu-id="f3922-116">az storage account create</span><span class="sxs-lookup"><span data-stu-id="f3922-116">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)


<span data-ttu-id="f3922-117">Если у вас еще нет подписки Azure, [создайте бесплатную учетную запись](https://azure.microsoft.com/free/?WT.mc_id=A261C142F), прежде чем начинать работу.</span><span class="sxs-lookup"><span data-stu-id="f3922-117">If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) before you begin.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3922-118">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f3922-118">Prerequisites</span></span>

1. [<span data-ttu-id="f3922-119">Установка Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f3922-119">Install the Azure CLI</span></span>](install-azure-cli.md)

   <span data-ttu-id="f3922-120">При желании для выполнения шагов, описанных в этом учебнике, вы можете использовать Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f3922-120">If you prefer, you can also use Azure Cloud Shell to complete the steps in this tutorial.</span></span>  <span data-ttu-id="f3922-121">Azure Cloud Shell — это интерактивная оболочка среды, с которой можно работать в браузере.</span><span class="sxs-lookup"><span data-stu-id="f3922-121">Azure Cloud Shell is an interactive shell environment that you use through your browser.</span></span>  <span data-ttu-id="f3922-122">Запустите Cloud Shell с помощью одного из этих методов:</span><span class="sxs-lookup"><span data-stu-id="f3922-122">Start Cloud Shell by using one of these methods:</span></span>

   - <span data-ttu-id="f3922-123">Откройте Cloud Shell, перейдя по ссылке: [https://shell.azure.com](https://shell.azure.com)</span><span class="sxs-lookup"><span data-stu-id="f3922-123">Open Cloud Shell by going to [https://shell.azure.com](https://shell.azure.com)</span></span>

   - <span data-ttu-id="f3922-124">Нажмите кнопку **Cloud Shell** в строке меню в правом верхнем углу окна [портала Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="f3922-124">Select the **Cloud Shell** button on the menu bar at the upper right corner in the [Azure portal](https://portal.azure.com)</span></span>

1. <span data-ttu-id="f3922-125">При использовании локальной установки Azure CLI выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="f3922-125">If you are using a local install of the Azure CLI, complete the following:</span></span>
   - <span data-ttu-id="f3922-126">Войдите в систему с помощью команды [az login](/cli/azure/reference-index#az-login), а затем выполните проверку подлинности, следуя инструкциям в окне терминала.</span><span class="sxs-lookup"><span data-stu-id="f3922-126">Sign in using the [az login](/cli/azure/reference-index#az-login) command, then follow the steps displayed in your terminal to complete the authentication process.</span></span>

     ```azurecli
     az login
     ```
    - <span data-ttu-id="f3922-127">Для этого учебника требуется пакет Azure CLI версии 2.12.0 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="f3922-127">This tutorial requires version 2.12.0 or later of the Azure CLI.</span></span>  <span data-ttu-id="f3922-128">Выполните команду [az version](/cli/azure/reference-index?#az_version), чтобы узнать установленную версию и зависимые библиотеки.</span><span class="sxs-lookup"><span data-stu-id="f3922-128">Run [az version](/cli/azure/reference-index?#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="f3922-129">Чтобы обновиться до последней версии, выполните команду [az upgrade](/cli/azure/reference-index?#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="f3922-129">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index?#az_upgrade).</span></span>

## <a name="1-determine-your-local-directory"></a><span data-ttu-id="f3922-130">1. Определение локального каталога</span><span class="sxs-lookup"><span data-stu-id="f3922-130">1. Determine your local directory</span></span>

<span data-ttu-id="f3922-131">Хранимые параметры хранятся в рабочей папке учетной записи хранения Azure, используемой Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f3922-131">Persisted parameter values are stored in the working directory of the Azure storage account used by Azure Cloud Shell.</span></span>  <span data-ttu-id="f3922-132">При использовании локальной установки Azure CLI значения сохраняются в рабочей папке на компьютере.</span><span class="sxs-lookup"><span data-stu-id="f3922-132">If you are using a local install of the Azure CLI, values are stored in the working directory on your machine.</span></span>

<span data-ttu-id="f3922-133">Чтобы найти, создать или изменить рабочую папку, используемую Azure CLI, воспользуйтесь знакомыми командами CLI.</span><span class="sxs-lookup"><span data-stu-id="f3922-133">To find, create or change the working directory being used by the Azure CLI, use these familiar CLI commands.</span></span>

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a><span data-ttu-id="f3922-134">2. Включение хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-134">2. Turn on Persisted parameters</span></span>

<span data-ttu-id="f3922-135">[Хранимые параметры](/cli/azure/param-persist) необходимо включить перед сохранением значений.</span><span class="sxs-lookup"><span data-stu-id="f3922-135">[Persisted parameters](/cli/azure/param-persist) must be turned on before parameter values can be stored.</span></span>  <span data-ttu-id="f3922-136">Вы будете получать предупреждение, пока **az config param-persist** не перейдет из экспериментального этапа.</span><span class="sxs-lookup"><span data-stu-id="f3922-136">You will receive a warning until **az config param-persist** moves out of the experimental stage.</span></span>  <span data-ttu-id="f3922-137">Сведения о ссылочных типах, состоянии и уровнях поддержки Azure CLI см. в статье [Обзор. Ссылочные типы и состояние Azure CLI](/cli/azure/reference-types-and-status).</span><span class="sxs-lookup"><span data-stu-id="f3922-137">See [Overview: Azure CLI reference types and status](/cli/azure/reference-types-and-status) to learn about the Azure CLI reference types, status, and support levels.</span></span>

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a><span data-ttu-id="f3922-138">3. Создание хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-138">3. Create persisted parameters</span></span>

<span data-ttu-id="f3922-139">Чтобы сохранить значения для хранимых параметров, выполните любую команду Azure CLI, содержащую параметры, которые необходимо сохранить.</span><span class="sxs-lookup"><span data-stu-id="f3922-139">To store values for persisted parameters, execute an Azure CLI command of your choice that contains the parameters you want to store.</span></span>  <span data-ttu-id="f3922-140">Например, создайте группу ресурсов, и параметры **--location** и **--name** будут сохранены для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f3922-140">For example, create a resource group and the **--location** and **--name** parameters are stored for future use.</span></span>

1. <span data-ttu-id="f3922-141">Сохраните расположение и имя группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f3922-141">Store the location and resource group name.</span></span>
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. <span data-ttu-id="f3922-142">Используя новые хранимые параметры, создайте учетную запись хранения.</span><span class="sxs-lookup"><span data-stu-id="f3922-142">Using the new persisted parameters, create a storage account.</span></span>

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="f3922-143">Создайте хранимый параметр без создания нового ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3922-143">Create a persisted parameter without creating a new resource.</span></span>

   <span data-ttu-id="f3922-144">Если вы не хотите создавать новый ресурс Azure, параметры **resource_group_name** и **location** можно сохранить с помощью команд без функции создания, таких как **show** или **list**.</span><span class="sxs-lookup"><span data-stu-id="f3922-144">If you do not want to create a new Azure resource, **resource_group_name** and **location** parameters can be stored by using non-create commands like **show** or **list**.</span></span>   <span data-ttu-id="f3922-145">Полный список поддерживаемых параметров и действия, необходимых для сохранения значений, см. на [этой странице](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).</span><span class="sxs-lookup"><span data-stu-id="f3922-145">See [Azure CLI persisted parameters](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) for a full list of supported parameters,   and the action needed to retain values.</span></span>  <span data-ttu-id="f3922-146">В этом примере также выполняется удаление всех значений параметров с помощью команды [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).</span><span class="sxs-lookup"><span data-stu-id="f3922-146">This example also removes all parameter values by using the [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) command.</span></span>

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the **resource_group_name** stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a><span data-ttu-id="f3922-147">4. Замена хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-147">4. Replace persisted parameters</span></span>

<span data-ttu-id="f3922-148">Заменить сохраненное значение параметра так же просто, как выполнить команду, содержащую другое значение.</span><span class="sxs-lookup"><span data-stu-id="f3922-148">Replacing a stored parameter value is as simple as executing a command containing a different value.</span></span>

1. <span data-ttu-id="f3922-149">Создайте новые хранимые параметры.</span><span class="sxs-lookup"><span data-stu-id="f3922-149">Create new persisted parameters.</span></span>
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="f3922-150">Замените только что сохраненные значения.</span><span class="sxs-lookup"><span data-stu-id="f3922-150">Replace the newly stored values.</span></span>

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > <span data-ttu-id="f3922-151">Даже если хранимые параметры включены, их не нужно использовать.</span><span class="sxs-lookup"><span data-stu-id="f3922-151">Even if persisted parameters are turned on, you don't have to use them.</span></span>  <span data-ttu-id="f3922-152">Вы по-прежнему можете выполнять команды со всеми указанными значениями параметров.</span><span class="sxs-lookup"><span data-stu-id="f3922-152">You can still execute commands with all parameter values specified.</span></span>  <span data-ttu-id="f3922-153">Однако имейте в виду, что при включении хранимых параметров _вы будете создавать новые хранимые параметры или перезаписывать имеющиеся._</span><span class="sxs-lookup"><span data-stu-id="f3922-153">However, be aware that with persisted parameters turned on, _you will be creating new persisted parameters, or overwriting existing ones._</span></span>

## <a name="5-execute-sequential-commands"></a><span data-ttu-id="f3922-154">5. Выполнение последовательных команд</span><span class="sxs-lookup"><span data-stu-id="f3922-154">5. Execute sequential commands</span></span>

<span data-ttu-id="f3922-155">Эти скрипты создают приложение-функцию Azure с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="f3922-155">These scripts create an Azure Function app using the Consumption plan.</span></span>

### <a name="using-persisted-parameters"></a>[<span data-ttu-id="f3922-156">С использованием хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-156">Using persisted parameters</span></span>](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[<span data-ttu-id="f3922-157">Без хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-157">Without persisted parameters</span></span>](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a><span data-ttu-id="f3922-158">6. Удаление хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-158">6. Delete persisted parameters</span></span>

<span data-ttu-id="f3922-159">Чтобы удалить записи, выполните команду [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete).</span><span class="sxs-lookup"><span data-stu-id="f3922-159">Use the [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) command to remove entries.</span></span>

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete --name resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> <span data-ttu-id="f3922-160">При удалении ресурса Azure хранимые параметры не обновляются.</span><span class="sxs-lookup"><span data-stu-id="f3922-160">Persisted parameters do not get updated when an Azure resource is deleted.</span></span>
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a><span data-ttu-id="f3922-161">7. Выключение хранимых параметров</span><span class="sxs-lookup"><span data-stu-id="f3922-161">7. Turn persisted parameters off</span></span>

<span data-ttu-id="f3922-162">Вы можете выключить хранимые параметры с помощью команды [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), однако сохраненные данные хранимых параметров при этом не удалятся.</span><span class="sxs-lookup"><span data-stu-id="f3922-162">You can turn persisted parameters off by using the [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) command, but your saved persisted parameters data won't be deleted.</span></span>

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a><span data-ttu-id="f3922-163">8. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="f3922-163">8. Clean up resources</span></span>

<span data-ttu-id="f3922-164">Вы можете удалить ставшие ненужными группу ресурсов и все связанные с ней ресурсы, выполнив команду [az group delete](/cli/azure/group).</span><span class="sxs-lookup"><span data-stu-id="f3922-164">When no longer needed, use the [az group delete](/cli/azure/group) command to remove the resource group, and all related resources.</span></span>

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a><span data-ttu-id="f3922-165">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="f3922-165">See also</span></span>

- [<span data-ttu-id="f3922-166">Работа с хранимыми параметрами Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f3922-166">(How to work with Azure CLI persisted parameters</span></span>](param-persist-howto.md)
- [<span data-ttu-id="f3922-167">Настройка Azure CLI с помощью команды az configure</span><span class="sxs-lookup"><span data-stu-id="f3922-167">Azure CLI Configuration using az configure</span></span>](/cli/azure/azure-cli-configuration)
