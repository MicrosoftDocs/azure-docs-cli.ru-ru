---
title: Советы по эффективному использованию Azure CLI
description: Советы по эффективному использованию Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 720e0866b97db0d56417db95f2518d5567836571
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563065"
---
# <a name="tips-for-using-azure-cli-effectively"></a>Советы по эффективному использованию Azure CLI

Сразу уточним, что во всем тексте используются скрипты Bash. В приложении вы найдете примеры пакетных файлов Windows и скриптов PowerShell, на основе которых можете легко создать аналогичные примеры.

## <a name="output-formatting-json-table-or-tsv"></a>Форматирование выходных данных (JSON, таблица или TSV)

1. Формат `json` по умолчанию используется в интерфейсе командной строки и предоставляет наиболее полные сведения. Если вы предпочитаете другой формат, с помощью аргумента `--output` переопределите формат для отдельного вызова или примените `az configure`, чтобы изменить глобальное значение по умолчанию. Обратите внимание, что в формате JSON сохраняются двойные кавычки. Это в большинстве случаев делает его непригодным для работы со скриптами.

2. Формат `table` полезен для получения сводки о конкретных параметрах, в частности для команд получения списков. Если вы не хотите использовать поля в формате таблицы по умолчанию (или формата по умолчанию нет), можете указать `--output json` для просмотра полной информации или `--query` для выбора нужного формата.

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. Формат `tsv` полезен для краткого вывода и работы со скриптами. В формате TSV удаляются двойные кавычки, которые сохраняются в формате JSON. Чтобы указать формат TSV, используйте аргумент `--query`.

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a>Передача значений из одной команды в другую

1. Если значение будет использоваться более одного раза, сохраните его в переменной. Обратите внимание, как применяется `-o tsv` в следующем примере:

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. Если значение используется только один раз, лучше использовать синтаксис конвейера:
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. Для списков учитывайте следующие рекомендации:

   Если вам важно точнее настроить результат, используйте цикл for:
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

    Также можно применить `xargs` и, при желании, флаг `-P` для параллельного выполнения операций для повышения производительности.
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    Наконец, Azure CLI имеет встроенную поддержку параллельного выполнения для команд с несколькими `--ids`. Это дает результат, аналогичный применению xargs. Обратите внимание, что для получения значений из конвейера используется `@-`:
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a>Асинхронные операции

Многие команды и группы поддерживают флаги `--no-wait` для длительных операций. Кроме того, есть отдельная команда `wait`. Эти механизмы полезны для нескольких сценариев:

1. Для очистки ресурсов, если вы не можете гарантировать выполнение какой-либо последующей операции, например удаления группы ресурсов:
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. Для создания нескольких независимых ресурсов в параллельном режиме. Это действует так же, как создание и присоединение потоков:

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a>Универсальные аргументы для обновления

Большинство команд обновления в CLI поддерживают три универсальных аргумента: `--add`, `--set` и `--remove`. Эти аргументы дают мощные возможности, но часто менее удобны, чем привычные для команд обновления строго типизированные аргументы. Интерфейс командной строки предоставляет строго типизированные аргументы для наиболее распространенных сценариев, где важна простота использования. Но если нужного вам свойства нет в списке, с помощью универсальных аргументов вы почти всегда сможете обойти такое ограничение, не дожидаясь нового выпуска.

1. Универсальный синтаксис обновления нельзя назвать самым удобным для пользователя. Для его применения потребуется немало терпения.
2. Проверьте, поддерживает ли для нужная команда обновления группу `Generic Update Arguments`. При наличии такой поддержки ее можно применить для решения поставленных задач. В противном случае придется оформить сообщение о проблеме.
3. Используйте команду `show` для нужного ресурса, чтобы выяснить путь для указания в универсальных аргументах. Например, перед попыткой применить `az vm update` выполните `az vm show`, чтобы определить правильный путь. Обычно для доступа к свойствам словаря используется синтаксис с точкой, а для обращения к элементам списка — квадратные скобки.
4. Чтобы было проще начать работу, изучите готовые рабочие примеры. Чтобы получить их, примените `az vm update -h`.
5. `--set` и `--add` принимают список пар "ключ — значение" в формате `<key1>=<value1> <key2>=<value2>`. Используйте их для создания нетипичных полезных данных. Если синтаксис получается слишком громоздкий, попробуйте перейти на формат строки JSON. Например, подключить новый диск данных к виртуальной машине можно так:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. Иногда будет удобнее использовать соглашение `@{file}` для CLI, помещая код JSON в файл и загружая его. Так, представленная выше команда упростится до следующей:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a>Универсальные команды для ресурсов — `az resource`

