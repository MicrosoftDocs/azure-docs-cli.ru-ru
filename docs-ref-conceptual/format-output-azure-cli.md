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
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2017
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="157e4-104">Форматы выходных данных для команд Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="157e4-104">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="157e4-105">Azure CLI 2.0 использует JSON в качестве формата выходных данных по умолчанию, но предлагает различные способы форматирования результатов выполнения команды.</span><span class="sxs-lookup"><span data-stu-id="157e4-105">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="157e4-106">Используйте параметр `--output` (или `--out`, или `-o`) для преобразования формата выходных данных команды в один из типов, указанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="157e4-106">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table.</span></span> 

<span data-ttu-id="157e4-107">--output</span><span class="sxs-lookup"><span data-stu-id="157e4-107">--output</span></span> | <span data-ttu-id="157e4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="157e4-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="157e4-109">Строка формата JSON.</span><span class="sxs-lookup"><span data-stu-id="157e4-109">json string.</span></span> <span data-ttu-id="157e4-110">Значение по умолчанию — `json`.</span><span class="sxs-lookup"><span data-stu-id="157e4-110">`json` is the default.</span></span>
`jsonc`  | <span data-ttu-id="157e4-111">Выделенная цветом строка JSON.</span><span class="sxs-lookup"><span data-stu-id="157e4-111">colorized json string.</span></span>
`table`  | <span data-ttu-id="157e4-112">Таблица с заголовками столбцов.</span><span class="sxs-lookup"><span data-stu-id="157e4-112">table with column headings.</span></span>
`tsv`    | <span data-ttu-id="157e4-113">Значения, разделенные табуляцией.</span><span class="sxs-lookup"><span data-stu-id="157e4-113">tab-separated values.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a><span data-ttu-id="157e4-114">Использование параметра JSON</span><span class="sxs-lookup"><span data-stu-id="157e4-114">Using the json option</span></span>

<span data-ttu-id="157e4-115">Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.</span><span class="sxs-lookup"><span data-stu-id="157e4-115">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="157e4-116">Результаты отображаются в этом формате (отображается только часть полученного результата для краткости).</span><span class="sxs-lookup"><span data-stu-id="157e4-116">The results are in this form (only showing partial output for sake of brevity).</span></span>

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
 
## <a name="using-the-table-option"></a><span data-ttu-id="157e4-117">Использование формата "таблица"</span><span class="sxs-lookup"><span data-stu-id="157e4-117">Using the table option</span></span>

<span data-ttu-id="157e4-118">Табличное представление позволяет легко читать набор выходных данных, однако в результатах не отображаются вложенные объекты с простым параметром `--output table` в отличие от формата JSON из предыдущего примера.</span><span class="sxs-lookup"><span data-stu-id="157e4-118">The table option provides an easy to read set of output, but note that nested objects are not included in the output with the simple `--output table`, unlike the preceding .json example.</span></span>  <span data-ttu-id="157e4-119">При использовании того же примера с форматом выходных данных "таблица" отображается проверенный список наиболее распространенных значений свойств.</span><span class="sxs-lookup"><span data-stu-id="157e4-119">Using the same example with 'table' output format provides a curated list of most common property values.</span></span>

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

<span data-ttu-id="157e4-120">Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="157e4-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="157e4-121">Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.</span><span class="sxs-lookup"><span data-stu-id="157e4-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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

## <a name="using-the-tsv-option"></a><span data-ttu-id="157e4-122">Использование параметра TSV</span><span class="sxs-lookup"><span data-stu-id="157e4-122">Using the tsv option</span></span>

<span data-ttu-id="157e4-123">Формат выходных данных TSV возвращает простой текст, разделенный табуляцией, без заголовков и дефисов.</span><span class="sxs-lookup"><span data-stu-id="157e4-123">'tsv' output format returns a simple text-based and tab-separated output with no headings and dashes.</span></span> <span data-ttu-id="157e4-124">Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме.</span><span class="sxs-lookup"><span data-stu-id="157e4-124">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="157e4-125">Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.</span><span class="sxs-lookup"><span data-stu-id="157e4-125">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="157e4-126">Следующий пример показывает, как выходные данные `tsv` можно передать в команды `grep` и `cut` для дальнейшего анализа конкретных значений из результатов выполнения команды `list`.</span><span class="sxs-lookup"><span data-stu-id="157e4-126">The next example shows how the `tsv` output can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="157e4-127">Команда `grep` выбирает только элементы, содержащие текст RGD, а затем команда `cut` выбирает только значения восьмого поля (разделенные символами табуляции) для отображения в выходных данных.</span><span class="sxs-lookup"><span data-stu-id="157e4-127">The `grep` command selects only items that have text "RGD" in them and then the `cut` command selects only the eighth field (separated by tabs) value to show in the output.</span></span>

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a><span data-ttu-id="157e4-128">Задание формата выходных данных по умолчанию</span><span class="sxs-lookup"><span data-stu-id="157e4-128">Setting the default output format</span></span>

<span data-ttu-id="157e4-129">Вы можете использовать команду `az configure`, чтобы настроить среду или параметры, например, параметры по умолчанию для выходных форматов.</span><span class="sxs-lookup"><span data-stu-id="157e4-129">You can use the `az configure` command to set up your environment or establish preferences such as default settings for output formats.</span></span> <span data-ttu-id="157e4-130">Для общего пользования самым простым форматом выходных данных по умолчанию является "таблица". Выберите **3**, когда появится запрос на выбор формата выходных данных.</span><span class="sxs-lookup"><span data-stu-id="157e4-130">For common use, the easiest output format default is the "table" format - select **3** when prompted for output format choices.</span></span> 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```