---
title: Форматы выходных данных для Azure CLI
description: Сведения о том, как форматировать результаты выполнения команды Azure CLI в виде таблиц, списков или объектов JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d83dcdda7d7485bc32f0da59163afe7ea906faa6
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593478"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="18a56-103">Форматы выходных данных для команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="18a56-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="18a56-104">Azure CLI использует JSON в качестве формата выходных данных по умолчанию, но поддерживает и другие форматы.</span><span class="sxs-lookup"><span data-stu-id="18a56-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="18a56-105">Параметр `--output` (`--out` или `-o`) позволяет форматировать данные, выводимые CLI.</span><span class="sxs-lookup"><span data-stu-id="18a56-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="18a56-106">Ниже описаны значения аргументов и их типы:</span><span class="sxs-lookup"><span data-stu-id="18a56-106">The argument values and types of output are:</span></span>

<span data-ttu-id="18a56-107">--output</span><span class="sxs-lookup"><span data-stu-id="18a56-107">--output</span></span> | <span data-ttu-id="18a56-108">ОПИСАНИЕ</span><span class="sxs-lookup"><span data-stu-id="18a56-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="18a56-109">Строка в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-109">JSON string.</span></span> <span data-ttu-id="18a56-110">Это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="18a56-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="18a56-111">Выделенная цветом строка JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="18a56-112">YAML, альтернативный JSON машиночитаемый формат.</span><span class="sxs-lookup"><span data-stu-id="18a56-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="18a56-113">Таблица ASCII с ключами в качестве заголовков столбцов.</span><span class="sxs-lookup"><span data-stu-id="18a56-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="18a56-114">Значения, разделенные табуляцией, без ключей.</span><span class="sxs-lookup"><span data-stu-id="18a56-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="18a56-115">Формат выходных данных JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-115">JSON output format</span></span>

<span data-ttu-id="18a56-116">Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-116">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="18a56-117">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="18a56-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="18a56-118">Формат выходных данных YAML</span><span class="sxs-lookup"><span data-stu-id="18a56-118">YAML output format</span></span>

<span data-ttu-id="18a56-119">`yaml`Выходные данные отображаются в [YAML](http://yaml.org/), формате сериализации данных обычного текста.</span><span class="sxs-lookup"><span data-stu-id="18a56-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="18a56-120">YAML легче для восприятия, чем JSON, и сопоставим с ним.</span><span class="sxs-lookup"><span data-stu-id="18a56-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="18a56-121">Входные данные конфигурации некоторых приложений и команд CLI задаются в формате YAML, а не JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="18a56-122">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="18a56-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a><span data-ttu-id="18a56-123">Формат табличных выходных данных</span><span class="sxs-lookup"><span data-stu-id="18a56-123">Table output format</span></span>

<span data-ttu-id="18a56-124">Формат `table` выводит данные в виде таблицы ASCII, упрощая чтение и сканирование данных.</span><span class="sxs-lookup"><span data-stu-id="18a56-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="18a56-125">Вложенные объекты не включаются в таблицу с выходными данными, но их можно отфильтровать как часть запроса.</span><span class="sxs-lookup"><span data-stu-id="18a56-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="18a56-126">Некоторые поля не включаются в таблицу, поэтому этот формат лучше всего подходит, когда вам нужно быстро получить обзор данных в наглядной форме.</span><span class="sxs-lookup"><span data-stu-id="18a56-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="18a56-127">Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="18a56-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="18a56-128">Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.</span><span class="sxs-lookup"><span data-stu-id="18a56-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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
> <span data-ttu-id="18a56-129">Некоторые ключи по умолчанию не отображаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="18a56-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="18a56-130">Доступны следующие параметры: `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="18a56-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="18a56-131">Если вам нужно отобразить их в выходных данных, вы можете использовать функцию повторного добавления ключа JMESPath, чтобы изменить имя ключа и избежать фильтрации.</span><span class="sxs-lookup"><span data-stu-id="18a56-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="18a56-132">Дополнительные сведения об использовании запросов для фильтрации данных см. в [руководстве по использованию запросов JMESPath в Azure CLI](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="18a56-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="18a56-133">Формат выходных данных TSV</span><span class="sxs-lookup"><span data-stu-id="18a56-133">TSV output format</span></span>

<span data-ttu-id="18a56-134">Формат выходных данных `tsv` возвращает значения, разделенные табуляцией и символом новой строки без дополнительного форматирования, ключей и других символов.</span><span class="sxs-lookup"><span data-stu-id="18a56-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="18a56-135">Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме.</span><span class="sxs-lookup"><span data-stu-id="18a56-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="18a56-136">Как и формат `table`, `tsv` не отображает вложенные объекты.</span><span class="sxs-lookup"><span data-stu-id="18a56-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="18a56-137">Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.</span><span class="sxs-lookup"><span data-stu-id="18a56-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="18a56-138">На следующем примере показано, как выходные данные команды `tsv` можно передать по каналу в другие команды оболочки bash.</span><span class="sxs-lookup"><span data-stu-id="18a56-138">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="18a56-139">Команда `grep` выбирает элементы, содержащие текст RGD, а затем команда `cut` выбирает восьмое поле, чтобы отобразить имя виртуальной машины в выходных данных.</span><span class="sxs-lookup"><span data-stu-id="18a56-139">`grep` selects items that have text "RGD" in them, then the `cut` command selects the eighth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="18a56-140">Для обработки полей, разделенных знаками табуляции, значения выводятся в том же порядке, что и в отображенном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="18a56-140">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="18a56-141">Этот порядок гарантирует согласованность между выполнениями команды.</span><span class="sxs-lookup"><span data-stu-id="18a56-141">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="18a56-142">Настройка формата вывода по умолчанию</span><span class="sxs-lookup"><span data-stu-id="18a56-142">Set the default output format</span></span>

<span data-ttu-id="18a56-143">Вы можете использовать интерактивную команду `az configure`, чтобы настроить окружение и выбрать параметры по умолчанию для форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="18a56-143">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="18a56-144">Формат выходных данных по умолчанию — `json`.</span><span class="sxs-lookup"><span data-stu-id="18a56-144">The default output format is `json`.</span></span>

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

<span data-ttu-id="18a56-145">Дополнительные сведения о настройке среды см. в [руководстве по конфигурации Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="18a56-145">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
