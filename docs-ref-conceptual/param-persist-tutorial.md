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
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a>Руководство по использованию сохраненных параметров для упрощения выполнения последовательных команд Azure CLI

Azure CLI предлагает функцию хранимых параметров, позволяющую сохранять значения параметров для дальнейшего использования.  В этом учебнике содержатся сведения о работе с сохраненными значениями и использовании этих локальных значений для эффективного выполнения последовательных команд.

Из этого руководства вы узнаете следующее:

> [!div class="checklist"]
> * Использование ссылочных команд **az config param-persist**.
> * Выполнение последовательных команд с помощью хранимых параметров.

В рамках этого учебника использованы следующие команды Azure CLI:

- [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off)
- [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on)
- [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show)
- [az function app create](/cli/azure/functionapp#az_functionapp_create)
- [az group create](/cli/azure/group#az_group_create)
- [az storage account create](/cli/azure/storage/account#az_storage_account_create)


Если у вас еще нет подписки Azure, [создайте бесплатную учетную запись](https://azure.microsoft.com/free/?WT.mc_id=A261C142F), прежде чем начинать работу.

## <a name="prerequisites"></a>Предварительные требования

1. [Установка Azure CLI](install-azure-cli.md)

   При желании для выполнения шагов, описанных в этом учебнике, вы можете использовать Azure Cloud Shell.  Azure Cloud Shell — это интерактивная оболочка среды, с которой можно работать в браузере.  Запустите Cloud Shell с помощью одного из этих методов:

   - Откройте Cloud Shell, перейдя по ссылке: [https://shell.azure.com](https://shell.azure.com)

   - Нажмите кнопку **Cloud Shell** в строке меню в правом верхнем углу окна [портала Azure](https://portal.azure.com).

1. При использовании локальной установки Azure CLI выполните следующие действия:
   - Войдите в систему с помощью команды [az login](/cli/azure/reference-index#az-login), а затем выполните проверку подлинности, следуя инструкциям в окне терминала.

     ```azurecli
     az login
     ```
    - Для этого учебника требуется пакет Azure CLI версии 2.12.0 или более поздней.  Выполните команду [az version](/cli/azure/reference-index?#az_version), чтобы узнать установленную версию и зависимые библиотеки. Чтобы обновиться до последней версии, выполните команду [az upgrade](/cli/azure/reference-index?#az_upgrade).

## <a name="1-determine-your-local-directory"></a>1. Определение локального каталога

Хранимые параметры хранятся в рабочей папке учетной записи хранения Azure, используемой Azure Cloud Shell.  При использовании локальной установки Azure CLI значения сохраняются в рабочей папке на компьютере.

Чтобы найти, создать или изменить рабочую папку, используемую Azure CLI, воспользуйтесь знакомыми командами CLI.

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a>2. Включение хранимых параметров

[Хранимые параметры](/cli/azure/param-persist) необходимо включить перед сохранением значений.  Вы будете получать предупреждение, пока **az config param-persist** не перейдет из экспериментального этапа.  Сведения о ссылочных типах, состоянии и уровнях поддержки Azure CLI см. в статье [Обзор. Ссылочные типы и состояние Azure CLI](/cli/azure/reference-types-and-status).

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a>3. Создание хранимых параметров

Чтобы сохранить значения для хранимых параметров, выполните любую команду Azure CLI, содержащую параметры, которые необходимо сохранить.  Например, создайте группу ресурсов, и параметры **--location** и **--name** будут сохранены для будущего использования.

1. Сохраните расположение и имя группы ресурсов.
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

1. Используя новые хранимые параметры, создайте учетную запись хранения.

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

1. Создайте хранимый параметр без создания нового ресурса.

   Если вы не хотите создавать новый ресурс Azure, параметры **resource_group_name** и **location** можно сохранить с помощью команд без функции создания, таких как **show** или **list**.   Полный список поддерживаемых параметров и действия, необходимых для сохранения значений, см. на [этой странице](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables).  В этом примере также выполняется удаление всех значений параметров с помощью команды [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).

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

## <a name="4-replace-persisted-parameters"></a>4. Замена хранимых параметров

Заменить сохраненное значение параметра так же просто, как выполнить команду, содержащую другое значение.

1. Создайте новые хранимые параметры.
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

1. Замените только что сохраненные значения.

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
   > Даже если хранимые параметры включены, их не нужно использовать.  Вы по-прежнему можете выполнять команды со всеми указанными значениями параметров.  Однако имейте в виду, что при включении хранимых параметров _вы будете создавать новые хранимые параметры или перезаписывать имеющиеся._

## <a name="5-execute-sequential-commands"></a>5. Выполнение последовательных команд

Эти скрипты создают приложение-функцию Azure с помощью плана потребления.

### <a name="using-persisted-parameters"></a>[С использованием хранимых параметров](#tab/azure-cli)

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

### <a name="without-persisted-parameters"></a>[Без хранимых параметров](#tab/azure-portal)

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

## <a name="6-delete-persisted-parameters"></a>6. Удаление хранимых параметров

Чтобы удалить записи, выполните команду [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete).

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete --name resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> При удалении ресурса Azure хранимые параметры не обновляются.
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

## <a name="7-turn-persisted-parameters-off"></a>7. Выключение хранимых параметров

Вы можете выключить хранимые параметры с помощью команды [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), однако сохраненные данные хранимых параметров при этом не удалятся.

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a>8. Очистка ресурсов

Вы можете удалить ставшие ненужными группу ресурсов и все связанные с ней ресурсы, выполнив команду [az group delete](/cli/azure/group).

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a>См. также раздел

- [Работа с хранимыми параметрами Azure CLI](param-persist-howto.md)
- [Настройка Azure CLI с помощью команды az configure](/cli/azure/azure-cli-configuration)
