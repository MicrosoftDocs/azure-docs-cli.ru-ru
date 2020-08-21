---
ms.openlocfilehash: 4794f1eb2fb45ca767f67de5270e232d6b68aede
ms.sourcegitcommit: 58d839589858acc1a7a9f114af7f4fce13d883ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "88601905"
---
# <a name="tips-for-using-azure-cli-effectively"></a><span data-ttu-id="dad26-101">Советы по эффективному использованию Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dad26-101">Tips for using Azure CLI effectively</span></span>

<span data-ttu-id="dad26-102">Сразу уточним, что во всем тексте используются скрипты Bash.</span><span class="sxs-lookup"><span data-stu-id="dad26-102">For clarity, Bash scripts are used inline.</span></span> <span data-ttu-id="dad26-103">В приложении вы найдете примеры пакетных файлов Windows и скриптов PowerShell, на основе которых можете легко создать аналогичные примеры.</span><span class="sxs-lookup"><span data-stu-id="dad26-103">Windows batch or PowerShell examples are listed in the appendix, which you can use to build similar examples.</span></span>

## <a name="output-formatting-json-table-or-tsv"></a><span data-ttu-id="dad26-104">Форматирование выходных данных (JSON, таблица или TSV)</span><span class="sxs-lookup"><span data-stu-id="dad26-104">Output formatting (json, table, or tsv)</span></span>

1. <span data-ttu-id="dad26-105">Формат `json` по умолчанию используется в интерфейсе командной строки и предоставляет наиболее полные сведения.</span><span class="sxs-lookup"><span data-stu-id="dad26-105">`json` format is the CLI's default, and is intended to give you the most comprehensive information.</span></span> <span data-ttu-id="dad26-106">Если вы предпочитаете другой формат, с помощью аргумента `--output` переопределите формат для отдельного вызова или примените `az configure`, чтобы изменить глобальное значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dad26-106">If you prefer a different format, use the `--output` argument to override for an individual command invocation, or use `az configure` to update your global default.</span></span> <span data-ttu-id="dad26-107">Обратите внимание, что в формате JSON сохраняются двойные кавычки. Это в большинстве случаев делает его непригодным для работы со скриптами.</span><span class="sxs-lookup"><span data-stu-id="dad26-107">Note that JSON format preserves the double quotes, generally making in unsuitable for scripting purposes.</span></span>

