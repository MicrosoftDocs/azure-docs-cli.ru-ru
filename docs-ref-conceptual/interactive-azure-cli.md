---
title: "Интерактивный режим Azure CLI 2.0"
description: "Использование Azure CLI 2.0 в интерактивном режиме."
keywords: "Azure CLI 2.0, интерактивный режим"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 
ms.openlocfilehash: fb260d7385728acd0c699488ecb5b108afefd08c
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2018
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="610c3-104">Интерактивный Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="610c3-104">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="610c3-105">Azure CLI 2.0 можно использовать в интерактивном режиме, выполнив команду `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="610c3-105">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="610c3-106">Она позволяет вызвать интерактивную оболочку, в которой команды завершаются автоматически и предоставляется доступ к описанию команд и их параметров, а также к примерам команд.</span><span class="sxs-lookup"><span data-stu-id="610c3-106">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![Интерактивный режим](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="610c3-108">Здесь мы не используем стиль по умолчанию, который неудобно читать, как и черный фон.</span><span class="sxs-lookup"><span data-stu-id="610c3-108">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="610c3-109">Если вы еще не вошли со своей учетной записью, выполните команду `login`, чтобы сделать это.</span><span class="sxs-lookup"><span data-stu-id="610c3-109">If you're not already logged in to your account, use the `login` command to do that.</span></span>

## <a name="configure"></a><span data-ttu-id="610c3-110">Настройка</span><span class="sxs-lookup"><span data-stu-id="610c3-110">Configure</span></span>

<span data-ttu-id="610c3-111">Интерактивный режим при необходимости позволяет отобразить описание команд, описание параметров и примеры команд.</span><span class="sxs-lookup"><span data-stu-id="610c3-111">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="610c3-112">Отображение описаний и примеров можно включить или отключить с помощью `F1`.</span><span class="sxs-lookup"><span data-stu-id="610c3-112">You can turn descriptions and examples on or off using `F1`.</span></span>

![Описания и примеры](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="610c3-114">Можно включить или отключить отображение значений параметров по умолчанию с помощью `F2`.</span><span class="sxs-lookup"><span data-stu-id="610c3-114">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![Значения по умолчанию](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="610c3-116">`F3` переключает отображение некоторых ключевых жестов.</span><span class="sxs-lookup"><span data-stu-id="610c3-116">`F3` toggles the display of some key gestures.</span></span>

![Жесты](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="610c3-118">Область</span><span class="sxs-lookup"><span data-stu-id="610c3-118">Scope</span></span>

<span data-ttu-id="610c3-119">Вы можете задать область для интерактивного режима, указав определенную группу команд, например `vm` или `vm image`.</span><span class="sxs-lookup"><span data-stu-id="610c3-119">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="610c3-120">При этом будут интерпретироваться все команды в этой области.</span><span class="sxs-lookup"><span data-stu-id="610c3-120">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="610c3-121">Это заметно упрощает работу, если для нее вам требуется определенная группа команд.</span><span class="sxs-lookup"><span data-stu-id="610c3-121">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="610c3-122">Например, требуется ввести следующие команды.</span><span class="sxs-lookup"><span data-stu-id="610c3-122">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="610c3-123">Вместо этого можно задать область для группы команд vm и ввести приведенные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="610c3-123">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="610c3-124">Кроме того, в качестве области можно задать группы команд более низкого уровня.</span><span class="sxs-lookup"><span data-stu-id="610c3-124">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="610c3-125">Для `vm image` можно задать область `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="610c3-125">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="610c3-126">В этом случае, так как мы уже задали `vm` в качестве области, можно было бы использовать `%%image`.</span><span class="sxs-lookup"><span data-stu-id="610c3-126">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="610c3-127">На этом этапе можно указать область `vm`, введя `%%..`, или указать корневой каталог, введя `%%`.</span><span class="sxs-lookup"><span data-stu-id="610c3-127">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="610c3-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="610c3-128">Query</span></span>

<span data-ttu-id="610c3-129">Можно выполнить запрос JMESPath к результатам последней выполненной команды.</span><span class="sxs-lookup"><span data-stu-id="610c3-129">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="610c3-130">Например, после создания виртуальной машины можно убедиться, что она полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="610c3-130">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

<span data-ttu-id="610c3-131">Чтобы узнать больше о выполнении запросов результатов команд, ознакомьтесь с разделом [Использование запросов JMESPath в Azure CLI 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="610c3-131">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="610c3-132">Команды Bash</span><span class="sxs-lookup"><span data-stu-id="610c3-132">Bash commands</span></span>

<span data-ttu-id="610c3-133">Можно выполнять команды оболочки, не выходя из интерактивного режима, с помощью `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="610c3-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="610c3-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="610c3-134">Examples</span></span>

<span data-ttu-id="610c3-135">Некоторые команды имеют множество примеров.</span><span class="sxs-lookup"><span data-stu-id="610c3-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="610c3-136">Вы можете прокрутить экран до следующей странице примеров с помощью `CTRL-N`, а до предыдущей страницы — с помощью `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="610c3-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![Примеры](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="610c3-138">Можно также изучить конкретный пример с помощью `::#`.</span><span class="sxs-lookup"><span data-stu-id="610c3-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
