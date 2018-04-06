---
title: Расширение псевдонимов Azure CLI 2.0
description: Как использовать расширение псевдонимов Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: e457d78b1009fe573554df36db18f525516e0b4a
ms.sourcegitcommit: 335c11e6c34f7907e61a43507745ba84ed4e7469
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2018
---
# <a name="the-azure-cli-20-alias-extension"></a>Расширение псевдонимов Azure CLI 2.0

Расширение псевдонимов позволяет пользователям определять команды для Azure CLI с помощью существующих команд. Псевдонимы оптимизируют и упрощают рабочие процессы, позволяя использовать ярлыки и позиционные аргументы. Так как поддержка псевдонимов осуществляется на базе модуля шаблонов Jinja2, вы можете использовать расширенные функции обработки аргументов.

> [!NOTE]
> Эта функция предоставляется в режиме общедоступной предварительной версии. Функции и формат файла конфигурации могут отличаться.

## <a name="install-the-alias-extension"></a>Установка расширения псевдонимов

Минимальная требуемая версия Azure CLI для использования расширения псевдонимов — **2.0.28**. Чтобы проверить используемую версию CLI, выполните `az --version`. При необходимости обновите [установку CLI Azure 2.0](./install-azure-cli.md).

Установите расширение с помощью команды [az extension add](/cli/azure/extension#az-extension-add).

```azurecli
az extension add --name alias
```

Проверьте установку расширения с помощью команды [az extension list](/cli/azure/extension#az-extension-list). Если расширение псевдонимов установлено правильно, оно отобразится в выходных данных команды.

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a>Обновление расширения

Так как расширение псевдонимов сейчас активно разрабатывается, новые версии выходят регулярно. Новые версии не устанавливаются автоматически при каждом обновлении CLI. Установите обновление расширения с помощью команды [az extension update](/cli/azure/extension#az-extension-update).

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a>Формат файла псевдонимов команд

Определения псевдонимов команд записываются в файл конфигурации, расположенный здесь: `$AZURE_USER_CONFIG/alias`. По умолчанию для `AZURE_USER_CONFIG` устанавливается значение `$HOME/.azure` в Linux и macOS и `%USERPROFILE%\.azure` в Windows. Файлы конфигурации псевдонимов записываются в формате INI. Общий формат для псевдонимов команд:

```
[command_name]
command = invoked_commands
```

Не включайте `az` как часть команды.

## <a name="create-simple-alias-commands"></a>Создание простых псевдонимов команд

Псевдонимы используются для сокращения существующих групп команд или имен команд. Например, можно сократить группу команд `group` до `rg` и команду `list` до `ls`.

```
[rg]
command = group

[ls]
command = list
```

Эти заново определенные псевдонимы теперь можно использовать в любом месте согласно их определению.

```azurecli
az rg list
az rg ls
az vm ls
```

Псевдонимы также могут быть представлены сочетаниями клавиш для завершения команд. В следующем примере перечислены доступные группы ресурсов и их расположения в выходной таблице:

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

Теперь `ls-groups` можно запускать, как любые другие команды CLI.

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a>Создание псевдонима команды с аргументами

Вы также можете добавить позиционные аргументы для псевдонима команды, включив их как `{{ arg_name }}` в имя псевдонима. Пробелы внутри скобок являются обязательными.

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

В следующем примере псевдонима показано, как использовать позиционные аргументы, чтобы получить общедоступный IP-адрес для виртуальной машины.

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

При выполнении этой команды вы предоставляете значения позиционным аргументам.

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

Вы также можете использовать переменные среды в командах, вызываемых с помощью псевдонимов, которые вычисляются во время выполнения команды. В следующем примере добавляется псевдоним `create-rg`, который создает группу ресурсов в `eastus` и добавляет тег `owner`. Для этого тега присваивается значение локальной переменной `USER`.

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a>Обработка аргументов с помощью шаблонов Jinja2

Замена аргументов в расширении псевдонимов выполняется с помощью [Jinja2](http://jinja.pocoo.org/docs/2.10/). Это позволяет использовать все возможности модуля шаблонов Jinja2. Шаблоны позволяют выполнять такие действия, как извлечение данных и подстановка в строках.

С помощью шаблонов Jinja2 вы можете создавать псевдонимы, которые принимают больше разных типов аргументов, чем базовая команда. Например, можно создать псевдоним, который принимает URL-адрес хранилища. Затем этот URL-адрес анализируется для передачи имен учетной записи и контейнера команде хранилища.

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

См. дополнительные сведения о [модуле шаблонов Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).

## <a name="uninstall-the-alias-extension"></a>Удаление расширения псевдонимов

Удалите расширение с помощью команды [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli
az extension remove --name alias
```

Если вы удаляете расширение из-за ошибки или другой проблемы, [отправьте сообщение об этом на GitHub](https://github.com/Azure/azure-cli-extensions/issues), чтобы мы реализовали исправление.
