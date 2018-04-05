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
ms.openlocfilehash: e8419394bb221d2614e15171bd19dd76fd9cd773
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="dc6ac-103">Расширение псевдонимов Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="dc6ac-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="dc6ac-104">Расширение псевдонимов позволяет пользователям определять команды для Azure CLI с помощью существующих команд.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="dc6ac-105">Псевдонимы оптимизируют и упрощают рабочие процессы, позволяя использовать ярлыки и позиционные аргументы.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="dc6ac-106">Так как поддержка псевдонимов осуществляется на базе модуля шаблонов Jinja2, вы можете использовать расширенные функции обработки аргументов.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="dc6ac-107">Эта функция предоставляется в режиме общедоступной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="dc6ac-108">Функции и формат файла конфигурации могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="dc6ac-109">Установка расширения псевдонимов</span><span class="sxs-lookup"><span data-stu-id="dc6ac-109">Install the alias extension</span></span>

<span data-ttu-id="dc6ac-110">Минимальная требуемая версия Azure CLI для использования расширения псевдонимов — **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="dc6ac-111">Чтобы проверить используемую версию CLI, выполните `az --version`.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="dc6ac-112">При необходимости обновите [установку CLI Azure 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="dc6ac-113">Установите расширение с помощью команды [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli
az extension add --name alias
```

<span data-ttu-id="dc6ac-114">Проверьте установку расширения с помощью команды [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="dc6ac-115">Если расширение псевдонимов установлено правильно, оно отобразится в выходных данных команды.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli
az extension list --output table
```

```output
ExtensionType    Name                       Version
---------------  -------------------------  ---------
whl              alias                      0.2.0
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="dc6ac-116">Обновление расширения</span><span class="sxs-lookup"><span data-stu-id="dc6ac-116">Keep the extension up to date</span></span>

<span data-ttu-id="dc6ac-117">Так как расширение псевдонимов сейчас активно разрабатывается, новые версии выходят регулярно.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="dc6ac-118">Новые версии не устанавливаются автоматически при каждом обновлении CLI.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="dc6ac-119">Установите обновление расширения с помощью команды [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli
az extension update --name alias
```

## <a name="alias-commands-file-format"></a><span data-ttu-id="dc6ac-120">Формат файла псевдонимов команд</span><span class="sxs-lookup"><span data-stu-id="dc6ac-120">Alias commands file format</span></span>

<span data-ttu-id="dc6ac-121">Определения псевдонимов команд записываются в файл конфигурации, расположенный здесь: `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-121">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="dc6ac-122">По умолчанию для `AZURE_USER_CONFIG` устанавливается значение `$HOME/.azure` в Linux и macOS и `%USERPROFILE%\.azure` в Windows.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-122">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="dc6ac-123">Файлы конфигурации псевдонимов записываются в формате INI.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-123">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="dc6ac-124">Общий формат для псевдонимов команд:</span><span class="sxs-lookup"><span data-stu-id="dc6ac-124">The general format for alias commands is:</span></span>

```
[command_name]
command = invoked_commands
```

<span data-ttu-id="dc6ac-125">Не включайте `az` как часть команды.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-125">Don't include `az` as part of the command.</span></span>

## <a name="create-simple-alias-commands"></a><span data-ttu-id="dc6ac-126">Создание простых псевдонимов команд</span><span class="sxs-lookup"><span data-stu-id="dc6ac-126">Create simple alias commands</span></span>

<span data-ttu-id="dc6ac-127">Псевдонимы используются для сокращения существующих групп команд или имен команд.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-127">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="dc6ac-128">Например, можно сократить группу команд `group` до `rg` и команду `list` до `ls`.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-128">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```
[rg]
command = group

[ls]
command = list
```

<span data-ttu-id="dc6ac-129">Эти заново определенные псевдонимы теперь можно использовать в любом месте согласно их определению.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-129">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="dc6ac-130">Псевдонимы также могут быть представлены сочетаниями клавиш для завершения команд.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-130">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="dc6ac-131">В следующем примере перечислены доступные группы ресурсов и их расположения в выходной таблице:</span><span class="sxs-lookup"><span data-stu-id="dc6ac-131">The next example lists available resource groups and their locations in table output:</span></span>

```
[ls-groups]
command = group list --query '[].{Name:name, Location:location}' --output table
```

<span data-ttu-id="dc6ac-132">Теперь `ls-groups` можно запускать, как любые другие команды CLI.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-132">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="dc6ac-133">Создание псевдонима команды с аргументами</span><span class="sxs-lookup"><span data-stu-id="dc6ac-133">Create an alias command with arguments</span></span>

<span data-ttu-id="dc6ac-134">Вы также можете добавить позиционные аргументы для псевдонима команды, включив их как `{{ arg_name }}` в имя псевдонима.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-134">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="dc6ac-135">Пробелы внутри фигурных скобок являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-135">The whitespace inside the curly braces is required.</span></span>

```
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoke_including_args
```

<span data-ttu-id="dc6ac-136">В следующем примере псевдонима показано, как использовать позиционные аргументы, чтобы получить общедоступный IP-адрес для виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-136">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

<span data-ttu-id="dc6ac-137">При выполнении этой команды вы предоставляете значения позиционным аргументам.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-137">When running this command, you give values to the positional arguments.</span></span>

```azruecli
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="dc6ac-138">Вы также можете использовать переменные среды в командах, вызываемых с помощью псевдонимов, которые вычисляются во время выполнения команды.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-138">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="dc6ac-139">В следующем примере добавляется псевдоним `create-rg`, который создает группу ресурсов в `eastus` и добавляет тег `owner`.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-139">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="dc6ac-140">Для этого тега присваивается значение локальной переменной `USER`.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-140">This tag is assigned the value of the local environment variable `USER`.</span></span>

```
[create-rg {{ groupName }}]
command = group create --name {{ groupName }} --location eastus --tags owner=$USER
```

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="dc6ac-141">Обработка аргументов с помощью шаблонов Jinja2</span><span class="sxs-lookup"><span data-stu-id="dc6ac-141">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="dc6ac-142">Замена аргументов в расширении псевдонимов выполняется с помощью [Jinja2](http://jinja.pocoo.org/docs/2.10/). Это позволяет использовать все возможности модуля шаблонов Jinja2.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-142">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="dc6ac-143">Шаблоны позволяют выполнять такие действия, как извлечение данных и подстановка в строках.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-143">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="dc6ac-144">С помощью шаблонов Jinja2 вы можете создавать псевдонимы, которые принимают больше разных типов аргументов, чем базовая команда.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-144">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="dc6ac-145">Например, можно создать псевдоним, который принимает URL-адрес хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-145">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="dc6ac-146">Затем этот URL-адрес анализируется для передачи имен учетной записи и контейнера команде хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-146">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```
[storage-ls {{ url }}]
command = storage blob list --account-name {{ url.replace('https://', '').split('.')[0] }} --container-name {{ url.replace('https://', '').split('/')[1] }}
```

<span data-ttu-id="dc6ac-147">См. дополнительные сведения о [модуле шаблонов Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-147">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="dc6ac-148">Удаление расширения псевдонимов</span><span class="sxs-lookup"><span data-stu-id="dc6ac-148">Uninstall the alias extension</span></span>

<span data-ttu-id="dc6ac-149">Удалите расширение с помощью команды [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="dc6ac-149">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```bash
az extension remove --name alias
```

<span data-ttu-id="dc6ac-150">Если вы удаляете расширение из-за ошибки или другой проблемы, [отправьте сообщение об этом на GitHub](https://github.com/Azure/azure-cli-extensions/issues), чтобы мы реализовали исправление.</span><span class="sxs-lookup"><span data-stu-id="dc6ac-150">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
