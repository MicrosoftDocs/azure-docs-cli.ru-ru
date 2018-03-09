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
ms.openlocfilehash: 96092c0cced4e0f88aa8898525bc3dd348550407
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Использование запросов JMESPath в Azure CLI 2.0

Интерфейс Azure CLI 2.0 использует аргумент `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команд. JMESPath — это язык запросов для JSON, который позволяет выбирать и представлять данные из выходных данных CLI. Эти запросы выполняются в выходных данных JSON до выполнения форматирования отображаемых данных.

Аргумент `--query` поддерживается всеми командами в Azure CLI. Примеры в этой статье включают распространенные варианты использования возможностей JMESPath.

## <a name="work-with-dictionary-output"></a>Работа с выходными данными словаря

Команды, которые возвращают словарь JSON, можно изучать по именам ключей. Пути ключей используют символ `.` в качестве разделителя. Следующий пример извлекает список открытых ключей SSH для подключения к виртуальной машине Linux:

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Можно также получить несколько значений, включив их в упорядоченный массив. Массив не имеет сведений о ключах, но порядок элементов массива совпадает с порядком запрашиваемых ключей. В следующем примере показано, как получить имя образа Azure, имя и размер диска операционной системы:

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Чтобы получить ключи в выходных данных, можно использовать альтернативный синтаксис словаря. При выборе нескольких элементов элемент в словаре используется формат `{displayKey:keyPath, ...}` для фильтрации выражения `keyPath` JMESPath. Результат выводится в виде `{displayKey: value}`. Следующий пример принимает предыдущий запрос и делает его более четким, назначая ключи в выходные данные:

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

При выводе сведений в выходном формате `table` отображать словарь особенно удобно. Это позволяет настраивать собственные заголовки столбцов, облегчая чтение выходных данных. См. дополнительные сведения о [форматах выходных данных для команд Azure CLI 2.0](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Некоторые ключи отфильтровываются и не печатаются в табличном представлении. Эти ключи — `id`, `type` и `etag`. Если необходимо просмотреть эти сведения, можно изменить имя ключа, избегая фильтрации.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Использование вывода списка

Команды CLI, которые могут возвращать несколько значений, всегда возвращают массив. Доступ к элементам массива осуществляется по индексу. В CLI элементы могут не упорядочиваться. Лучше всего выполнять запрос к массиву значений, преобразуя их в плоскую структуру с помощью оператора `[]`. Оператор записывается после ключа массива или как первый элемент в выражении. После преобразования запрос выполняется к каждому отдельному элементу в массиве, при этом результирующие значения включаются в новый массив. В следующем примере выводятся имя и ОС, запущенная на каждой виртуальной машине в группе ресурсов. 

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

Массивы, которые входят в путь ключа, также можно преобразовать в плоскую структуру. Этот пример показывает запрос, который возвращает идентификаторы объектов Azure для сетевых адаптеров, к которым подключена виртуальная машина.

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Фильтрация выходных данных массива с использованием предикатов

JMESPath предлагает [выражения для фильтрации](http://jmespath.org/specification.html#filterexpressions) отображаемых данных. Это мощное средство, особенно при использовании в комбинации со [встроенными функциями JMESPath ](http://jmespath.org/specification.html#built-in-functions) для выполнения частичных совпадений или преобразования данных в стандартный формат. Выражения фильтрации работают только с данными массива данных. При использовании в других случаях они возвращают значение `null`. Например, можно получить выходные данные таких команд, как `vm list`, и отфильтровать их для поиска определенных типов виртуальных машин. Следующий пример продолжает предыдущий. В нем отфильтровывается тип виртуальных машин для записи только виртуальных машин Windows и вывода их имени.

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Интерактивное использование запросов

Для экспериментов с выражениями JMESPath удобно работать так, чтобы можно было быстро изменять запросы и проверять выходные данные. Для этого используется интерактивное окружение [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) пакета Python. Оно отображает данные конвейера как входные, а затем создает запросы для извлечения данных.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
