---
title: Запросы результатов команд в Azure CLI
description: Сведения о том, как выполнять запросы JMESPath к результатам команд Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c9f0afdd626ac8d9af027db02275e5a553595473
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "77780083"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="d4788-103">Запросы к выходным данным команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d4788-103">Query Azure CLI command output</span></span>

<span data-ttu-id="d4788-104">Интерфейс Azure CLI использует аргумент `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команд.</span><span class="sxs-lookup"><span data-stu-id="d4788-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="d4788-105">JMESPath — это язык запросов для JSON, который позволяет выбирать и изменять выходные данные команд CLI.</span><span class="sxs-lookup"><span data-stu-id="d4788-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="d4788-106">Запросы выполняются к выходным данным в формате JSON до их форматирования для отображения.</span><span class="sxs-lookup"><span data-stu-id="d4788-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="d4788-107">Аргумент `--query` поддерживается всеми командами в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="d4788-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="d4788-108">В этой статье описано использование возможностей JMESPath на основе ряда небольших простых примеров.</span><span class="sxs-lookup"><span data-stu-id="d4788-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="d4788-109">Результаты команд CLI в виде словарей и списков</span><span class="sxs-lookup"><span data-stu-id="d4788-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="d4788-110">Даже если используется формат выходных данных, отличный от JSON, при выполнении запросов результаты выполнения команд сначала обрабатываются как объекты JSON.</span><span class="sxs-lookup"><span data-stu-id="d4788-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="d4788-111">Результаты выполнения команд CLI представляют собой массив или словарь JSON.</span><span class="sxs-lookup"><span data-stu-id="d4788-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="d4788-112">Массивы — это последовательности объектов, доступ к которым может осуществляться по индексу, а словари — это неупорядоченные объекты, доступ к которым осуществляется с помощью ключей.</span><span class="sxs-lookup"><span data-stu-id="d4788-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="d4788-113">Команды, которые _могут_ возвращать несколько объектов, возвращают массив, а команды, которые _всегда_ возвращают _только_ один объект, возвращают его в виде словаря.</span><span class="sxs-lookup"><span data-stu-id="d4788-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="d4788-114">Получение свойств из словаря</span><span class="sxs-lookup"><span data-stu-id="d4788-114">Get properties in a dictionary</span></span>

<span data-ttu-id="d4788-115">При работе с результатами в виде словаря вы всегда можете получить свойства верхнего уровня с помощью ключа.</span><span class="sxs-lookup"><span data-stu-id="d4788-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="d4788-116">Для доступа к свойствам вложенных словарей используется символ `.` (__часть выражения__).</span><span class="sxs-lookup"><span data-stu-id="d4788-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="d4788-117">Прежде чем перейти к запросам, рассмотрим неизмененные выходные данные команды `az vm show`:</span><span class="sxs-lookup"><span data-stu-id="d4788-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="d4788-118">Результаты этой команда выводятся в виде словаря.</span><span class="sxs-lookup"><span data-stu-id="d4788-118">The command will output a dictionary.</span></span> <span data-ttu-id="d4788-119">Часть содержимого опущена.</span><span class="sxs-lookup"><span data-stu-id="d4788-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="d4788-120">Следующая команда предназначена для получения открытых ключей SSH, имеющих разрешение на подключение к виртуальной машине, с помощью запроса:</span><span class="sxs-lookup"><span data-stu-id="d4788-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

## <a name="get-a-single-value"></a><span data-ttu-id="d4788-121">Получение одного значения</span><span class="sxs-lookup"><span data-stu-id="d4788-121">Get a single value</span></span>

<span data-ttu-id="d4788-122">Часто нужно, чтобы команда CLI должна вернуть только _одно_ значение, например идентификатор ресурса Azure, имя ресурса, имя пользователя или пароль.</span><span class="sxs-lookup"><span data-stu-id="d4788-122">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="d4788-123">При этом значение должно быть сохранено в локальной переменной.</span><span class="sxs-lookup"><span data-stu-id="d4788-123">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="d4788-124">Чтобы получить одно свойство, сначала убедитесь, что вам удалось извлечь только одно свойство из запроса.</span><span class="sxs-lookup"><span data-stu-id="d4788-124">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="d4788-125">В последнем примере показано, как получить только имя пользователя администратора:</span><span class="sxs-lookup"><span data-stu-id="d4788-125">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="d4788-126">Оно выглядит как допустимое отдельное значение, но обратите внимание, что символы `"` возвращаются как часть выходных данных.</span><span class="sxs-lookup"><span data-stu-id="d4788-126">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="d4788-127">Это означает, что объект представляет собой строку JSON.</span><span class="sxs-lookup"><span data-stu-id="d4788-127">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="d4788-128">Важно отметить, что при назначении этого значения переменной среды непосредственно в качестве выходных данных команды, кавычки могут __не__ интерпретироваться оболочкой:</span><span class="sxs-lookup"><span data-stu-id="d4788-128">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="d4788-129">Это явно не то, что нужно.</span><span class="sxs-lookup"><span data-stu-id="d4788-129">This is almost certainly not what you want.</span></span> <span data-ttu-id="d4788-130">В этом случае вам нужно использовать формат выходных данных с возвращаемыми значениями с информацией о типах без кавычек.</span><span class="sxs-lookup"><span data-stu-id="d4788-130">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="d4788-131">Наилучший вариант, который предоставляет CLI для этой цели, — `tsv` или значение с разделением знаками табуляции.</span><span class="sxs-lookup"><span data-stu-id="d4788-131">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="d4788-132">В частности, при извлечении отдельного значения (не словаря или списка) выходные данные `tsv` гарантированно не будут включать кавычки.</span><span class="sxs-lookup"><span data-stu-id="d4788-132">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="d4788-133">См. подробнее о [формате выходных данных `tsv`](format-output-azure-cli.md#tsv-output-format).</span><span class="sxs-lookup"><span data-stu-id="d4788-133">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="get-multiple-values"></a><span data-ttu-id="d4788-134">Получение нескольких значений</span><span class="sxs-lookup"><span data-stu-id="d4788-134">Get multiple values</span></span>

