---
title: "Результаты выполнения команды запроса в Azure CLI 2.0"
description: "Выполнение запросов JMESPath к результатам команд CLI Azure 2.0."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/22/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 2a0cdc34bbaf0864885588ecaddff725c744c90e
ms.sourcegitcommit: 5a4c7205087d2f6c4800cf25178f0543a6157d99
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/24/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="aec0a-103">Использование запросов JMESPath в Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="aec0a-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="aec0a-104">Интерфейс Azure CLI 2.0 использует аргумент `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команд.</span><span class="sxs-lookup"><span data-stu-id="aec0a-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="aec0a-105">JMESPath — это язык запросов для JSON, который позволяет выбирать и представлять данные из выходных данных CLI.</span><span class="sxs-lookup"><span data-stu-id="aec0a-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="aec0a-106">Эти запросы выполняются в выходных данных JSON до выполнения форматирования отображаемых данных.</span><span class="sxs-lookup"><span data-stu-id="aec0a-106">These queries are executed on the JSON output, before performing any other display formatting.</span></span>

<span data-ttu-id="aec0a-107">Аргумент `--query` поддерживается всеми командами в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="aec0a-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="aec0a-108">Примеры в этой статье включают распространенные варианты использования возможностей JMESPath.</span><span class="sxs-lookup"><span data-stu-id="aec0a-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="aec0a-109">Работа с выходными данными словаря</span><span class="sxs-lookup"><span data-stu-id="aec0a-109">Work with dictionary output</span></span>

<span data-ttu-id="aec0a-110">Команды, которые возвращают словарь JSON, можно изучать по именам ключей.</span><span class="sxs-lookup"><span data-stu-id="aec0a-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="aec0a-111">Пути ключей используют символ `.` в качестве разделителя.</span><span class="sxs-lookup"><span data-stu-id="aec0a-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="aec0a-112">Следующий пример извлекает список открытых ключей SSH для подключения к виртуальной машине Linux:</span><span class="sxs-lookup"><span data-stu-id="aec0a-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="aec0a-113">Можно также получить несколько значений, включив их в упорядоченный массив.</span><span class="sxs-lookup"><span data-stu-id="aec0a-113">You can also get multiple values, putting them in an ordered array.</span></span> <span data-ttu-id="aec0a-114">Массив не имеет сведений о ключах, но порядок элементов массива совпадает с порядком запрашиваемых ключей.</span><span class="sxs-lookup"><span data-stu-id="aec0a-114">The array doesn't have any key information, but the order of the array's elements matches the order of the queried keys.</span></span> <span data-ttu-id="aec0a-115">В следующем примере показано, как получить имя образа Azure, имя и размер диска операционной системы:</span><span class="sxs-lookup"><span data-stu-id="aec0a-115">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="aec0a-116">Чтобы получить ключи в выходных данных, можно использовать альтернативный синтаксис словаря.</span><span class="sxs-lookup"><span data-stu-id="aec0a-116">If you want keys in your output, you can use an alternate dictionary syntax.</span></span> <span data-ttu-id="aec0a-117">При выборе нескольких элементов элемент в словаре используется формат `{displayKey:keyPath, ...}` для фильтрации выражения `keyPath` JMESPath.</span><span class="sxs-lookup"><span data-stu-id="aec0a-117">Multiple element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="aec0a-118">Результат выводится в виде `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="aec0a-118">This displays in the output as `{displayKey: value}`.</span></span> <span data-ttu-id="aec0a-119">Следующий пример принимает предыдущий запрос и делает его более четким, назначая ключи в выходные данные:</span><span class="sxs-lookup"><span data-stu-id="aec0a-119">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="aec0a-120">При выводе сведений в выходном формате `table` отображать словарь особенно удобно.</span><span class="sxs-lookup"><span data-stu-id="aec0a-120">When displaying information in the `table` output format, dictionary display is especially useful.</span></span> <span data-ttu-id="aec0a-121">Это позволяет настраивать собственные заголовки столбцов, облегчая чтение выходных данных.</span><span class="sxs-lookup"><span data-stu-id="aec0a-121">This allows for setting your own column headers, making output even easier to read.</span></span> <span data-ttu-id="aec0a-122">См. дополнительные сведения о [форматах выходных данных для команд Azure CLI 2.0](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="aec0a-122">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="aec0a-123">Некоторые ключи отфильтровываются и не печатаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="aec0a-123">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="aec0a-124">Эти ключи — `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="aec0a-124">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="aec0a-125">Если необходимо просмотреть эти сведения, можно изменить имя ключа, избегая фильтрации.</span><span class="sxs-lookup"><span data-stu-id="aec0a-125">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="aec0a-126">Использование вывода списка</span><span class="sxs-lookup"><span data-stu-id="aec0a-126">Work with list output</span></span>

