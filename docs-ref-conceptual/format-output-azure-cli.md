---
title: Форматы выходных данных для Azure CLI
description: Сведения о том, как форматировать результаты выполнения команды Azure CLI в виде таблиц, списков или объектов JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/23/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 125055eec956e56c95af9a1c24ee4254e77556e6
ms.sourcegitcommit: 5b9b4446c08b94256ced7f63c145b493ba8b50df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2019
ms.locfileid: "71217451"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="6165b-103">Форматы выходных данных для команд Azure CLI</span><span class="sxs-lookup"><span data-stu-id="6165b-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="6165b-104">Azure CLI использует JSON в качестве формата выходных данных по умолчанию, но поддерживает и другие форматы.</span><span class="sxs-lookup"><span data-stu-id="6165b-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="6165b-105">Параметр `--output` (`--out` или `-o`) позволяет форматировать данные, выводимые CLI.</span><span class="sxs-lookup"><span data-stu-id="6165b-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="6165b-106">Ниже описаны значения аргументов и их типы:</span><span class="sxs-lookup"><span data-stu-id="6165b-106">The argument values and types of output are:</span></span>

<span data-ttu-id="6165b-107">--output</span><span class="sxs-lookup"><span data-stu-id="6165b-107">--output</span></span> | <span data-ttu-id="6165b-108">ОПИСАНИЕ</span><span class="sxs-lookup"><span data-stu-id="6165b-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="6165b-109">Строка в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6165b-109">JSON string.</span></span> <span data-ttu-id="6165b-110">Это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6165b-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="6165b-111">Выделенная цветом строка JSON.</span><span class="sxs-lookup"><span data-stu-id="6165b-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="6165b-112">YAML, альтернативный JSON машиночитаемый формат.</span><span class="sxs-lookup"><span data-stu-id="6165b-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="6165b-113">Таблица ASCII с ключами в качестве заголовков столбцов.</span><span class="sxs-lookup"><span data-stu-id="6165b-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="6165b-114">Значения, разделенные табуляцией, без ключей.</span><span class="sxs-lookup"><span data-stu-id="6165b-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="6165b-115">Формат выходных данных JSON.</span><span class="sxs-lookup"><span data-stu-id="6165b-115">JSON output format</span></span>

<span data-ttu-id="6165b-116">Следующий пример отображает список виртуальных машин в подписках в стандартном формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6165b-116">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="6165b-117">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="6165b-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="6165b-118">Формат выходных данных YAML</span><span class="sxs-lookup"><span data-stu-id="6165b-118">YAML output format</span></span>

