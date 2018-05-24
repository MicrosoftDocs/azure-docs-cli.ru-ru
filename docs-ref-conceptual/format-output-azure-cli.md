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
ms.openlocfilehash: 016465080e95af3ab0650146e955dd8cffc569e8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="5818a-103">Форматы выходных данных для команд Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="5818a-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="5818a-104">Azure CLI 2.0 использует JSON в качестве формата выходных данных по умолчанию, но предлагает различные способы форматирования результатов выполнения команды.</span><span class="sxs-lookup"><span data-stu-id="5818a-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="5818a-105">Используйте параметр `--output` (`--out` или `-o`), чтобы преобразовать формат выходных данных команды в один из типов, указанных в следующей таблице:</span><span class="sxs-lookup"><span data-stu-id="5818a-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="5818a-106">--output</span><span class="sxs-lookup"><span data-stu-id="5818a-106">--output</span></span> | <span data-ttu-id="5818a-107">ОПИСАНИЕ</span><span class="sxs-lookup"><span data-stu-id="5818a-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="5818a-108">Строка в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5818a-108">JSON string.</span></span> <span data-ttu-id="5818a-109">Это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5818a-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="5818a-110">Выделенная цветом строка JSON.</span><span class="sxs-lookup"><span data-stu-id="5818a-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="5818a-111">Таблица ASCII с ключами в качестве заголовков столбцов.</span><span class="sxs-lookup"><span data-stu-id="5818a-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="5818a-112">Значения, разделенные табуляцией, без ключей.</span><span class="sxs-lookup"><span data-stu-id="5818a-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="5818a-113">Формат выходных данных JSON.</span><span class="sxs-lookup"><span data-stu-id="5818a-113">JSON output format</span></span>

<span data-ttu-id="5818a-114">Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5818a-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="5818a-115">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="5818a-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="5818a-116">Формат табличных выходных данных</span><span class="sxs-lookup"><span data-stu-id="5818a-116">Table output format</span></span>

<span data-ttu-id="5818a-117">Формат выходных данных `table` предоставляет обычные выходные данные в виде строк и столбцов с упорядоченными данными, что упрощает чтение и проверку.</span><span class="sxs-lookup"><span data-stu-id="5818a-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="5818a-118">Вложенные объекты не включаются в табличные выходные данные, но все равно могут фильтроваться как часть запроса.</span><span class="sxs-lookup"><span data-stu-id="5818a-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="5818a-119">Некоторые поля также исключаются из табличных данных, поэтому такой формат лучше всего обеспечивает возможность быстрого просмотра и поиска данных пользователем.</span><span class="sxs-lookup"><span data-stu-id="5818a-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="5818a-120">Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="5818a-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="5818a-121">Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.</span><span class="sxs-lookup"><span data-stu-id="5818a-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="5818a-122">Некоторые ключи отфильтровываются и не печатаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="5818a-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="5818a-123">Доступны следующие параметры: `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="5818a-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="5818a-124">Если вам нужно отобразить их в выходных данных, вы можете использовать функцию повторного добавления ключа JMESPath, чтобы изменить имя ключа и избежать фильтрации.</span><span class="sxs-lookup"><span data-stu-id="5818a-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="5818a-125">Дополнительные сведения об использовании запросов для фильтрации данных см. в руководстве по [использованию запросов JMESPath с Azure CLI 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="5818a-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="5818a-126">Формат выходных данных TSV</span><span class="sxs-lookup"><span data-stu-id="5818a-126">TSV output format</span></span>

<span data-ttu-id="5818a-127">Формат выходных данных `tsv` возвращает значения, разделенные табуляцией и символом новой строки без дополнительного форматирования, ключей и других символов.</span><span class="sxs-lookup"><span data-stu-id="5818a-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="5818a-128">Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме.</span><span class="sxs-lookup"><span data-stu-id="5818a-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="5818a-129">Как и формат `table`, вариант `tsv` не выводит вложенные объекты.</span><span class="sxs-lookup"><span data-stu-id="5818a-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="5818a-130">Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.</span><span class="sxs-lookup"><span data-stu-id="5818a-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="5818a-131">В следующем примере показано, как выходные данные `tsv` можно передать в другие команды UNIX для получения более конкретных данных.</span><span class="sxs-lookup"><span data-stu-id="5818a-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="5818a-132">Команда `grep` выбирает элементы, содержащие текст "RGD", а затем команда `cut` выбирает значения восьмого поля (разделенные знаками табуляции) для отображения имени виртуальной машины в выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5818a-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="5818a-133">Для обработки полей, разделенных знаками табуляции, значения выводятся в том же порядке, что и в отображенном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="5818a-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="5818a-134">Этот порядок гарантирует согласованность между выполнениями команды.</span><span class="sxs-lookup"><span data-stu-id="5818a-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="5818a-135">Настройка формата вывода по умолчанию</span><span class="sxs-lookup"><span data-stu-id="5818a-135">Set the default output format</span></span>

<span data-ttu-id="5818a-136">Вы можете использовать интерактивную команду `az configure`, чтобы настроить окружение и выбрать параметры по умолчанию для форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="5818a-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="5818a-137">Формат выходных данных по умолчанию — `json`.</span><span class="sxs-lookup"><span data-stu-id="5818a-137">The default output format is `json`.</span></span> 

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

<span data-ttu-id="5818a-138">Дополнительные сведения о настройке окружения см. в описании [конфигурации Azure CLI 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="5818a-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>