<span data-ttu-id="d4788-135">Чтобы получить несколько свойств, заключите список выражений, разделенных запятыми, в квадратные скобки — `[ ]` (__список из нескольких элементов__).</span><span class="sxs-lookup"><span data-stu-id="d4788-135">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="d4788-136">Чтобы получить имя виртуальной машины, имя администратора и ключ SSH с помощью одной команды, введите ее в следующем виде:</span><span class="sxs-lookup"><span data-stu-id="d4788-136">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="d4788-137">Эти значения включены в полученный массив в том порядке, в котором они были указаны в запросе.</span><span class="sxs-lookup"><span data-stu-id="d4788-137">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="d4788-138">Поскольку результат имеет формат массива, значения не имеют соответствующих ключей.</span><span class="sxs-lookup"><span data-stu-id="d4788-138">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="d4788-139">Переименование свойств в запросе</span><span class="sxs-lookup"><span data-stu-id="d4788-139">Rename properties in a query</span></span>

<span data-ttu-id="d4788-140">Чтобы при запросе нескольких значений получить словарь вместо массива, используйте оператор `{ }` (__хэш-таблица из нескольких элементов__).</span><span class="sxs-lookup"><span data-stu-id="d4788-140">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="d4788-141">Формат запроса для получения хэш-таблицы имеет вид `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="d4788-141">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="d4788-142">`displayName` — это строка, отображаемая в выходных данных, а `JMESPathExpression` — вычисляемое выражение JMESPath.</span><span class="sxs-lookup"><span data-stu-id="d4788-142">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="d4788-143">Изменим пример из предыдущего раздела, чтобы заменить список элементов хэш-таблицей:</span><span class="sxs-lookup"><span data-stu-id="d4788-143">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="d4788-144">Получение свойств из массива</span><span class="sxs-lookup"><span data-stu-id="d4788-144">Get properties in an array</span></span>

<span data-ttu-id="d4788-145">Массив не имеет свойств как таковых, но доступ к нему может осуществляться по индексу.</span><span class="sxs-lookup"><span data-stu-id="d4788-145">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="d4788-146">Эта возможность показана в предыдущем примере, когда выражение `publicKeys[0]` использовалось для получения элемента с индексом `publicKeys` из массива.</span><span class="sxs-lookup"><span data-stu-id="d4788-146">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="d4788-147">Порядок выходных данных в командах CLI не гарантирован. Поэтому используйте индексы, только если вы уверены в порядке выходных данных или вам все равно, какой элемент вы получите.</span><span class="sxs-lookup"><span data-stu-id="d4788-147">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="d4788-148">Чтобы получить доступ к элементам массива, используется одна из двух операций: _преобразование в плоскую структуру_ или _фильтрация_.</span><span class="sxs-lookup"><span data-stu-id="d4788-148">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="d4788-149">В этом разделе описано преобразование массива в плоскую структуру.</span><span class="sxs-lookup"><span data-stu-id="d4788-149">This section covers how to flatten an array.</span></span>

<span data-ttu-id="d4788-150">Преобразование массива в плоскую структуру выполняется с помощью оператора JMESPath `[]`.</span><span class="sxs-lookup"><span data-stu-id="d4788-150">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="d4788-151">Все выражения после оператора `[]` применяются к каждому элементу в текущем массиве.</span><span class="sxs-lookup"><span data-stu-id="d4788-151">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="d4788-152">Если оператор `[]` стоит в начале запроса, он преобразовывает в плоскую структуру результат выполнения команды CLI.</span><span class="sxs-lookup"><span data-stu-id="d4788-152">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="d4788-153">Эта возможность позволяет изучить результат выполнения команды `az vm list`.</span><span class="sxs-lookup"><span data-stu-id="d4788-153">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="d4788-154">Чтобы получить имя, сведения об операционной системе и имя администратора для каждой виртуальной машины в группе ресурсов, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="d4788-154">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="d4788-155">При использовании формата выходных данных `--output table` имена столбцов соответствуют значению `displayKey` в хэш-таблице:</span><span class="sxs-lookup"><span data-stu-id="d4788-155">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="d4788-156">Некоторые ключи отфильтровываются и не печатаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="d4788-156">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="d4788-157">Эти ключи — `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="d4788-157">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="d4788-158">Чтобы отобразить эти значения, можно изменить имя ключа в хэш-таблице.</span><span class="sxs-lookup"><span data-stu-id="d4788-158">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="d4788-159">Преобразовать в плоскую структуру можно любой массив, а не только массив верхнего уровня, возвращаемый командой.</span><span class="sxs-lookup"><span data-stu-id="d4788-159">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="d4788-160">В предыдущем разделе с помощью выражения `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` мы получили открытый ключ SSH, используемый для входа.</span><span class="sxs-lookup"><span data-stu-id="d4788-160">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="d4788-161">Чтобы получить _все_ открытые ключи SSH, выражение можно записать в следующем виде: `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span><span class="sxs-lookup"><span data-stu-id="d4788-161">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="d4788-162">Этот запрос преобразовывает массив `osProfile.linuxConfiguration.ssh.publicKeys` в плоскую структуру, а затем применяет выражение `keyData` к каждому элементу:</span><span class="sxs-lookup"><span data-stu-id="d4788-162">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="d4788-163">Фильтрация массивов</span><span class="sxs-lookup"><span data-stu-id="d4788-163">Filter arrays</span></span>

<span data-ttu-id="d4788-164">Еще одной операцией, используемой для получения данных из массива, является _фильтрация_.</span><span class="sxs-lookup"><span data-stu-id="d4788-164">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="d4788-165">Фильтрация выполняется с помощью оператора JMESPath `[?...]`.</span><span class="sxs-lookup"><span data-stu-id="d4788-165">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="d4788-166">В этом операторе используется предикат.</span><span class="sxs-lookup"><span data-stu-id="d4788-166">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="d4788-167">Предикат — это любое выражение, результат которого равен `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="d4788-167">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="d4788-168">Выражения, предикат которых возвращает `true`, включаются в выходные данные.</span><span class="sxs-lookup"><span data-stu-id="d4788-168">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="d4788-169">JMESPath поддерживает стандартные операторы сравнения и логические операторы.</span><span class="sxs-lookup"><span data-stu-id="d4788-169">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="d4788-170">Это операторы `<`, `<=`, `>`, `>=`, `==` и `!=`.</span><span class="sxs-lookup"><span data-stu-id="d4788-170">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="d4788-171">JMESPath также поддерживает логические операторы "И" (`&&`), "ИЛИ" (`||`) и "НЕ" (`!`).</span><span class="sxs-lookup"><span data-stu-id="d4788-171">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="d4788-172">Выражения можно объединять в группы с помощью круглых скобок. Это позволяет использовать более сложные выражения в качестве предикатов.</span><span class="sxs-lookup"><span data-stu-id="d4788-172">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="d4788-173">Подробные сведения о предикатах и логических операциях см. в [спецификации JMESPath](http://jmespath.org/specification.html).</span><span class="sxs-lookup"><span data-stu-id="d4788-173">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="d4788-174">В последнем примере мы преобразовали массив в плоскую структуру, чтобы получить список всех виртуальных машин в группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d4788-174">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="d4788-175">С помощью фильтров в эти выходные данные можно включить только виртуальные машины с ОС Linux:</span><span class="sxs-lookup"><span data-stu-id="d4788-175">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="d4788-176">В JMESPath строки всегда заключаются в одиночные кавычки (`'`).</span><span class="sxs-lookup"><span data-stu-id="d4788-176">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="d4788-177">Если в строке, стоящей в предикате фильтра, используются двойные кавычки, команда вернет пустой результат.</span><span class="sxs-lookup"><span data-stu-id="d4788-177">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="d4788-178">В JMESPath также встроены функции, которые помогают фильтровать данные.</span><span class="sxs-lookup"><span data-stu-id="d4788-178">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="d4788-179">Одна из таких функций — `contains(string, substring)`. Она позволяет проверить, содержит ли строка указанную подстроку.</span><span class="sxs-lookup"><span data-stu-id="d4788-179">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="d4788-180">Выражения вычисляются до вызова функции. Поэтому первым аргументом может быть полное выражение JMESPath.</span><span class="sxs-lookup"><span data-stu-id="d4788-180">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="d4788-181">В следующем примере выполняется поиск всех машин, использующих диски SSD для размещения ОС:</span><span class="sxs-lookup"><span data-stu-id="d4788-181">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="d4788-182">Этот запрос достаточно длинный.</span><span class="sxs-lookup"><span data-stu-id="d4788-182">This query is a little long.</span></span> <span data-ttu-id="d4788-183">Ключ `storageProfile.osDisk.managedDisk.storageAccountType` используется дважды, и в выходных данных ему присвоено другое имя.</span><span class="sxs-lookup"><span data-stu-id="d4788-183">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="d4788-184">Один из способов сократить запрос — применить фильтр после преобразования массива в плоскую структуру и выбора данных.</span><span class="sxs-lookup"><span data-stu-id="d4788-184">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="d4788-185">Если в массиве с множество элементов, возможно, применение фильтра перед выбором данных ускорит операцию.</span><span class="sxs-lookup"><span data-stu-id="d4788-185">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="d4788-186">Полный список встроенных функций см. в [этом разделе спецификации JMESPath](http://jmespath.org/specification.html#built-in-functions).</span><span class="sxs-lookup"><span data-stu-id="d4788-186">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="d4788-187">Изменение выходных данных</span><span class="sxs-lookup"><span data-stu-id="d4788-187">Change output</span></span>

<span data-ttu-id="d4788-188">Функции JMESPath также можно использовать для обработки результатов запроса.</span><span class="sxs-lookup"><span data-stu-id="d4788-188">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="d4788-189">Любая функция, которая возвращает значение, отличное от логического, изменяет результаты выражения.</span><span class="sxs-lookup"><span data-stu-id="d4788-189">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="d4788-190">Например, данные можно отсортировать по значению свойства с помощью функции `sort_by(array, &sort_expression)`.</span><span class="sxs-lookup"><span data-stu-id="d4788-190">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="d4788-191">В JMESPath используется специальный оператор `&` для выражений, которые должны вычисляться позднее в функции.</span><span class="sxs-lookup"><span data-stu-id="d4788-191">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="d4788-192">В следующем примере показано, как отсортировать список виртуальных машин по размеру диска с ОС:</span><span class="sxs-lookup"><span data-stu-id="d4788-192">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="d4788-193">Полный список встроенных функций см. в [этом разделе спецификации JMESPath](http://jmespath.org/specification.html#built-in-functions).</span><span class="sxs-lookup"><span data-stu-id="d4788-193">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="d4788-194">Интерактивное использование запросов</span><span class="sxs-lookup"><span data-stu-id="d4788-194">Experiment with queries interactively</span></span>

<span data-ttu-id="d4788-195">Чтобы начать изучение JMESPath, можно использовать пакет Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal), который предоставляет интерактивную среду для работы с запросами.</span><span class="sxs-lookup"><span data-stu-id="d4788-195">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="d4788-196">Данные подаются на вход, и в редакторе можно составлять и выполнять запросы.</span><span class="sxs-lookup"><span data-stu-id="d4788-196">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