<span data-ttu-id="aec0a-127">Команды CLI, которые могут возвращать несколько значений, всегда возвращают массив.</span><span class="sxs-lookup"><span data-stu-id="aec0a-127">CLI commands that may return more than one value always return an array.</span></span> <span data-ttu-id="aec0a-128">Доступ к элементам массива осуществляется по индексу. В CLI элементы могут не упорядочиваться.</span><span class="sxs-lookup"><span data-stu-id="aec0a-128">Arrays can have their elements accessed by index, but there's never an order guarantee from the CLI.</span></span> <span data-ttu-id="aec0a-129">Лучше всего выполнять запрос к массиву значений, преобразуя их в плоскую структуру с помощью оператора `[]`.</span><span class="sxs-lookup"><span data-stu-id="aec0a-129">The best way to query an array of values is to flatten them with the `[]` operator.</span></span> <span data-ttu-id="aec0a-130">Оператор записывается после ключа массива или как первый элемент в выражении.</span><span class="sxs-lookup"><span data-stu-id="aec0a-130">The operator is written after the key for the array, or as the first element in the expression.</span></span> <span data-ttu-id="aec0a-131">После преобразования запрос выполняется к каждому отдельному элементу в массиве, при этом результирующие значения включаются в новый массив.</span><span class="sxs-lookup"><span data-stu-id="aec0a-131">Flattening runs the query following it against each individual element in the array, and places the resulting values into a new array.</span></span> <span data-ttu-id="aec0a-132">В следующем примере выводятся имя и ОС, запущенная на каждой виртуальной машине в группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="aec0a-132">The following example prints out the name and OS running on each VM in a resource group.</span></span> 

```azurecli
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

<span data-ttu-id="aec0a-133">Массивы, которые входят в путь ключа, также можно преобразовать в плоскую структуру.</span><span class="sxs-lookup"><span data-stu-id="aec0a-133">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="aec0a-134">Этот пример показывает запрос, который возвращает идентификаторы объектов Azure для сетевых адаптеров, к которым подключена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="aec0a-134">This example demonstrates a query that gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="aec0a-135">Фильтрация выходных данных массива с использованием предикатов</span><span class="sxs-lookup"><span data-stu-id="aec0a-135">Filter array output with predicates</span></span>

<span data-ttu-id="aec0a-136">JMESPath предлагает [выражения для фильтрации](http://jmespath.org/specification.html#filterexpressions) отображаемых данных.</span><span class="sxs-lookup"><span data-stu-id="aec0a-136">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="aec0a-137">Это мощное средство, особенно при использовании в комбинации со [встроенными функциями JMESPath ](http://jmespath.org/specification.html#built-in-functions) для выполнения частичных совпадений или преобразования данных в стандартный формат.</span><span class="sxs-lookup"><span data-stu-id="aec0a-137">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to perform partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="aec0a-138">Выражения фильтрации работают только с данными массива данных. При использовании в других случаях они возвращают значение `null`.</span><span class="sxs-lookup"><span data-stu-id="aec0a-138">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="aec0a-139">Например, можно получить выходные данные таких команд, как `vm list`, и отфильтровать их для поиска определенных типов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="aec0a-139">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="aec0a-140">Следующий пример продолжает предыдущий. В нем отфильтровывается тип виртуальных машин для записи только виртуальных машин Windows и вывода их имени.</span><span class="sxs-lookup"><span data-stu-id="aec0a-140">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="aec0a-141">Интерактивное использование запросов</span><span class="sxs-lookup"><span data-stu-id="aec0a-141">Experiment with queries interactively</span></span>

<span data-ttu-id="aec0a-142">Для экспериментов с выражениями JMESPath удобно работать так, чтобы можно было быстро изменять запросы и проверять выходные данные.</span><span class="sxs-lookup"><span data-stu-id="aec0a-142">To experiment with JMESPath expressions, you might want to work in a way where you can quickly edit queries and inspect the output.</span></span> <span data-ttu-id="aec0a-143">Для этого используется интерактивное окружение [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) пакета Python. Оно отображает данные конвейера как входные, а затем создает запросы для извлечения данных.</span><span class="sxs-lookup"><span data-stu-id="aec0a-143">An interactive environment is offered by the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package, which allows for piping data as input and then writing in-program queries to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```