Иногда нужная служба не поддерживает команды CLI. Для работы с такими ресурсами можно использовать команды `az resource create/show/list/delete/update/invoke-action`. Вот несколько рекомендаций:
1. Если используются только команды `create/update`, можно применить `az group deployment create`. Изучите готовые [шаблоны быстрого запуска Azure](https://github.com/Azure/azure-quickstart-templates).
2. Ознакомьтесь с документацией по REST API, чтобы узнать формат полезных данных, URL-адрес и версию API для запроса. Для примера изучите комментарии сообщества по [созданию AppInsights](https://github.com/Azure/azure-cli/issues/5543).

## <a name="rest-api-command---az-rest"></a>Команда REST API — `az rest`

Если вам не подходят ни универсальные аргументы обновления, ни `az resource`, можно применить команду `az rest` для вызова REST API. Будет автоматически выполнена проверка подлинности с использованием учетных данных пользователя, вошедшего в систему, и установлен заголовок `Content-Type: application/json`.

Это очень полезно для вызова [API Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0), который сейчас не поддерживают команды интерфейса командной строки ([#12946](https://github.com/Azure/azure-cli/issues/12946)).

Например, чтобы обновить `redirectUris` для [приложения](/graph/api/resources/application?view=graph-rest-1.0), мы можем вызвать REST API [обновления приложения](/graph/api/application-update?view=graph-rest-1.0&tabs=http) следующим образом:

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

При использовании `--uri-parameters` для запросов в форме OData обязательно экранируйте `$`. В разных средах это делается так: в `Bash` символ `$` записывается как `\$`, а в `PowerShell` символ `$` записывается как `` `$``.

## <a name="quoting-issues"></a>Проблемы с кавычками

Эта проблема связана с тем, что при анализе команды CLI командная оболочка (Bash, Zsh, командная строка Windows, PowerShell и т. д.) преобразует кавычки и пробелы. Обязательно сверьтесь с соответствующей документацией, если вы не до конца разобрались с правилами использования оболочки:

- Bash: [Заключение в кавычки](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)
- PowerShell. [Сведения о правилах заключения в кавычки](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)
    - Из-за известной проблемы в PowerShell ([#1995](https://github.com/PowerShell/PowerShell/issues/1995)) применяется ряд дополнительных правил экранирования. Дополнительные сведения см. в статье [Проблемы с заключением в кавычки в PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).
- Командная строка Windows: [Практическое руководство. Escape-символы, разделители и кавычки в командной строке Windows](https://ss64.com/nt/syntax-esc.html)

Чтобы избежать непредвиденных результатов, соблюдайте несколько рекомендаций:

1. Если значение содержит пробелы, его необходимо заключить в кавычки.
2. В Bash и Windows PowerShell будут преобразованы одинарные и двойные кавычки. В командной строке Windows преобразуются только двойные кавычки, то есть одинарные кавычки считаются частью значения.
3. Если команда выполняется только на Bash (или Zsh), использование одинарных кавычек позволяет сохранить заключенное в них содержимое. Это может быть очень полезно при передаче встроенного кода JSON. Этот пример нормально работает в Bash: `'{"foo": "bar"}'`.
4. Если команда будет выполняться в командной строке Windows, следует использовать исключительно двойные кавычки. Если значение содержит двойные кавычки, их необходимо экранировать: `"i like to use \" a lot"`. Эквивалент этой команды для командной строки Windows: `"{\"foo\": \"bar\"}"`.
5. Экспортированные переменные в Bash, заключенные в двойные кавычки, будут оцениваться. Если это вам не нужно, также экранируйте их с помощью `\ `, как и для `"\$var"`, или используйте одинарные кавычки `'$var'`.
6. Несколько аргументов CLI, в том числе универсальные аргументы обновления, принимают список значений, разделенных пробелами, например `<key1>=<value1> <key2>=<value2>`. Так как имя и значение ключа могут содержать произвольную строку, в том числе с пробелами, потребуется использовать кавычки. Заключайте в кавычки всю пару, а не отдельно ключ и (или) значение. Так, запись `"my name"=john` ошибочна. Вместо этого используйте `"my name=john"`. Пример:
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. Используйте соглашение `@<file>` в CLI для загрузки данных из файла, чтобы обойти механизмы преобразования в оболочках:
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. Если для аргумента CLI указано, что он принимает список с разделителями-пробелами, принимаются следующие форматы:
    - `--arg foo bar`: Все в порядке. Список с разделителями-пробелами без кавычек
    - `--arg "foo" "bar"`: Хорошо. Список с разделителями-пробелами с кавычками
    - `--arg "foo bar"`: Плохо. Это строка с пробелом, а не список с разделителями-пробелами.
9. При выполнении команд Azure CLI в PowerShell могут возникать ошибки анализа, если аргументы содержат специальные символы PowerShell, как, например, `@`. Чтобы решить эту проблему, добавьте `` ` `` перед специальным символом, чтобы экранировать его, или заключите аргумент в одинарные либо двойные кавычки: `'`/`"`. Например, `az group deployment create --parameters @parameters.json` не работает в PowerShell, так как `@` воспринимается как [символ сплаттинга](/powershell/module/microsoft.powershell.core/about/about_splatting). Чтобы устранить эту проблему, вместо аргумента `` `@parameters.json`` используйте `'@parameters.json'`.
10. При использовании `--query` в команде некоторые символы [JMESPath](https://jmespath.org/specification.html) нужно экранировать от оболочки. Пример (bash):
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

    В командной строке:
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    В PowerShell (требуется дополнительное экранирование):
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

11. Лучший способ устранить проблему с кавычками — выполнить команду с флагом `--debug`. Отобразятся реальные полученные аргументы CLI с использованием синтаксиса [Python](https://docs.python.org/3/tutorial/introduction.html#strings). Пример (bash):

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

## <a name="work-behind-a-proxy"></a>Работа за прокси-сервером

Прокси-серверы часто встречаются в корпоративных сетях или добавляются средствами трассировки, как, например, Fiddler, mitmproxy и т. д. Если прокси-сервер использует самозаверяющие сертификаты, библиотека Python [Requests](https://github.com/kennethreitz/requests), которую использует интерфейс командной строки, создает исключение `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`. Есть два способа устранения этой ошибки:

1. В переменную среды `REQUESTS_CA_BUNDLE` поместите путь к файлу сертификатов из пакета ЦС в формате PEM. Это рекомендуемый вариант, если вы часто используете CLI за корпоративным прокси-сервером. По умолчанию CLI использует следующие пакеты ЦС: `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` в Windows и ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` в Linux. Вы можете добавить в этот файл сертификат прокси-сервера или скопировать его содержимое в другой файл сертификата, а затем сохранить путь к нему в переменной `REQUESTS_CA_BUNDLE`. Пример:

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   Часто возникает вопрос, нужно ли задавать переменные среды `HTTP_PROXY` или `HTTPS_PROXY`. Ответ на него может быть разным. Для Fiddler в Windows, который по умолчанию выступает в качестве системного прокси-сервера при запуске, ничего задавать не нужно. Если параметр отключен или используются другие средства, которые не выполняют функций системного прокси-сервера, переменные следует задать. Так как почти весь трафик из CLI передается по протоколу SSL, достаточно установить `HTTPS_PROXY`. Если вы не уверены, лучше установить их, но не забудьте удалить их после завершения работы прокси-сервера. Для Fiddler используется значение по умолчанию `http://localhost:8888`.

   Другие сведения см. в [блоге Стефана](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).

2. Отключите проверку сертификата в Azure CLI, задав переменную среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`. Это небезопасный вариант, но он может быть полезен на непродолжительное время, например для сбора трассировки сети по определенной команде, сразу после завершения которой эту переменную необходимо удалить. Это может не работать для некоторых команд уровня данных из-за ограничений базового пакета SDK.

## <a name="concurrent-builds"></a>Параллельные сборки

Если вы используете az на компьютере сборки и несколько заданий могут выполняться параллельно, есть риск того, что маркеры входа будут использоваться одновременно двумя заданиями сборки, так как эти задания выполняются от имени одного и того же пользователя ОС.  Чтобы избежать этого, сохраните в переменной AZURE_CONFIG_DIR путь к каталогу, в котором следует хранить маркеры входа.  Это может быть папка со случайным именем или имя рабочей области Jenkins, например: ```AZURE_CONFIG_DIR=.```.

## <a name="appendix"></a>Приложение

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a>Пакетные скрипты Windows для сохранения их в переменных и использования в будущем

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a>Скрипты Windows PowerShell для сохранения их в переменных и использования в будущем

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a>Пакетные скрипты Windows для циклического перебора списка
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a>Скрипты Windows PowerShell для циклического перебора списка
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a>Переменные среды CLI

|  Переменная среды          | Описание            |
|--------------------------------|------------------------|
| **AZURE_CONFIG_DIR**           | Глобальный каталог конфигурации для файлов конфигурации, журналов и телеметрии. Если значение не указано, по умолчанию используется `~/.azure`. |
| **AZURE_EXTENSION_DIR**        | Каталог установки расширений. Если не указано, по умолчанию используется каталог `cliextensions` в глобальном каталоге конфигурации. |
