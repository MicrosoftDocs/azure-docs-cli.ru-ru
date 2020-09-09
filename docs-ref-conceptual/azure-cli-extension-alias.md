---
title: Расширение псевдонимов Azure CLI
description: Как использовать расширение псевдонимов Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 576ed223887ff9a20cf5015d96ee4c949576d653
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562844"
---
# <a name="the-azure-cli-alias-extension"></a><span data-ttu-id="e2f33-103">Расширение псевдонимов Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e2f33-103">The Azure CLI alias extension</span></span>

<span data-ttu-id="e2f33-104">Расширение псевдонимов позволяет пользователям определять команды для Azure CLI с помощью существующих команд.</span><span class="sxs-lookup"><span data-stu-id="e2f33-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="e2f33-105">Псевдонимы упрощают рабочий процесс за счет использования ярлыков.</span><span class="sxs-lookup"><span data-stu-id="e2f33-105">Aliases help keep your workflow simple by allowing shortcuts.</span></span> <span data-ttu-id="e2f33-106">Так как поддержка псевдонимов осуществляется на базе модуля шаблонов Jinja2, вы можете использовать расширенные функции обработки аргументов.</span><span class="sxs-lookup"><span data-stu-id="e2f33-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="e2f33-107">Эта функция предоставляется в режиме общедоступной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="e2f33-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="e2f33-108">Функции и формат файла конфигурации могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="e2f33-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="e2f33-109">Установка расширения псевдонимов</span><span class="sxs-lookup"><span data-stu-id="e2f33-109">Install the alias extension</span></span>

<span data-ttu-id="e2f33-110">Минимальная требуемая версия Azure CLI для использования расширения псевдонимов — **2.0.28**.</span><span class="sxs-lookup"><span data-stu-id="e2f33-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="e2f33-111">Чтобы проверить используемую версию CLI, выполните `az --version`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="e2f33-112">Если необходимо обновить установленный пакет CLI, следуйте инструкциям в статье [Установка Azure CLI](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e2f33-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI](./install-azure-cli.md).</span></span>

