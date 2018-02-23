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
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Использование запросов JMESPath в Azure CLI 2.0

Интерфейс Azure CLI 2.0 использует параметр `--query` для выполнения [запроса JMESPath](http://jmespath.org) к результатам выполнения команды `az`. JMESPath — это эффективный язык запросов для выходных данных JSON.  Если вам не приходилось работать с запросами JMESPath, ознакомьтесь с руководством по адресу [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).

Параметр `Query` поддерживают все типы ресурсов (службы контейнеров, веб-приложения, виртуальные машины и т.д.) в Azure CLI 2.0, и его можно использовать в различных целях.  Ниже перечислены некоторые примеры.

## <a name="select-simple-properties"></a>Выбор простых свойств

Простая команда `list` с форматом результатов `table` возвращает проверенный набор наиболее распространенных простых свойств для каждого типа ресурсов в удобном для чтения табличном формате.

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

Можно использовать параметр `--query`, чтобы отобразить только имя группы ресурсов и имя виртуальной машины для всех виртуальных машин в подписке.

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

В предыдущем примере вы могли заметить, что заголовки столбцов названы Column1 и Column2.  Вы можете выбрать понятные метки или имена для выбранных свойств.  В следующем примере мы добавили метки VMName и RGName для выбранных свойств name и resourceGroup.


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

## <a name="select-complex-nested-properties"></a>Выбор сложных вложенных свойств

Если вы хотите выбрать свойства, которые глубоко вложены в выходные данные JSON, необходимо указать полный путь к такому свойству. Следующий пример показывает, как выбрать имя виртуальной машины и тип ОС с помощью команды vm list.

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

## <a name="filter-with-the-contains-function"></a>Фильтрация с помощью функции contains

Можно использовать функцию JMESPath `contains`, чтобы уточнить результаты, которые возвращаются в запросе.
В следующем примере команда выбирает только виртуальные машины, имя которых содержит текст RGD.

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

В следующем примере результаты вернут виртуальные машины размера Standard_DS1.

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

## <a name="filter-with-grep"></a>Фильтрация с помощью grep

Формат результатов `tsv` является текстом, разделенным табуляцией, без заголовков. Его можно передать в команды `grep` и `cut` для дальнейшего анализа конкретных значений из результатов выполнения команды `list`. В следующем примере команда `grep` выбирает только виртуальные машины, имя которых содержит текст RGD.  Команда `cut` выбирает только значение восьмого поля (разделенное символами табуляции), чтобы отобразить результаты.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Обзор с jpterm

Также можно передать результаты выполнения команды в [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) и поэкспериментировать с запросом JMESPath.

```bash
pip install jmespath-terminal
az vm list | jpterm
```

