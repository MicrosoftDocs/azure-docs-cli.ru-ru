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
# <a name="use-jmespath-queries-with-azure-cli"></a>Использование запросов JMESPath в Azure CLI 

Интерфейс Azure CLI использует аргумент `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команд. JMESPath — это язык запросов для JSON, который позволяет выбирать и представлять данные из выходных данных CLI. Запросы выполняются с выходными данными в формате JSON до форматирования для отображения.

Аргумент `--query` поддерживается всеми командами в Azure CLI. Примеры в этой статье включают распространенные варианты использования возможностей JMESPath.

## <a name="work-with-dictionary-output"></a>Работа с выходными данными словаря

Команды, которые возвращают словарь JSON, можно изучать по именам ключей. Пути ключей используют символ `.` в качестве разделителя. Следующий пример извлекает список открытых ключей SSH для подключения к виртуальной машине Linux:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Несколько значений можно поместить в упорядоченный массив. В следующем примере показано, как получить имя образа Azure, имя и размер диска операционной системы:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Чтобы получить ключи в выходных данных, можно использовать альтернативный синтаксис словаря.  Чтобы выбрать элемент в словаре, используется формат `{displayKey:keyPath, ...}` для фильтрации выражения JMESPath `keyPath`. В выходных значениях пары "ключ-значение" меняются на `{displayKey: value}`. Следующий пример принимает предыдущий запрос и делает его более четким, назначая ключи в выходные данные:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

При отображении выводимой информации в формате `table` отображение словаря позволяет задавать собственные заголовки столбцов. См. дополнительные сведения о [форматах выходных данных для команд Azure CLI](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Некоторые ключи отфильтровываются и не печатаются в табличном представлении. Эти ключи — `id`, `type` и `etag`. Если необходимо просмотреть эти сведения, можно изменить имя ключа, избегая фильтрации.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Использование вывода списка

Команды CLI, которые могут возвращать несколько значений, всегда возвращают массив. Доступ к элементам массива осуществляется по индексу, и каждый раз порядок элементов может отличаться. Можно выполнить запрос ко всем элементам массива одновременно путем преобразования их в плоскую структуру с помощью оператора `[]`. Этот оператор помещается после массива или используется как первый элемент выражения. При преобразовании массива в плоскую структуру последующий запрос обрабатывает каждый элемент массива.

В следующем примере выводятся имя и ОС, запущенная на каждой виртуальной машине в группе ресурсов.

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

Массивы, которые входят в путь ключа, также можно преобразовать в плоскую структуру. Следующий запрос получает идентификаторы объектов Azure для сетевых адаптеров, к которым подключена виртуальная машина.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Фильтрация выходных данных массива с использованием предикатов

JMESPath предлагает [выражения для фильтрации](http://jmespath.org/specification.html#filterexpressions) отображаемых данных. Эти выражения представляют собой мощное средство, особенно при использовании в комбинации со [встроенными функциями JMESPath ](http://jmespath.org/specification.html#built-in-functions) для поиска частичных совпадений или преобразования данных в стандартный формат. Выражения фильтрации работают только с данными массива данных. При использовании в других случаях они возвращают значение `null`. Например, можно получить выходные данные таких команд, как `vm list`, и отфильтровать их для поиска определенных типов виртуальных машин. Следующий пример продолжает предыдущий. В нем отфильтровывается тип виртуальных машин для записи только виртуальных машин Windows и вывода их имени.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Интерактивное использование запросов

Если вы хотите начать изучение JMESPath, пакет Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) предлагает интерактивную среду для экспериментов с запросами. Данные подаются по каналу на вход, а затем внутри программы можно писать и изменять запросы, чтобы извлекать данные.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