2. <span data-ttu-id="dad26-108">Формат `table` полезен для получения сводки о конкретных параметрах, в частности для команд получения списков.</span><span class="sxs-lookup"><span data-stu-id="dad26-108">`table` is useful for getting a summary of focused information, particularly for list commands.</span></span> <span data-ttu-id="dad26-109">Если вы не хотите использовать поля в формате таблицы по умолчанию (или формата по умолчанию нет), можете указать `--output json` для просмотра полной информации или `--query` для выбора нужного формата.</span><span class="sxs-lookup"><span data-stu-id="dad26-109">If you do not like the fields in the default table format (or there isn't a default format), you can use `--output json` to see all information, or leverage `--query` to specify a format you like.</span></span>

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. <span data-ttu-id="dad26-110">Формат `tsv` полезен для краткого вывода и работы со скриптами.</span><span class="sxs-lookup"><span data-stu-id="dad26-110">`tsv` is useful for concise output and scripting purposes.</span></span> <span data-ttu-id="dad26-111">В формате TSV удаляются двойные кавычки, которые сохраняются в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad26-111">The tsv will strip double quotes that the JSON format preserves.</span></span> <span data-ttu-id="dad26-112">Чтобы указать формат TSV, используйте аргумент `--query`.</span><span class="sxs-lookup"><span data-stu-id="dad26-112">To specify the format you want for TSV, use the `--query` argument.</span></span>

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a><span data-ttu-id="dad26-113">Передача значений из одной команды в другую</span><span class="sxs-lookup"><span data-stu-id="dad26-113">Pass values from one command to another</span></span>

1. <span data-ttu-id="dad26-114">Если значение будет использоваться более одного раза, сохраните его в переменной.</span><span class="sxs-lookup"><span data-stu-id="dad26-114">If the value will be used more than once, assign it to a variable.</span></span> <span data-ttu-id="dad26-115">Обратите внимание, как применяется `-o tsv` в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="dad26-115">Note the use of `-o tsv` in the following example:</span></span>

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. <span data-ttu-id="dad26-116">Если значение используется только один раз, лучше использовать синтаксис конвейера:</span><span class="sxs-lookup"><span data-stu-id="dad26-116">If the value is used only once, consider piping:</span></span>
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. <span data-ttu-id="dad26-117">Для списков учитывайте следующие рекомендации:</span><span class="sxs-lookup"><span data-stu-id="dad26-117">For lists consider the following suggestions:</span></span>

   <span data-ttu-id="dad26-118">Если вам важно точнее настроить результат, используйте цикл for:</span><span class="sxs-lookup"><span data-stu-id="dad26-118">If you need more controls on the result, use "for" loop:</span></span>
    ```sh
    #!/usr/bin/env bash
    for vm in $(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv); do
        echo stopping $vm
        az vm stop --ids $vm
        if [ $? -ne 0 ]; then
            echo "Failed to stop $vm"
            exit 1
        fi
        echo $vm stopped
    done
    ```

    <span data-ttu-id="dad26-119">Также можно применить `xargs` и, при желании, флаг `-P` для параллельного выполнения операций для повышения производительности.</span><span class="sxs-lookup"><span data-stu-id="dad26-119">Alternatively, use `xargs` and consider using the `-P` flag to run the operations in parallel for improved performance:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    <span data-ttu-id="dad26-120">Наконец, Azure CLI имеет встроенную поддержку параллельного выполнения для команд с несколькими `--ids`. Это дает результат, аналогичный применению xargs.</span><span class="sxs-lookup"><span data-stu-id="dad26-120">Finally, Azure CLI has built-in support to process commands with multiple `--ids` in parallel to achieve the same effect of xargs.</span></span> <span data-ttu-id="dad26-121">Обратите внимание, что для получения значений из конвейера используется `@-`:</span><span class="sxs-lookup"><span data-stu-id="dad26-121">Note that `@-` is used to get values from the pipe:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a><span data-ttu-id="dad26-122">Асинхронные операции</span><span class="sxs-lookup"><span data-stu-id="dad26-122">Async operations</span></span>

<span data-ttu-id="dad26-123">Многие команды и группы поддерживают флаги `--no-wait` для длительных операций. Кроме того, есть отдельная команда `wait`.</span><span class="sxs-lookup"><span data-stu-id="dad26-123">Many commands and group expose `--no-wait` flags on their long-running operations as well as a dedicated `wait` command.</span></span> <span data-ttu-id="dad26-124">Эти механизмы полезны для нескольких сценариев:</span><span class="sxs-lookup"><span data-stu-id="dad26-124">These become handy for certain scenarios:</span></span>

1. <span data-ttu-id="dad26-125">Для очистки ресурсов, если вы не можете гарантировать выполнение какой-либо последующей операции, например удаления группы ресурсов:</span><span class="sxs-lookup"><span data-stu-id="dad26-125">Cleaning up resources when you aren't relying on the clean up for some subsequent operation, such as deleting a resource group:</span></span>
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. <span data-ttu-id="dad26-126">Для создания нескольких независимых ресурсов в параллельном режиме.</span><span class="sxs-lookup"><span data-stu-id="dad26-126">When you want to create multiple independent resources in parallel.</span></span> <span data-ttu-id="dad26-127">Это действует так же, как создание и присоединение потоков:</span><span class="sxs-lookup"><span data-stu-id="dad26-127">This is similar to creating and joining threads:</span></span>

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a><span data-ttu-id="dad26-128">Универсальные аргументы для обновления</span><span class="sxs-lookup"><span data-stu-id="dad26-128">Generic update arguments</span></span>

<span data-ttu-id="dad26-129">Большинство команд обновления в CLI поддерживают три универсальных аргумента: `--add`, `--set` и `--remove`.</span><span class="sxs-lookup"><span data-stu-id="dad26-129">Most update commands in the CLI feature the three generic arguments: `--add`, `--set` and `--remove`.</span></span> <span data-ttu-id="dad26-130">Эти аргументы дают мощные возможности, но часто менее удобны, чем привычные для команд обновления строго типизированные аргументы.</span><span class="sxs-lookup"><span data-stu-id="dad26-130">These arguments are powerful but often less convenient than the strongly-typed arguments typically featured in update commands.</span></span> <span data-ttu-id="dad26-131">Интерфейс командной строки предоставляет строго типизированные аргументы для наиболее распространенных сценариев, где важна простота использования. Но если нужного вам свойства нет в списке, с помощью универсальных аргументов вы почти всегда сможете обойти такое ограничение, не дожидаясь нового выпуска.</span><span class="sxs-lookup"><span data-stu-id="dad26-131">The CLI provides strongly-typed arguments for most common scenarios for ease-of-use, but if the property you want to set isn't listed, the generic update arguments will often present a path forward to unblock you without having to wait for a new release.</span></span>

1. <span data-ttu-id="dad26-132">Универсальный синтаксис обновления нельзя назвать самым удобным для пользователя. Для его применения потребуется немало терпения.</span><span class="sxs-lookup"><span data-stu-id="dad26-132">The generic update syntax isn't the most user friendly, so it will require some patience.</span></span>
2. <span data-ttu-id="dad26-133">Проверьте, поддерживает ли для нужная команда обновления группу `Generic Update Arguments`.</span><span class="sxs-lookup"><span data-stu-id="dad26-133">Verify whether the update command has the `Generic Update Arguments` group exposed.</span></span> <span data-ttu-id="dad26-134">При наличии такой поддержки ее можно применить для решения поставленных задач. В противном случае придется оформить сообщение о проблеме.</span><span class="sxs-lookup"><span data-stu-id="dad26-134">If not, you'll need to file an issue, but if they are you can attempt you scenario using them.</span></span>
3. <span data-ttu-id="dad26-135">Используйте команду `show` для нужного ресурса, чтобы выяснить путь для указания в универсальных аргументах.</span><span class="sxs-lookup"><span data-stu-id="dad26-135">Use the `show` command on the resource you are interested in to figure out what path you should supply in the generic arguments.</span></span> <span data-ttu-id="dad26-136">Например, перед попыткой применить `az vm update` выполните `az vm show`, чтобы определить правильный путь.</span><span class="sxs-lookup"><span data-stu-id="dad26-136">For example, before you try out `az vm update`, run `az vm show` to determine the right path.</span></span> <span data-ttu-id="dad26-137">Обычно для доступа к свойствам словаря используется синтаксис с точкой, а для обращения к элементам списка — квадратные скобки.</span><span class="sxs-lookup"><span data-stu-id="dad26-137">Generally, you will use dot syntax to access dictionary properties and brackets to index into lists.</span></span>
4. <span data-ttu-id="dad26-138">Чтобы было проще начать работу, изучите готовые рабочие примеры.</span><span class="sxs-lookup"><span data-stu-id="dad26-138">Check out working examples to get started.</span></span> <span data-ttu-id="dad26-139">Чтобы получить их, примените `az vm update -h`.</span><span class="sxs-lookup"><span data-stu-id="dad26-139">`az vm update -h` has good ones.</span></span>
5. <span data-ttu-id="dad26-140">`--set` и `--add` принимают список пар "ключ — значение" в формате `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="dad26-140">`--set` and `--add` take a list of key value pairs in the format of `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="dad26-141">Используйте их для создания нетипичных полезных данных.</span><span class="sxs-lookup"><span data-stu-id="dad26-141">Use them to construct non- trivial payloads.</span></span> <span data-ttu-id="dad26-142">Если синтаксис получается слишком громоздкий, попробуйте перейти на формат строки JSON.</span><span class="sxs-lookup"><span data-stu-id="dad26-142">If the syntax gets too message, consider using a JSON string.</span></span> <span data-ttu-id="dad26-143">Например, подключить новый диск данных к виртуальной машине можно так:</span><span class="sxs-lookup"><span data-stu-id="dad26-143">For example, to attach a new data disk to a VM:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. <span data-ttu-id="dad26-144">Иногда будет удобнее использовать соглашение `@{file}` для CLI, помещая код JSON в файл и загружая его.</span><span class="sxs-lookup"><span data-stu-id="dad26-144">You may find it more useful to leverage the CLI's `@{file}` convention, putting the JSON into a file and loading it.</span></span> <span data-ttu-id="dad26-145">Так, представленная выше команда упростится до следующей:</span><span class="sxs-lookup"><span data-stu-id="dad26-145">This simplifies the above command to:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a><span data-ttu-id="dad26-146">Универсальные команды для ресурсов — `az resource`</span><span class="sxs-lookup"><span data-stu-id="dad26-146">Generic resource commands - `az resource`</span></span>

<span data-ttu-id="dad26-147">Иногда нужная служба не поддерживает команды CLI.</span><span class="sxs-lookup"><span data-stu-id="dad26-147">There may be cases where a service you are interested in does not have CLI command coverage.</span></span> <span data-ttu-id="dad26-148">Для работы с такими ресурсами можно использовать команды `az resource create/show/list/delete/update/invoke-action`.</span><span class="sxs-lookup"><span data-stu-id="dad26-148">You can use the `az resource create/show/list/delete/update/invoke-action` commands to work with these resources.</span></span> <span data-ttu-id="dad26-149">Вот несколько рекомендаций:</span><span class="sxs-lookup"><span data-stu-id="dad26-149">Here are a few suggestions:</span></span>
1. <span data-ttu-id="dad26-150">Если используются только команды `create/update`, можно применить `az group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="dad26-150">If only `create/update` are involved, consider using `az group deployment create`.</span></span> <span data-ttu-id="dad26-151">Изучите готовые [шаблоны быстрого запуска Azure](https://github.com/Azure/azure-quickstart-templates).</span><span class="sxs-lookup"><span data-stu-id="dad26-151">Leverage [Azure Quickstart Templates](https://github.com/Azure/azure-quickstart-templates) for working examples.</span></span>
2. <span data-ttu-id="dad26-152">Ознакомьтесь с документацией по REST API, чтобы узнать формат полезных данных, URL-адрес и версию API для запроса.</span><span class="sxs-lookup"><span data-stu-id="dad26-152">Check out the Rest API reference for the request payload, URL and API version.</span></span> <span data-ttu-id="dad26-153">Для примера изучите комментарии сообщества по [созданию AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span><span class="sxs-lookup"><span data-stu-id="dad26-153">As an example, check out the community's comments on [how to create AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span></span>

## <a name="rest-api-command---az-rest"></a><span data-ttu-id="dad26-154">Команда REST API — `az rest`</span><span class="sxs-lookup"><span data-stu-id="dad26-154">REST API command - `az rest`</span></span>

<span data-ttu-id="dad26-155">Если вам не подходят ни универсальные аргументы обновления, ни `az resource`, можно применить команду `az rest` для вызова REST API.</span><span class="sxs-lookup"><span data-stu-id="dad26-155">If neither generic update arguments nor `az resource` meets your needs, you can use `az rest` command to call the REST API.</span></span> <span data-ttu-id="dad26-156">Будет автоматически выполнена проверка подлинности с использованием учетных данных пользователя, вошедшего в систему, и установлен заголовок `Content-Type: application/json`.</span><span class="sxs-lookup"><span data-stu-id="dad26-156">It automatically authenticates using the logged-in credential and sets header `Content-Type: application/json`.</span></span>

<span data-ttu-id="dad26-157">Это очень полезно для вызова [API Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0), который сейчас не поддерживают команды интерфейса командной строки ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span><span class="sxs-lookup"><span data-stu-id="dad26-157">This is extremely useful for calling [Microsoft Graph API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) which is not currently supported by CLI commands ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span></span>

<span data-ttu-id="dad26-158">Например, чтобы обновить `redirectUris` для [приложения](/graph/api/resources/application?view=graph-rest-1.0), мы можем вызвать REST API [обновления приложения](/graph/api/application-update?view=graph-rest-1.0&tabs=http) следующим образом:</span><span class="sxs-lookup"><span data-stu-id="dad26-158">For example, to update `redirectUris` for an [Application](/graph/api/resources/application?view=graph-rest-1.0), we call the [Update application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) REST API with:</span></span>

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --url 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --url 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

<span data-ttu-id="dad26-159">При использовании `--url-parameters` для запросов в форме OData обязательно экранируйте `$`. В разных средах это делается так: в `Bash` символ `$` записывается как `\$`, а в `PowerShell` символ `$` записывается как `` `$``.</span><span class="sxs-lookup"><span data-stu-id="dad26-159">When using `--url-parameters` for requests in the form of OData, please make sure to escape `$` in different environments: in `Bash`, escape `$` as `\$` and in `PowerShell`, escape `$` as `` `$``</span></span>

## <a name="quoting-issues"></a><span data-ttu-id="dad26-160">Проблемы с кавычками</span><span class="sxs-lookup"><span data-stu-id="dad26-160">Quoting issues</span></span>

<span data-ttu-id="dad26-161">Эта проблема связана с тем, что при анализе команды CLI командная оболочка (Bash, Zsh, командная строка Windows, PowerShell и т. д.) преобразует кавычки и пробелы.</span><span class="sxs-lookup"><span data-stu-id="dad26-161">This becomes an issue because when the command shell (Bash, Zsh, Windows Command Prompt, PowerShell, etc) parses the CLI command, it will interpret the quotes and spaces.</span></span> <span data-ttu-id="dad26-162">Обязательно сверьтесь с соответствующей документацией, если вы не до конца разобрались с правилами использования оболочки:</span><span class="sxs-lookup"><span data-stu-id="dad26-162">Always refer to the documents when you are uncertain about the usage of a shell:</span></span>

- <span data-ttu-id="dad26-163">Bash: [Заключение в кавычки](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span><span class="sxs-lookup"><span data-stu-id="dad26-163">Bash: [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span></span>
- <span data-ttu-id="dad26-164">PowerShell. [Сведения о правилах заключения в кавычки](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span><span class="sxs-lookup"><span data-stu-id="dad26-164">PowerShell: [About Quoting Rules](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span></span>
    - <span data-ttu-id="dad26-165">Из-за известной проблемы в PowerShell ([#1995](https://github.com/PowerShell/PowerShell/issues/1995)) применяется ряд дополнительных правил экранирования.</span><span class="sxs-lookup"><span data-stu-id="dad26-165">Due to a known issue [#1995](https://github.com/PowerShell/PowerShell/issues/1995) of PowerShell, some extra escaping rules apply.</span></span> <span data-ttu-id="dad26-166">Дополнительные сведения см. в статье [Проблемы с заключением в кавычки в PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).</span><span class="sxs-lookup"><span data-stu-id="dad26-166">See [Quoting issues with PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) for more information.</span></span>
- <span data-ttu-id="dad26-167">Командная строка Windows: [Практическое руководство. Escape-символы, разделители и кавычки в командной строке Windows](https://ss64.com/nt/syntax-esc.html)</span><span class="sxs-lookup"><span data-stu-id="dad26-167">Windows Command Prompt: [How-to: Escape Characters, Delimiters and Quotes at the Windows command line](https://ss64.com/nt/syntax-esc.html)</span></span>

<span data-ttu-id="dad26-168">Чтобы избежать непредвиденных результатов, соблюдайте несколько рекомендаций:</span><span class="sxs-lookup"><span data-stu-id="dad26-168">To avoid unanticipated results, here are a few suggestions:</span></span>

1. <span data-ttu-id="dad26-169">Если значение содержит пробелы, его необходимо заключить в кавычки.</span><span class="sxs-lookup"><span data-stu-id="dad26-169">If the value contains whitespace, you must wrap it in quotes.</span></span>
2. <span data-ttu-id="dad26-170">В Bash и Windows PowerShell будут преобразованы одинарные и двойные кавычки. В командной строке Windows преобразуются только двойные кавычки, то есть одинарные кавычки считаются частью значения.</span><span class="sxs-lookup"><span data-stu-id="dad26-170">In bash or Windows PowerShell, both single and double quotes will be interpreted, while in Windows Command Prompt, only double quotes are handled which means single quotes will be interpreted as a part of the value.</span></span>
3. <span data-ttu-id="dad26-171">Если команда выполняется только на Bash (или Zsh), использование одинарных кавычек позволяет сохранить заключенное в них содержимое.</span><span class="sxs-lookup"><span data-stu-id="dad26-171">If your command only runs on Bash (or Zsh), using single quotes has the benefit of preserving the content inside.</span></span> <span data-ttu-id="dad26-172">Это может быть очень полезно при передаче встроенного кода JSON.</span><span class="sxs-lookup"><span data-stu-id="dad26-172">This can be very helpful when supplying inline JSON.</span></span> <span data-ttu-id="dad26-173">Этот пример нормально работает в Bash: `'{"foo": "bar"}'`.</span><span class="sxs-lookup"><span data-stu-id="dad26-173">For example this works in bash: `'{"foo": "bar"}'`</span></span>
4. <span data-ttu-id="dad26-174">Если команда будет выполняться в командной строке Windows, следует использовать исключительно двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="dad26-174">If your command will run on Windows Command Prompt, you must use double quotes exclusively.</span></span> <span data-ttu-id="dad26-175">Если значение содержит двойные кавычки, их необходимо экранировать: `"i like to use \" a lot"`.</span><span class="sxs-lookup"><span data-stu-id="dad26-175">If the value contains double quotes, you must escape it: `"i like to use \" a lot"`.</span></span> <span data-ttu-id="dad26-176">Эквивалент этой команды для командной строки Windows: `"{\"foo\": \"bar\"}"`.</span><span class="sxs-lookup"><span data-stu-id="dad26-176">The Command Prompt equivalent of the above would be: `"{\"foo\": \"bar\"}"`</span></span>
5. <span data-ttu-id="dad26-177">Экспортированные переменные в Bash, заключенные в двойные кавычки, будут оцениваться.</span><span class="sxs-lookup"><span data-stu-id="dad26-177">Exported variables in bash inside double quotes will be evaluated.</span></span> <span data-ttu-id="dad26-178">Если это вам не нужно, также экранируйте их с помощью `\ `, как и для `"\$var"`, или используйте одинарные кавычки `'$var'`.</span><span class="sxs-lookup"><span data-stu-id="dad26-178">If this is not what you want, again use `\ ` to escape it like `"\$var"` or use single quotes `'$var'`.</span></span>
6. <span data-ttu-id="dad26-179">Несколько аргументов CLI, в том числе универсальные аргументы обновления, принимают список значений, разделенных пробелами, например `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="dad26-179">A few CLI arguments, including the generic update arguments, take a list of space-separated values, like `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="dad26-180">Так как имя и значение ключа могут содержать произвольную строку, в том числе с пробелами, потребуется использовать кавычки.</span><span class="sxs-lookup"><span data-stu-id="dad26-180">Since the key name and value can take arbitrary string which might contain whitespace, using quotes will be necessary.</span></span> <span data-ttu-id="dad26-181">Заключайте в кавычки всю пару, а не отдельно ключ и (или) значение.</span><span class="sxs-lookup"><span data-stu-id="dad26-181">Wrap the pair, not individual key or value.</span></span> <span data-ttu-id="dad26-182">Так, запись `"my name"=john` ошибочна.</span><span class="sxs-lookup"><span data-stu-id="dad26-182">So `"my name"=john` is wrong.</span></span> <span data-ttu-id="dad26-183">Вместо этого используйте `"my name=john"`.</span><span class="sxs-lookup"><span data-stu-id="dad26-183">Instead, use `"my name=john"`.</span></span> <span data-ttu-id="dad26-184">Пример:</span><span class="sxs-lookup"><span data-stu-id="dad26-184">For example:</span></span>
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. <span data-ttu-id="dad26-185">Используйте соглашение `@<file>` в CLI для загрузки данных из файла, чтобы обойти механизмы преобразования в оболочках:</span><span class="sxs-lookup"><span data-stu-id="dad26-185">Use CLI's `@<file>` convention to load from a file so to bypass the shell's interpretation mechanisms:</span></span>
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. <span data-ttu-id="dad26-186">Если для аргумента CLI указано, что он принимает список с разделителями-пробелами, принимаются следующие форматы:</span><span class="sxs-lookup"><span data-stu-id="dad26-186">When a CLI argument says it accepts a space-separated list, these are the formats accepted:</span></span>
    - <span data-ttu-id="dad26-187">`--arg foo bar`: Все в порядке.</span><span class="sxs-lookup"><span data-stu-id="dad26-187">`--arg foo bar`: OK.</span></span> <span data-ttu-id="dad26-188">Список с разделителями-пробелами без кавычек</span><span class="sxs-lookup"><span data-stu-id="dad26-188">Unquoted, space-separated list</span></span>
    - <span data-ttu-id="dad26-189">`--arg "foo" "bar"`: Хорошо. Список с разделителями-пробелами с кавычками</span><span class="sxs-lookup"><span data-stu-id="dad26-189">`--arg "foo" "bar"`: OK: Quoted, space-separated list</span></span>
    - <span data-ttu-id="dad26-190">`--arg "foo bar"`: Плохо.</span><span class="sxs-lookup"><span data-stu-id="dad26-190">`--arg "foo bar"`: BAD.</span></span> <span data-ttu-id="dad26-191">Это строка с пробелом, а не список с разделителями-пробелами.</span><span class="sxs-lookup"><span data-stu-id="dad26-191">This is a string with a space in it, not a space-separated list.</span></span>
9. <span data-ttu-id="dad26-192">При выполнении команд Azure CLI в PowerShell могут возникать ошибки анализа, если аргументы содержат специальные символы PowerShell, как, например, `@`.</span><span class="sxs-lookup"><span data-stu-id="dad26-192">When running Azure CLI commands in PowerShell, parsing errors will occur when the arguments contain special characters of PowerShell, such as at `@`.</span></span> <span data-ttu-id="dad26-193">Чтобы решить эту проблему, добавьте `` ` `` перед специальным символом, чтобы экранировать его, или заключите аргумент в одинарные либо двойные кавычки: `'`/`"`.</span><span class="sxs-lookup"><span data-stu-id="dad26-193">You can solve this problem by adding `` ` `` before the special character to escape it, or by enclosing the argument with single or double quotes `'`/`"`.</span></span> <span data-ttu-id="dad26-194">Например, `az group deployment create --parameters @parameters.json` не работает в PowerShell, так как `@` воспринимается как [символ сплаттинга](/powershell/module/microsoft.powershell.core/about/about_splatting).</span><span class="sxs-lookup"><span data-stu-id="dad26-194">For example, `az group deployment create --parameters @parameters.json` doesn't work in PowerShell because `@` is parsed as a [splatting symbol](/powershell/module/microsoft.powershell.core/about/about_splatting).</span></span> <span data-ttu-id="dad26-195">Чтобы устранить эту проблему, вместо аргумента `` `@parameters.json`` используйте `'@parameters.json'`.</span><span class="sxs-lookup"><span data-stu-id="dad26-195">To fix this, you may change the argument to `` `@parameters.json`` or `'@parameters.json'`.</span></span>
10. <span data-ttu-id="dad26-196">При использовании `--query` в команде некоторые символы [JMESPath](https://jmespath.org/specification.html) нужно экранировать от оболочки.</span><span class="sxs-lookup"><span data-stu-id="dad26-196">When using `--query` with a command, some characters of [JMESPath](https://jmespath.org/specification.html) need to be escaped in the shell.</span></span> <span data-ttu-id="dad26-197">Пример (bash):</span><span class="sxs-lookup"><span data-stu-id="dad26-197">For example, in Bash:</span></span>
    ```sh
    # Wrong, as the dash needs to be quoted in a JMESPath query
    $ az version --query azure-cli
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Wrong, as the dash needs to be quoted in a JMESPath query, but quotes are interpreted by Bash
    $ az version --query "azure-cli"
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Correct
    $ az version --query '"azure-cli"'
    "2.5.1"

    $ az version --query \"azure-cli\"
    "2.5.1"

    $ az version --query "\"azure-cli\""
    "2.5.1"
    ```

    <span data-ttu-id="dad26-198">В командной строке:</span><span class="sxs-lookup"><span data-stu-id="dad26-198">In Command Prompt:</span></span>
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    <span data-ttu-id="dad26-199">В PowerShell (требуется дополнительное экранирование):</span><span class="sxs-lookup"><span data-stu-id="dad26-199">In PowerShell (extra escaping is needed):</span></span>
    ```powershell
    > az version --query '\"azure-cli\"'
    "2.5.1"

    > az version --query "\`"azure-cli\`""
    "2.5.1"

    > az version --query "\""azure-cli\"""
    "2.5.1"

    > az --% version --query "\"azure-cli\""
    "2.5.1"

    > az --% version --query \"azure-cli\"
    "2.5.1"
    ```

11. <span data-ttu-id="dad26-200">Лучший способ устранить проблему с кавычками — выполнить команду с флагом `--debug`.</span><span class="sxs-lookup"><span data-stu-id="dad26-200">The best way to troubleshoot a quoting issue is to run the command with `--debug` flag.</span></span> <span data-ttu-id="dad26-201">Отобразятся реальные полученные аргументы CLI с использованием синтаксиса [Python](https://docs.python.org/3/tutorial/introduction.html#strings).</span><span class="sxs-lookup"><span data-stu-id="dad26-201">It reveals the actual arguments received by CLI in [Python's syntax](https://docs.python.org/3/tutorial/introduction.html#strings).</span></span> <span data-ttu-id="dad26-202">Пример (bash):</span><span class="sxs-lookup"><span data-stu-id="dad26-202">For example, in Bash:</span></span>

    ```sh
    # Wrong, as quotes and spaces are interpreted by Bash
    $ az {"key": "value"} --debug
    Command arguments: ['{key:', 'value}', '--debug']

    # Wrong, as quotes are interpreted by Bash
    $ az {"key":"value"} --debug
    Command arguments: ['{key:value}', '--debug']

    # Correct
    $ az '{"key":"value"}' --debug
    Command arguments: ['{"key":"value"}', '--debug']

    # Correct
    $ az "{\"key\":\"value\"}" --debug
    Command arguments: ['{"key":"value"}', '--debug']
    ```

## <a name="work-behind-a-proxy"></a><span data-ttu-id="dad26-203">Работа за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="dad26-203">Work behind a proxy</span></span>

<span data-ttu-id="dad26-204">Прокси-серверы часто встречаются в корпоративных сетях или добавляются средствами трассировки, как, например, Fiddler, mitmproxy и т. д. Если прокси-сервер использует самозаверяющие сертификаты, библиотека Python [Requests](https://github.com/kennethreitz/requests), которую использует интерфейс командной строки, создает исключение `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span><span class="sxs-lookup"><span data-stu-id="dad26-204">Proxy is common behind corporate network or introduced by tracing tools like Fiddler, mitmproxy, etc. If the proxy uses self-signed certificates, the Python [Requests](https://github.com/kennethreitz/requests) library which CLI uses will throw `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span></span> <span data-ttu-id="dad26-205">Есть два способа устранения этой ошибки:</span><span class="sxs-lookup"><span data-stu-id="dad26-205">There are 2 ways to handle this error:</span></span>

1. <span data-ttu-id="dad26-206">В переменную среды `REQUESTS_CA_BUNDLE` поместите путь к файлу сертификатов из пакета ЦС в формате PEM.</span><span class="sxs-lookup"><span data-stu-id="dad26-206">Set environment variable `REQUESTS_CA_BUNDLE` to the path of CA bundle certificate file in PEM format.</span></span> <span data-ttu-id="dad26-207">Это рекомендуемый вариант, если вы часто используете CLI за корпоративным прокси-сервером.</span><span class="sxs-lookup"><span data-stu-id="dad26-207">This is recommended if you use CLI frequently behind a corporate proxy.</span></span> <span data-ttu-id="dad26-208">По умолчанию CLI использует следующие пакеты ЦС: `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` в Windows и ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` в Linux.</span><span class="sxs-lookup"><span data-stu-id="dad26-208">The default CA bundle which CLI uses is located at `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` on Windows and ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` on Linux.</span></span> <span data-ttu-id="dad26-209">Вы можете добавить в этот файл сертификат прокси-сервера или скопировать его содержимое в другой файл сертификата, а затем сохранить путь к нему в переменной `REQUESTS_CA_BUNDLE`.</span><span class="sxs-lookup"><span data-stu-id="dad26-209">You may append the proxy server's certificate to this file or copy the contents to another certificate file, then set `REQUESTS_CA_BUNDLE` to it.</span></span> <span data-ttu-id="dad26-210">Пример:</span><span class="sxs-lookup"><span data-stu-id="dad26-210">For example:</span></span>

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   <span data-ttu-id="dad26-211">Часто возникает вопрос, нужно ли задавать переменные среды `HTTP_PROXY` или `HTTPS_PROXY`. Ответ на него может быть разным.</span><span class="sxs-lookup"><span data-stu-id="dad26-211">A frequent ask is whether or not `HTTP_PROXY` or `HTTPS_PROXY` environment variables should be set, the answer is it depends.</span></span> <span data-ttu-id="dad26-212">Для Fiddler в Windows, который по умолчанию выступает в качестве системного прокси-сервера при запуске, ничего задавать не нужно.</span><span class="sxs-lookup"><span data-stu-id="dad26-212">For Fiddler on Windows, by default it acts as system proxy on start, you don't need to set anything.</span></span> <span data-ttu-id="dad26-213">Если параметр отключен или используются другие средства, которые не выполняют функций системного прокси-сервера, переменные следует задать.</span><span class="sxs-lookup"><span data-stu-id="dad26-213">If the option is off or using other tools which don't work as system proxy, you should set them.</span></span> <span data-ttu-id="dad26-214">Так как почти весь трафик из CLI передается по протоколу SSL, достаточно установить `HTTPS_PROXY`.</span><span class="sxs-lookup"><span data-stu-id="dad26-214">Since almost all traffic from CLI is SSL-based, only `HTTPS_PROXY` should be set.</span></span> <span data-ttu-id="dad26-215">Если вы не уверены, лучше установить их, но не забудьте удалить их после завершения работы прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="dad26-215">If you are not sure, just set them, but do remember to unset it after the proxy is shut down.</span></span> <span data-ttu-id="dad26-216">Для Fiddler используется значение по умолчанию `http://localhost:8888`.</span><span class="sxs-lookup"><span data-stu-id="dad26-216">For fiddler, the default value is `http://localhost:8888`.</span></span>

   <span data-ttu-id="dad26-217">Другие сведения см. в [блоге Стефана](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span><span class="sxs-lookup"><span data-stu-id="dad26-217">For other details, check out [Stefan's blog](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span></span>

2. <span data-ttu-id="dad26-218">Отключите проверку сертификата в Azure CLI, задав переменную среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span><span class="sxs-lookup"><span data-stu-id="dad26-218">Disable the certificate check across Azure CLI by setting environment variable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span></span> <span data-ttu-id="dad26-219">Это небезопасный вариант, но он может быть полезен на непродолжительное время, например для сбора трассировки сети по определенной команде, сразу после завершения которой эту переменную необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="dad26-219">This is not safe, but good for a short period like capturing a network trace for a specific command and promptly turning it off when finished.</span></span> <span data-ttu-id="dad26-220">Это может не работать для некоторых команд уровня данных из-за ограничений базового пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="dad26-220">This may not work for some data-plane commands due to underlying SDK limitations.</span></span>

## <a name="concurrent-builds"></a><span data-ttu-id="dad26-221">Параллельные сборки</span><span class="sxs-lookup"><span data-stu-id="dad26-221">Concurrent builds</span></span>

<span data-ttu-id="dad26-222">Если вы используете az на компьютере сборки и несколько заданий могут выполняться параллельно, есть риск того, что маркеры входа будут использоваться одновременно двумя заданиями сборки, так как эти задания выполняются от имени одного и того же пользователя ОС.</span><span class="sxs-lookup"><span data-stu-id="dad26-222">If you are using az on a build machine, and multiple jobs can be run in parallel, then there is a risk that the login tokens are shared between two build jobs is the jobs run as the same OS user.</span></span>  <span data-ttu-id="dad26-223">Чтобы избежать этого, сохраните в переменной AZURE_CONFIG_DIR путь к каталогу, в котором следует хранить маркеры входа.</span><span class="sxs-lookup"><span data-stu-id="dad26-223">To avoid mix ups like this, set AZURE_CONFIG_DIR to a directory where the login tokens should be stored.</span></span>  <span data-ttu-id="dad26-224">Это может быть папка со случайным именем или имя рабочей области Jenkins, например: ```AZURE_CONFIG_DIR=.```.</span><span class="sxs-lookup"><span data-stu-id="dad26-224">It could be a randomly created folder, or just the name of the jenkins workspace, like this ```AZURE_CONFIG_DIR=.```</span></span>

## <a name="appendix"></a><span data-ttu-id="dad26-225">Приложение</span><span class="sxs-lookup"><span data-stu-id="dad26-225">Appendix</span></span>

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="dad26-226">Пакетные скрипты Windows для сохранения их в переменных и использования в будущем</span><span class="sxs-lookup"><span data-stu-id="dad26-226">Windows batch scripts for saving to variables and using it later</span></span>

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="dad26-227">Скрипты Windows PowerShell для сохранения их в переменных и использования в будущем</span><span class="sxs-lookup"><span data-stu-id="dad26-227">Windows PowerShell scripts for saving to variables and using it later</span></span>

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a><span data-ttu-id="dad26-228">Пакетные скрипты Windows для циклического перебора списка</span><span class="sxs-lookup"><span data-stu-id="dad26-228">Windows batch scripts to loop through a list</span></span>
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a><span data-ttu-id="dad26-229">Скрипты Windows PowerShell для циклического перебора списка</span><span class="sxs-lookup"><span data-stu-id="dad26-229">Windows PowerShell scripts to loop through a list</span></span>
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a><span data-ttu-id="dad26-230">Переменные среды CLI</span><span class="sxs-lookup"><span data-stu-id="dad26-230">CLI Environment Variables</span></span>

|  <span data-ttu-id="dad26-231">Переменная среды</span><span class="sxs-lookup"><span data-stu-id="dad26-231">Environment Variable</span></span>          | <span data-ttu-id="dad26-232">Описание</span><span class="sxs-lookup"><span data-stu-id="dad26-232">Description</span></span>            |
|--------------------------------|------------------------|
| <span data-ttu-id="dad26-233">**AZURE_CONFIG_DIR**</span><span class="sxs-lookup"><span data-stu-id="dad26-233">**AZURE_CONFIG_DIR**</span></span>           | <span data-ttu-id="dad26-234">Глобальный каталог конфигурации для файлов конфигурации, журналов и телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dad26-234">Global config directory for config files, logs and telemetry.</span></span> <span data-ttu-id="dad26-235">Если значение не указано, по умолчанию используется `~/.azure`.</span><span class="sxs-lookup"><span data-stu-id="dad26-235">If unspecified, defaults to `~/.azure`.</span></span> |
| <span data-ttu-id="dad26-236">**AZURE_EXTENSION_DIR**</span><span class="sxs-lookup"><span data-stu-id="dad26-236">**AZURE_EXTENSION_DIR**</span></span>        | <span data-ttu-id="dad26-237">Каталог установки расширений.</span><span class="sxs-lookup"><span data-stu-id="dad26-237">Extensions' installation directory.</span></span> <span data-ttu-id="dad26-238">Если не указано, по умолчанию используется каталог `cliextensions` в глобальном каталоге конфигурации.</span><span class="sxs-lookup"><span data-stu-id="dad26-238">If unspecified, defaults to `cliextensions` directory within the global config directory.</span></span> |