<span data-ttu-id="6165b-119">`yaml`Выходные данные отображаются в [YAML](http://yaml.org/), формате сериализации данных обычного текста.</span><span class="sxs-lookup"><span data-stu-id="6165b-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="6165b-120">YAML легче для восприятия, чем JSON, и сопоставим с ним.</span><span class="sxs-lookup"><span data-stu-id="6165b-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="6165b-121">Входные данные конфигурации некоторых приложений и команд CLI задаются в формате YAML, а не JSON.</span><span class="sxs-lookup"><span data-stu-id="6165b-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="6165b-122">Следующие выходные данные содержат некоторые поля, которые исключены для краткости, и замененные сведения для идентификации.</span><span class="sxs-lookup"><span data-stu-id="6165b-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="6165b-123">Формат табличных выходных данных</span><span class="sxs-lookup"><span data-stu-id="6165b-123">Table output format</span></span>

<span data-ttu-id="6165b-124">Формат `table` выводит данные в виде таблицы ASCII, упрощая чтение и сканирование данных.</span><span class="sxs-lookup"><span data-stu-id="6165b-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="6165b-125">Вложенные объекты не включаются в таблицу с выходными данными, но их можно отфильтровать как часть запроса.</span><span class="sxs-lookup"><span data-stu-id="6165b-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="6165b-126">Некоторые поля не включаются в таблицу, поэтому этот формат лучше всего подходит, когда вам нужно быстро получить обзор данных в наглядной форме.</span><span class="sxs-lookup"><span data-stu-id="6165b-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="6165b-127">Вы можете использовать параметр `--query` для настройки свойств и столбцов, которые будут отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="6165b-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="6165b-128">Следующий пример показывает, как выбрать только имя виртуальной машины и имя группы ресурсов в команде `list`.</span><span class="sxs-lookup"><span data-stu-id="6165b-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="6165b-129">Некоторые ключи по умолчанию не отображаются в табличном представлении.</span><span class="sxs-lookup"><span data-stu-id="6165b-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="6165b-130">Доступны следующие параметры: `id`, `type` и `etag`.</span><span class="sxs-lookup"><span data-stu-id="6165b-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="6165b-131">Если вам нужно отобразить их в выходных данных, вы можете использовать функцию повторного добавления ключа JMESPath, чтобы изменить имя ключа и избежать фильтрации.</span><span class="sxs-lookup"><span data-stu-id="6165b-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="6165b-132">Дополнительные сведения об использовании запросов для фильтрации данных см. в [руководстве по использованию запросов JMESPath в Azure CLI](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="6165b-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="6165b-133">Формат выходных данных TSV</span><span class="sxs-lookup"><span data-stu-id="6165b-133">TSV output format</span></span>

<span data-ttu-id="6165b-134">Формат выходных данных `tsv` возвращает значения, разделенные табуляцией и символом новой строки без дополнительного форматирования, ключей и других символов.</span><span class="sxs-lookup"><span data-stu-id="6165b-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="6165b-135">Такой формат позволяет использовать выходные данные в других командах и инструментах, необходимых для обработки текста в определенной форме.</span><span class="sxs-lookup"><span data-stu-id="6165b-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="6165b-136">Как и формат `table`, `tsv` не отображает вложенные объекты.</span><span class="sxs-lookup"><span data-stu-id="6165b-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="6165b-137">Если применить для предыдущего примера параметр `tsv`, отобразится результат в виде текста, разделенного табуляцией.</span><span class="sxs-lookup"><span data-stu-id="6165b-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="6165b-138">Одним из ограничений формата вывода TSV является то, что порядок вывода не гарантируется.</span><span class="sxs-lookup"><span data-stu-id="6165b-138">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="6165b-139">В интерфейсе командной строки порядок сохраняется за счет расположения ключей в алфавитном порядке в ответе JSON и последующем выводе их значений в том порядке, который соответствует выходным данным TSV.</span><span class="sxs-lookup"><span data-stu-id="6165b-139">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="6165b-140">Это не гарантирует постоянного соблюдения порядка, так как формат ответа службы Azure может измениться.</span><span class="sxs-lookup"><span data-stu-id="6165b-140">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="6165b-141">Чтобы обеспечить требуемый порядок, необходимо использовать параметр `--query` и формат [списка из нескольких элементов](query-azure-cli.md#get-multiple-values).</span><span class="sxs-lookup"><span data-stu-id="6165b-141">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="6165b-142">Если команда CLI возвращает один словарь JSON, используйте общий формат `[key1, key2, ..., keyN]` для обеспечения порядка ключей.</span><span class="sxs-lookup"><span data-stu-id="6165b-142">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="6165b-143">Если команда CLI возвращает массив, используйте общий формат `[].[key1, key2, ..., keyN]`, чтобы упорядочить значения столбцов.</span><span class="sxs-lookup"><span data-stu-id="6165b-143">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="6165b-144">Так, чтобы упорядочить приведенные выше сведения по идентификатору, расположению, группе ресурсов и имени виртуальной машины, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="6165b-144">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

<span data-ttu-id="6165b-145">На следующем примере показано, как выходные данные команды `tsv` можно передать по каналу в другие команды оболочки bash.</span><span class="sxs-lookup"><span data-stu-id="6165b-145">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="6165b-146">Фильтрация выходных данных и принудительное упорядочивание выполняются с помощью запроса. Команда `grep` выбирает элементы, содержащие текст RGD, а затем команда `cut` выбирает четвертое поле, чтобы отобразить имя виртуальной машины в выходных данных.</span><span class="sxs-lookup"><span data-stu-id="6165b-146">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="6165b-147">Настройка формата вывода по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6165b-147">Set the default output format</span></span>

<span data-ttu-id="6165b-148">Вы можете использовать интерактивную команду `az configure`, чтобы настроить окружение и выбрать параметры по умолчанию для форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="6165b-148">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="6165b-149">Формат выходных данных по умолчанию — `json`.</span><span class="sxs-lookup"><span data-stu-id="6165b-149">The default output format is `json`.</span></span>

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
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

<span data-ttu-id="6165b-150">Дополнительные сведения о настройке среды см. в [руководстве по конфигурации Azure CLI](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="6165b-150">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
