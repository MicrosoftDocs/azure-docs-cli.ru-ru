---
title: "Форматы выходных данных для Azure CLI 2.0"
description: "Использование параметра --output для преобразования формата результатов выполнения команды Azure CLI 2.0 в таблицы, списки или формат JSON."
keywords: "Azure CLI 2.0, выходные данные, формат, таблица, список, JSON, Linux, Mac, Windows, OS X"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 74bdb727-481d-45f7-a44e-15d18dc55483
ms.openlocfilehash: d1440cc1e99ccddb18d23306cc0fcdb4b8babf14
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2017
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Форматы выходных данных для команд Azure CLI 2.0

Azure CLI 2.0 использует JSON в качестве формата выходных данных по умолчанию, но предлагает различные способы форматирования результатов выполнения команды.  Используйте параметр `--output` (или `--out`, или `-o`) для преобразования формата выходных данных команды в один из типов, указанных в следующей таблице. 

--output | Описание
---------|-------------------------------
`json`   | Строка формата JSON. Значение по умолчанию — `json`.
`jsonc`  | Выделенная цветом строка JSON.
`table`  | Таблица с заголовками столбцов.
`tsv`    | Значения, разделенные табуляцией.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a>Использование параметра JSON

Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.

```azurecli-interactive
az vm list --output json
```

Результаты отображаются в этом формате (отображается только часть полученного результата для краткости).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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
 
## <a name="using-the-table-option"></a>Использование формата "таблица"

Табличное представление позволяет легко читать набор выходных данных, однако в результатах не отображаются вложенные объекты с простым параметром `--output table` в отличие от формата JSON из предыдущего примера.  При использовании того же примера с форматом выходных данных "таблица" отображается проверенный список наиболее распространенных значений свойств.

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке. Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.

```azurecli-interactive
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a>Использование параметра TSV

Формат выходных данных TSV возвращает простой текст, разделенный табуляцией, без заголовков и дефисов. Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме. Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

Следующий пример показывает, как выходные данные `tsv` можно передать в команды `grep` и `cut` для дальнейшего анализа конкретных значений из результатов выполнения команды `list`. Команда `grep` выбирает только элементы, содержащие текст RGD, а затем команда `cut` выбирает только значения восьмого поля (разделенные символами табуляции) для отображения в выходных данных.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>Задание формата выходных данных по умолчанию

Вы можете использовать команду `az configure`, чтобы настроить среду или параметры, например, параметры по умолчанию для выходных форматов. Для общего пользования самым простым форматом выходных данных по умолчанию является "таблица". Выберите **3**, когда появится запрос на выбор формата выходных данных. 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```