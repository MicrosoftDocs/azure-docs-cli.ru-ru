---
title: "Результаты выполнения команды запроса в Azure CLI 2.0"
description: "Выполнение запросов JMESPath к результатам команд CLI Azure 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98bc35c1e8136231011a2303901f42c68c9a7758
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="23e80-103">Использование запросов JMESPath в Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="23e80-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="23e80-104">Интерфейс Azure CLI 2.0 использует параметр `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команды `az`.</span><span class="sxs-lookup"><span data-stu-id="23e80-104">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="23e80-105">JMESPath — это эффективный язык запросов для выходных данных JSON.</span><span class="sxs-lookup"><span data-stu-id="23e80-105">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="23e80-106">Если вам не приходилось работать с запросами JMESPath, ознакомьтесь с руководством по адресу [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="23e80-106">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="23e80-107">Параметр `Query` поддерживают все типы ресурсов (службы контейнеров, веб-приложения, виртуальные машины и т.д.) в Azure CLI 2.0, и его можно использовать в различных целях.</span><span class="sxs-lookup"><span data-stu-id="23e80-107">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="23e80-108">Ниже перечислены некоторые примеры.</span><span class="sxs-lookup"><span data-stu-id="23e80-108">We have listed several examples below.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="23e80-109">Выбор простых свойств</span><span class="sxs-lookup"><span data-stu-id="23e80-109">Select simple properties</span></span>

<span data-ttu-id="23e80-110">Простая команда `list` с форматом результатов `table` возвращает проверенный набор наиболее распространенных простых свойств для каждого типа ресурсов в удобном для чтения табличном формате.</span><span class="sxs-lookup"><span data-stu-id="23e80-110">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

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

<span data-ttu-id="23e80-111">Можно использовать параметр `--query`, чтобы отобразить только имя группы ресурсов и имя виртуальной машины для всех виртуальных машин в подписке.</span><span class="sxs-lookup"><span data-stu-id="23e80-111">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query "[].[name, resourceGroup]" --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

<span data-ttu-id="23e80-112">В предыдущем примере вы могли заметить, что заголовки столбцов названы Column1 и Column2.</span><span class="sxs-lookup"><span data-stu-id="23e80-112">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="23e80-113">Вы можете выбрать понятные метки или имена для выбранных свойств.</span><span class="sxs-lookup"><span data-stu-id="23e80-113">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="23e80-114">В следующем примере мы добавили метки VMName и RGName для выбранных свойств name и resourceGroup.</span><span class="sxs-lookup"><span data-stu-id="23e80-114">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="select-complex-nested-properties"></a><span data-ttu-id="23e80-115">Выбор сложных вложенных свойств</span><span class="sxs-lookup"><span data-stu-id="23e80-115">Select complex nested properties</span></span>

<span data-ttu-id="23e80-116">Если вы хотите выбрать свойства, которые глубоко вложены в выходные данные JSON, необходимо указать полный путь к такому свойству.</span><span class="sxs-lookup"><span data-stu-id="23e80-116">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="23e80-117">Следующий пример показывает, как выбрать имя виртуальной машины и тип ОС с помощью команды vm list.</span><span class="sxs-lookup"><span data-stu-id="23e80-117">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="23e80-118">Фильтрация с помощью функции contains</span><span class="sxs-lookup"><span data-stu-id="23e80-118">Filter with the contains function</span></span>

<span data-ttu-id="23e80-119">Можно использовать функцию JMESPath `contains`, чтобы уточнить результаты, которые возвращаются в запросе.</span><span class="sxs-lookup"><span data-stu-id="23e80-119">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="23e80-120">В следующем примере команда выбирает только виртуальные машины, имя которых содержит текст RGD.</span><span class="sxs-lookup"><span data-stu-id="23e80-120">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

<span data-ttu-id="23e80-121">В следующем примере результаты вернут виртуальные машины размера Standard_DS1.</span><span class="sxs-lookup"><span data-stu-id="23e80-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a><span data-ttu-id="23e80-122">Фильтрация с помощью grep</span><span class="sxs-lookup"><span data-stu-id="23e80-122">Filter with grep</span></span>

<span data-ttu-id="23e80-123">Формат результатов `tsv` является текстом, разделенным табуляцией, без заголовков.</span><span class="sxs-lookup"><span data-stu-id="23e80-123">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="23e80-124">Его можно передать в команды `grep` и `cut` для дальнейшего анализа конкретных значений из результатов выполнения команды `list`.</span><span class="sxs-lookup"><span data-stu-id="23e80-124">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="23e80-125">В следующем примере команда `grep` выбирает только виртуальные машины, имя которых содержит текст RGD.</span><span class="sxs-lookup"><span data-stu-id="23e80-125">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="23e80-126">Команда `cut` выбирает только значение восьмого поля (разделенное символами табуляции), чтобы отобразить результаты.</span><span class="sxs-lookup"><span data-stu-id="23e80-126">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="23e80-127">Обзор с jpterm</span><span class="sxs-lookup"><span data-stu-id="23e80-127">Explore with jpterm</span></span>

<span data-ttu-id="23e80-128">Также можно передать результаты выполнения команды в [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) и поэкспериментировать с запросом JMESPath.</span><span class="sxs-lookup"><span data-stu-id="23e80-128">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

