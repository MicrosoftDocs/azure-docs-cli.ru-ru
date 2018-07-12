---
title: Форматы выходных данных для Azure CLI 2.0
description: Форматирование результатов выполнения команд Azure CLI 2.0 в таблицы, списки или файлы JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b402ce89cbf51adb3d521a604e992dd1fb5a42fa
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967611"
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Форматы выходных данных для команд Azure CLI 2.0

Azure CLI 2.0 использует JSON в качестве формата выходных данных по умолчанию, но предлагает различные способы форматирования результатов выполнения команды.  Используйте параметр `--output` (`--out` или `-o`), чтобы преобразовать формат выходных данных команды в один из типов, указанных в следующей таблице:

--output | ОПИСАНИЕ
---------|-------------------------------
`json`   | Строка в формате JSON. Это значение по умолчанию.
`jsonc`  | Выделенная цветом строка JSON.
`table`  | Таблица ASCII с ключами в качестве заголовков столбцов.
`tsv`    | Значения, разделенные табуляцией, без ключей.

## <a name="json-output-format"></a>Формат выходных данных JSON.

Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.

```azurecli-interactive
az vm list --output json
```

Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="table-output-format"></a>Формат табличных выходных данных

Формат выходных данных `table` предоставляет обычные выходные данные в виде строк и столбцов с упорядоченными данными, что упрощает чтение и проверку. Вложенные объекты не включаются в табличные выходные данные, но все равно могут фильтроваться как часть запроса. Некоторые поля также исключаются из табличных данных, поэтому такой формат лучше всего обеспечивает возможность быстрого просмотра и поиска данных пользователем.

```azurecli-interactive
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке. Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> Некоторые ключи отфильтровываются и не печатаются в табличном представлении. Доступны следующие параметры: `id`, `type` и `etag`. Если вам нужно отобразить их в выходных данных, вы можете использовать функцию повторного добавления ключа JMESPath, чтобы изменить имя ключа и избежать фильтрации.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Дополнительные сведения об использовании запросов для фильтрации данных см. в руководстве по [использованию запросов JMESPath с Azure CLI 2.0](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>Формат выходных данных TSV

Формат выходных данных `tsv` возвращает значения, разделенные табуляцией и символом новой строки без дополнительного форматирования, ключей и других символов. Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме. Как и формат `table`, вариант `tsv` не выводит вложенные объекты.

Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

В следующем примере показано, как выходные данные `tsv` можно передать в другие команды UNIX для получения более конкретных данных. Команда `grep` выбирает элементы, содержащие текст "RGD", а затем команда `cut` выбирает значения восьмого поля (разделенные знаками табуляции) для отображения имени виртуальной машины в выходных данных.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

Для обработки полей, разделенных знаками табуляции, значения выводятся в том же порядке, что и в отображенном объекте JSON. Этот порядок гарантирует согласованность между выполнениями команды.

## <a name="set-the-default-output-format"></a>Настройка формата вывода по умолчанию

Вы можете использовать интерактивную команду `az configure`, чтобы настроить окружение и выбрать параметры по умолчанию для форматов выходных данных. Формат выходных данных по умолчанию — `json`.

```azurecli-interactive
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

Дополнительные сведения о настройке окружения см. в описании [конфигурации Azure CLI 2.0](/cli/azure/azure-cli-configuration).