<span data-ttu-id="e2f33-113">Установите расширение с помощью команды [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="e2f33-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="e2f33-114">Проверьте установку расширения с помощью команды [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="e2f33-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="e2f33-115">Если расширение псевдонимов установлено правильно, оно отобразится в выходных данных команды.</span><span class="sxs-lookup"><span data-stu-id="e2f33-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="e2f33-116">Обновление расширения</span><span class="sxs-lookup"><span data-stu-id="e2f33-116">Keep the extension up-to-date</span></span>

<span data-ttu-id="e2f33-117">Так как расширение псевдонимов сейчас активно разрабатывается, новые версии выходят регулярно.</span><span class="sxs-lookup"><span data-stu-id="e2f33-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="e2f33-118">При обновлении CLI новые версии не устанавливаются.</span><span class="sxs-lookup"><span data-stu-id="e2f33-118">New versions aren't installed when you update the CLI.</span></span> <span data-ttu-id="e2f33-119">Установите обновление расширения с помощью команды [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="e2f33-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="e2f33-120">Управление псевдонимами для Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e2f33-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="e2f33-121">Расширение псевдонимов позволяет создавать псевдонимы для других команд CLI и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="e2f33-121">The alias extension lets you create and manage aliases for other CLI commands.</span></span> <span data-ttu-id="e2f33-122">Чтобы просмотреть сведения о всех доступных командах и их параметрах, выполните команду alias с параметром `--help`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-122">To view all the available commands and parameter details, run the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="e2f33-123">Создание простых псевдонимов команд</span><span class="sxs-lookup"><span data-stu-id="e2f33-123">Create simple alias commands</span></span>

<span data-ttu-id="e2f33-124">Псевдонимы используются для сокращения существующих групп команд или имен команд.</span><span class="sxs-lookup"><span data-stu-id="e2f33-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="e2f33-125">Например, можно сократить группу команд `group` до `rg` и команду `list` до `ls`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="e2f33-126">Эти заново определенные псевдонимы теперь можно использовать в любом месте согласно их определению.</span><span class="sxs-lookup"><span data-stu-id="e2f33-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="e2f33-127">Не добавляйте `az` в команду.</span><span class="sxs-lookup"><span data-stu-id="e2f33-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="e2f33-128">Псевдонимы также могут быть представлены сочетаниями клавиш для завершения команд.</span><span class="sxs-lookup"><span data-stu-id="e2f33-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="e2f33-129">В следующем примере перечислены доступные группы ресурсов и их расположения в выходной таблице:</span><span class="sxs-lookup"><span data-stu-id="e2f33-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="e2f33-130">Теперь `ls-groups` можно запускать, как любые другие команды CLI.</span><span class="sxs-lookup"><span data-stu-id="e2f33-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="e2f33-131">Создание псевдонима команды с аргументами</span><span class="sxs-lookup"><span data-stu-id="e2f33-131">Create an alias command with arguments</span></span>

<span data-ttu-id="e2f33-132">Вы также можете добавить позиционные аргументы для псевдонима команды, включив их как `{{ arg_name }}` в имя псевдонима.</span><span class="sxs-lookup"><span data-stu-id="e2f33-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="e2f33-133">Пробелы внутри скобок являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="e2f33-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="e2f33-134">В следующем примере псевдонима показано, как использовать позиционные аргументы, чтобы получить общедоступный IP-адрес для виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="e2f33-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="e2f33-135">При выполнении этой команды вы предоставляете значения позиционным аргументам.</span><span class="sxs-lookup"><span data-stu-id="e2f33-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="e2f33-136">В командах-псевдонимах также можно использовать переменные среды, которые вычисляются во время выполнения.</span><span class="sxs-lookup"><span data-stu-id="e2f33-136">You can also use environment variables in aliased commands, which are evaluated at runtime.</span></span> <span data-ttu-id="e2f33-137">В следующем примере добавляется псевдоним `create-rg`, который создает группу ресурсов в `eastus` и добавляет тег `owner`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="e2f33-138">Для этого тега присваивается значение локальной переменной `USER`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="e2f33-139">Чтобы зарегистрировать переменные среды внутри команды псевдонима, знак доллара `$` необходимо экранировать.</span><span class="sxs-lookup"><span data-stu-id="e2f33-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="e2f33-140">Обработка аргументов с помощью шаблонов Jinja2</span><span class="sxs-lookup"><span data-stu-id="e2f33-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="e2f33-141">Подстановка аргументов в расширении псевдонимов выполняется с помощью шаблона [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span><span class="sxs-lookup"><span data-stu-id="e2f33-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span></span> <span data-ttu-id="e2f33-142">Шаблоны Jinja2 позволяют манипулировать аргументами.</span><span class="sxs-lookup"><span data-stu-id="e2f33-142">Jinja2 templates allow for manipulating the arguments.</span></span>

<span data-ttu-id="e2f33-143">С помощью шаблонов Jinja2 вы можете создавать псевдонимы, которые принимают другие типы аргументов, отличные от аргументов базовой команды.</span><span class="sxs-lookup"><span data-stu-id="e2f33-143">With Jinja2 templates, you can write aliases that take different types of arguments than the underlying command.</span></span> <span data-ttu-id="e2f33-144">Например, можно создать псевдоним, который принимает URL-адрес хранилища.</span><span class="sxs-lookup"><span data-stu-id="e2f33-144">For example, you can make an alias that takes a storage URL.</span></span> <span data-ttu-id="e2f33-145">Затем этот URL-адрес анализируется для передачи имен учетной записи и контейнера команде хранилища.</span><span class="sxs-lookup"><span data-stu-id="e2f33-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="e2f33-146">См. дополнительные сведения о [модуле шаблонов Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="e2f33-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="e2f33-147">Файл конфигурации псевдонимов</span><span class="sxs-lookup"><span data-stu-id="e2f33-147">Alias configuration file</span></span>

<span data-ttu-id="e2f33-148">Еще один способ создания и изменения псевдонимов заключается в изменении файла конфигурации псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="e2f33-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="e2f33-149">Определения псевдонимов команд записываются в файл конфигурации, расположенный здесь: `$AZURE_USER_CONFIG/alias`.</span><span class="sxs-lookup"><span data-stu-id="e2f33-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="e2f33-150">По умолчанию для `AZURE_USER_CONFIG` устанавливается значение `$HOME/.azure` в Linux и macOS и `%USERPROFILE%\.azure` в Windows.</span><span class="sxs-lookup"><span data-stu-id="e2f33-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="e2f33-151">Файлы конфигурации псевдонимов записываются в формате INI.</span><span class="sxs-lookup"><span data-stu-id="e2f33-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="e2f33-152">Псевдонимы команд имеют такой формат:</span><span class="sxs-lookup"><span data-stu-id="e2f33-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="e2f33-153">Псевдонимы с позиционными аргументами имеют такой формат:</span><span class="sxs-lookup"><span data-stu-id="e2f33-153">For aliases that have positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="e2f33-154">Создание псевдонима команды с аргументами с помощью файла конфигурации псевдонимов</span><span class="sxs-lookup"><span data-stu-id="e2f33-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="e2f33-155">В следующем примере показан псевдоним команды с аргументами.</span><span class="sxs-lookup"><span data-stu-id="e2f33-155">The next example shows an alias for a command with arguments.</span></span> <span data-ttu-id="e2f33-156">Эта команда получает общедоступный IP-адрес виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="e2f33-156">This command gets the public IP address for a VM.</span></span> <span data-ttu-id="e2f33-157">Команды-псевдонимы должны занимать одну строку и использовать все аргументы в имени псевдонима.</span><span class="sxs-lookup"><span data-stu-id="e2f33-157">Aliased commands must all be on a single line, and use all of the arguments in the alias name.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="e2f33-158">Удаление расширения псевдонимов</span><span class="sxs-lookup"><span data-stu-id="e2f33-158">Uninstall the alias extension</span></span>

<span data-ttu-id="e2f33-159">Удалите расширение с помощью команды [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="e2f33-159">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="e2f33-160">Если вы удалили расширение из-за ошибки или другой проблемы, [отправьте сообщение об этом на сайте GitHub](https://github.com/Azure/azure-cli-extensions/issues), чтобы мы реализовали исправление.</span><span class="sxs-lookup"><span data-stu-id="e2f33-160">If you uninstalled because a bug or other problem with the extension, [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>
