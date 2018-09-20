---
title: Форматы выходных данных для Azure CLI 2.0
description: Форматирование результатов выполнения команд Azure CLI 2.0 в таблицы, списки или файлы JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 07a5e9d913257d6aeb20a68263a6256ffadbe627
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388513"
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="061b7-103">Форматы выходных данных для команд Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="061b7-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="061b7-104">Azure CLI 2.0 использует JSON в качестве формата выходных данных по умолчанию, но поддерживает и другие форматы.</span><span class="sxs-lookup"><span data-stu-id="061b7-104">Azure CLI 2.0 uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="061b7-105">Параметр `--output` (`--out` или `-o`) позволяет форматировать данные, выводимые CLI.</span><span class="sxs-lookup"><span data-stu-id="061b7-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="061b7-106">Ниже описаны значения аргументов и их типы:</span><span class="sxs-lookup"><span data-stu-id="061b7-106">The argument values and types of output are:</span></span>

<span data-ttu-id="061b7-107">--output</span><span class="sxs-lookup"><span data-stu-id="061b7-107">--output</span></span> | <span data-ttu-id="061b7-108">ОПИСАНИЕ</span><span class="sxs-lookup"><span data-stu-id="061b7-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="061b7-109">Строка в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="061b7-109">JSON string.</span></span> <span data-ttu-id="061b7-110">Это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="061b7-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="061b7-111">Выделенная цветом строка JSON.</span><span class="sxs-lookup"><span data-stu-id="061b7-111">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="061b7-112">Таблица ASCII с ключами в качестве заголовков столбцов.</span><span class="sxs-lookup"><span data-stu-id="061b7-112">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="061b7-113">Значения, разделенные табуляцией, без ключей.</span><span class="sxs-lookup"><span data-stu-id="061b7-113">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="061b7-114">Формат выходных данных JSON.</span><span class="sxs-lookup"><span data-stu-id="061b7-114">JSON output format</span></span>

<span data-ttu-id="061b7-115">Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.</span><span class="sxs-lookup"><span data-stu-id="061b7-115">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="061b7-116">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="061b7-116">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="061b7-117">Формат табличных выходных данных</span><span class="sxs-lookup"><span data-stu-id="061b7-117">Table output format</span></span>

<span data-ttu-id="061b7-118">Формат `table` выводит данные в виде таблицы ASCII, упрощая чтение и сканирование данных.</span><span class="sxs-lookup"><span data-stu-id="061b7-118">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="061b7-119">Вложенные объекты не включаются в таблицу с выходными данными, но их можно отфильтровать как часть запроса.</span><span class="sxs-lookup"><span data-stu-id="061b7-119">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="061b7-120">Некоторые поля не включаются в таблицу, поэтому этот формат лучше всего подходит, когда вам нужно быстро получить обзор данных в наглядной форме.</span><span class="sxs-lookup"><span data-stu-id="061b7-120">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="061b7-121">Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="061b7-121">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="061b7-122">Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.</span><span class="sxs-lookup"><span data-stu-id="061b7-122">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="061b7-123">Некоторые ключи по умолчанию не отображаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="061b7-123">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="061b7-124">Доступны следующие параметры: `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="061b7-124">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="061b7-125">Если вам нужно отобразить их в выходных данных, вы можете использовать функцию повторного добавления ключа JMESPath, чтобы изменить имя ключа и избежать фильтрации.</span><span class="sxs-lookup"><span data-stu-id="061b7-125">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="061b7-126">Дополнительные сведения об использовании запросов для фильтрации данных см. в руководстве по [использованию запросов JMESPath с Azure CLI 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="061b7-126">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="061b7-127">Формат выходных данных TSV</span><span class="sxs-lookup"><span data-stu-id="061b7-127">TSV output format</span></span>

<span data-ttu-id="061b7-128">Формат выходных данных `tsv` возвращает значения, разделенные табуляцией и символом новой строки без дополнительного форматирования, ключей и других символов.</span><span class="sxs-lookup"><span data-stu-id="061b7-128">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="061b7-129">Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме.</span><span class="sxs-lookup"><span data-stu-id="061b7-129">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="061b7-130">Как и формат `table`, `tsv` не отображает вложенные объекты.</span><span class="sxs-lookup"><span data-stu-id="061b7-130">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="061b7-131">Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.</span><span class="sxs-lookup"><span data-stu-id="061b7-131">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="061b7-132">На следующем примере показано, как выходные данные команды `tsv` можно передать по каналу в другие команды оболочки bash.</span><span class="sxs-lookup"><span data-stu-id="061b7-132">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="061b7-133">Команда `grep` выбирает элементы, содержащие текст RGD, а затем команда `cut` выбирает восьмое поле, чтобы отобразить имя виртуальной машины в выходных данных.</span><span class="sxs-lookup"><span data-stu-id="061b7-133">`grep` selects items that have text "RGD" in them, then the `cut` command selects the eighth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="061b7-134">Для обработки полей, разделенных знаками табуляции, значения выводятся в том же порядке, что и в отображенном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="061b7-134">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="061b7-135">Этот порядок гарантирует согласованность между выполнениями команды.</span><span class="sxs-lookup"><span data-stu-id="061b7-135">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="061b7-136">Настройка формата вывода по умолчанию</span><span class="sxs-lookup"><span data-stu-id="061b7-136">Set the default output format</span></span>

<span data-ttu-id="061b7-137">Вы можете использовать интерактивную команду `az configure`, чтобы настроить окружение и выбрать параметры по умолчанию для форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="061b7-137">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="061b7-138">Формат выходных данных по умолчанию — `json`.</span><span class="sxs-lookup"><span data-stu-id="061b7-138">The default output format is `json`.</span></span>

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

<span data-ttu-id="061b7-139">Дополнительные сведения о настройке окружения см. в описании [конфигурации Azure CLI 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="061b7-139">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>