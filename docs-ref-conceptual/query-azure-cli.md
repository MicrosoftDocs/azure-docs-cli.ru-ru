---
title: Запросы результатов команд в Azure CLI
description: Сведения о том, как выполнять запросы JMESPath к результатам команд Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1736d1677fb6c7fc83a092493e8706c2d5edfccd
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222537"
---
# <a name="use-jmespath-queries-with-azure-cli"></a><span data-ttu-id="22c03-103">Использование запросов JMESPath в Azure CLI</span><span class="sxs-lookup"><span data-stu-id="22c03-103">Use JMESPath queries with Azure CLI</span></span> 

<span data-ttu-id="22c03-104">Интерфейс Azure CLI использует аргумент `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команд.</span><span class="sxs-lookup"><span data-stu-id="22c03-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="22c03-105">JMESPath — это язык запросов для JSON, который позволяет выбирать и представлять данные из выходных данных CLI.</span><span class="sxs-lookup"><span data-stu-id="22c03-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="22c03-106">Запросы выполняются с выходными данными в формате JSON до форматирования для отображения.</span><span class="sxs-lookup"><span data-stu-id="22c03-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="22c03-107">Аргумент `--query` поддерживается всеми командами в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="22c03-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="22c03-108">Примеры в этой статье включают распространенные варианты использования возможностей JMESPath.</span><span class="sxs-lookup"><span data-stu-id="22c03-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="22c03-109">Работа с выходными данными словаря</span><span class="sxs-lookup"><span data-stu-id="22c03-109">Work with dictionary output</span></span>

<span data-ttu-id="22c03-110">Команды, которые возвращают словарь JSON, можно изучать по именам ключей.</span><span class="sxs-lookup"><span data-stu-id="22c03-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="22c03-111">Пути ключей используют символ `.` в качестве разделителя.</span><span class="sxs-lookup"><span data-stu-id="22c03-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="22c03-112">Следующий пример извлекает список открытых ключей SSH для подключения к виртуальной машине Linux:</span><span class="sxs-lookup"><span data-stu-id="22c03-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="22c03-113">Несколько значений можно поместить в упорядоченный массив.</span><span class="sxs-lookup"><span data-stu-id="22c03-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="22c03-114">В следующем примере показано, как получить имя образа Azure, имя и размер диска операционной системы:</span><span class="sxs-lookup"><span data-stu-id="22c03-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="22c03-115">Чтобы получить ключи в выходных данных, можно использовать альтернативный синтаксис словаря.</span><span class="sxs-lookup"><span data-stu-id="22c03-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="22c03-116">Чтобы выбрать элемент в словаре, используется формат `{displayKey:keyPath, ...}` для фильтрации выражения JMESPath `keyPath`.</span><span class="sxs-lookup"><span data-stu-id="22c03-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="22c03-117">В выходных значениях пары "ключ-значение" меняются на `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="22c03-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="22c03-118">Следующий пример принимает предыдущий запрос и делает его более четким, назначая ключи в выходные данные:</span><span class="sxs-lookup"><span data-stu-id="22c03-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="22c03-119">При отображении выводимой информации в формате `table` отображение словаря позволяет задавать собственные заголовки столбцов.</span><span class="sxs-lookup"><span data-stu-id="22c03-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="22c03-120">См. дополнительные сведения о [форматах выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="22c03-120">For more information on output formats, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="22c03-121">Некоторые ключи отфильтровываются и не печатаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="22c03-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="22c03-122">Эти ключи — `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="22c03-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="22c03-123">Если необходимо просмотреть эти сведения, можно изменить имя ключа, избегая фильтрации.</span><span class="sxs-lookup"><span data-stu-id="22c03-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="22c03-124">Использование вывода списка</span><span class="sxs-lookup"><span data-stu-id="22c03-124">Work with list output</span></span>

<span data-ttu-id="22c03-125">Команды CLI, которые могут возвращать несколько значений, всегда возвращают массив.</span><span class="sxs-lookup"><span data-stu-id="22c03-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="22c03-126">Доступ к элементам массива осуществляется по индексу, и каждый раз порядок элементов может отличаться.</span><span class="sxs-lookup"><span data-stu-id="22c03-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="22c03-127">Можно выполнить запрос ко всем элементам массива одновременно путем преобразования их в плоскую структуру с помощью оператора `[]`.</span><span class="sxs-lookup"><span data-stu-id="22c03-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="22c03-128">Этот оператор помещается после массива или используется как первый элемент выражения.</span><span class="sxs-lookup"><span data-stu-id="22c03-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="22c03-129">При преобразовании массива в плоскую структуру последующий запрос обрабатывает каждый элемент массива.</span><span class="sxs-lookup"><span data-stu-id="22c03-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="22c03-130">В следующем примере выводятся имя и ОС, запущенная на каждой виртуальной машине в группе ресурсов.</span><span class="sxs-lookup"><span data-stu-id="22c03-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

```azurecli-interactive
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

<span data-ttu-id="22c03-131">Массивы, которые входят в путь ключа, также можно преобразовать в плоскую структуру.</span><span class="sxs-lookup"><span data-stu-id="22c03-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="22c03-132">Следующий запрос получает идентификаторы объектов Azure для сетевых адаптеров, к которым подключена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="22c03-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="22c03-133">Фильтрация выходных данных массива с использованием предикатов</span><span class="sxs-lookup"><span data-stu-id="22c03-133">Filter array output with predicates</span></span>

<span data-ttu-id="22c03-134">JMESPath предлагает [выражения для фильтрации](http://jmespath.org/specification.html#filterexpressions) отображаемых данных.</span><span class="sxs-lookup"><span data-stu-id="22c03-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="22c03-135">Эти выражения представляют собой мощное средство, особенно при использовании в комбинации со [встроенными функциями JMESPath ](http://jmespath.org/specification.html#built-in-functions) для поиска частичных совпадений или преобразования данных в стандартный формат.</span><span class="sxs-lookup"><span data-stu-id="22c03-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="22c03-136">Выражения фильтрации работают только с данными массива данных. При использовании в других случаях они возвращают значение `null`.</span><span class="sxs-lookup"><span data-stu-id="22c03-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="22c03-137">Например, можно получить выходные данные таких команд, как `vm list`, и отфильтровать их для поиска определенных типов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="22c03-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="22c03-138">Следующий пример продолжает предыдущий. В нем отфильтровывается тип виртуальных машин для записи только виртуальных машин Windows и вывода их имени.</span><span class="sxs-lookup"><span data-stu-id="22c03-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="22c03-139">Интерактивное использование запросов</span><span class="sxs-lookup"><span data-stu-id="22c03-139">Experiment with queries interactively</span></span>

<span data-ttu-id="22c03-140">Если вы хотите начать изучение JMESPath, пакет Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) предлагает интерактивную среду для экспериментов с запросами.</span><span class="sxs-lookup"><span data-stu-id="22c03-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="22c03-141">Данные подаются по каналу на вход, а затем внутри программы можно писать и изменять запросы, чтобы извлекать данные.</span><span class="sxs-lookup"><span data-stu-id="22c03-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
