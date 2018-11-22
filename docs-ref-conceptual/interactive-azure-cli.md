---
title: Интерактивный режим Azure CLI
description: Использование Azure CLI в интерактивном режиме.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: cbfeec67468b8529580c7773883ebfaaa0d0185f
ms.sourcegitcommit: f92d5b3ccd409be126f1e7c06b9f1adc98dad78b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2018
ms.locfileid: "52159309"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="22154-103">Интерактивный режим Azure CLI</span><span class="sxs-lookup"><span data-stu-id="22154-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="22154-104">Azure CLI можно использовать в интерактивном режиме, выполнив команду `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="22154-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="22154-105">В этом режиме открывается интерактивная оболочка с функцией автозавершения, описаниями команд и примерами.</span><span class="sxs-lookup"><span data-stu-id="22154-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![Интерактивный режим](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="22154-107">Здесь мы не используем стиль по умолчанию, который неудобно читать, как и черный фон.</span><span class="sxs-lookup"><span data-stu-id="22154-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="22154-108">Если вы еще не вошли со своей учетной записью, выполните команду `login`.</span><span class="sxs-lookup"><span data-stu-id="22154-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="22154-109">Настройка</span><span class="sxs-lookup"><span data-stu-id="22154-109">Configure</span></span>

<span data-ttu-id="22154-110">Интерактивный режим при необходимости позволяет отобразить описание команд, описание параметров и примеры команд.</span><span class="sxs-lookup"><span data-stu-id="22154-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="22154-111">Отображение описаний и примеров можно включить или отключить с помощью `F1`.</span><span class="sxs-lookup"><span data-stu-id="22154-111">Turn descriptions and examples on or off using `F1`.</span></span>

![Описания и примеры](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="22154-113">Можно включить или отключить отображение значений параметров по умолчанию с помощью `F2`.</span><span class="sxs-lookup"><span data-stu-id="22154-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![Значения по умолчанию](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="22154-115">`F3` переключает отображение некоторых ключевых жестов.</span><span class="sxs-lookup"><span data-stu-id="22154-115">`F3` toggles the display of some key gestures.</span></span>

![Жесты](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="22154-117">Область</span><span class="sxs-lookup"><span data-stu-id="22154-117">Scope</span></span>

<span data-ttu-id="22154-118">Вы можете задать область для интерактивного режима, указав определенную группу команд, например `vm` или `vm image`.</span><span class="sxs-lookup"><span data-stu-id="22154-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="22154-119">При этом будут интерпретироваться все команды в этой области.</span><span class="sxs-lookup"><span data-stu-id="22154-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="22154-120">Это заметно упрощает работу, если для нее вам требуется определенная группа команд.</span><span class="sxs-lookup"><span data-stu-id="22154-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="22154-121">Например, требуется ввести следующие команды.</span><span class="sxs-lookup"><span data-stu-id="22154-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="22154-122">Вместо этого можно задать область для группы команд vm и ввести приведенные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="22154-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="22154-123">Кроме того, в качестве области можно задать группы команд более низкого уровня.</span><span class="sxs-lookup"><span data-stu-id="22154-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="22154-124">Для `vm image` можно задать область `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="22154-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="22154-125">В этом случае, так как мы уже задали `vm` в качестве области, можно было бы использовать `%%image`.</span><span class="sxs-lookup"><span data-stu-id="22154-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="22154-126">На этом этапе можно указать область `vm`, введя `%%..`, или указать корневой каталог, введя `%%`.</span><span class="sxs-lookup"><span data-stu-id="22154-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="22154-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="22154-127">Query</span></span>

<span data-ttu-id="22154-128">Можно выполнить запрос JMESPath к результатам последней выполненной команды.</span><span class="sxs-lookup"><span data-stu-id="22154-128">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="22154-129">Например, после создания виртуальной машины можно убедиться, что она полностью подготовлена.</span><span class="sxs-lookup"><span data-stu-id="22154-129">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> ? [*].provisioningState
```

```json
[
  "Creating"
]
```

<span data-ttu-id="22154-130">Чтобы узнать больше о выполнении запросов к результатам команд в Azure CLI, ознакомьтесь с [этой статьей](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="22154-130">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="22154-131">Команды Bash</span><span class="sxs-lookup"><span data-stu-id="22154-131">Bash commands</span></span>

<span data-ttu-id="22154-132">Можно выполнять команды оболочки, не выходя из интерактивного режима, с помощью `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="22154-132">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="22154-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="22154-133">Examples</span></span>

<span data-ttu-id="22154-134">Некоторые команды имеют множество примеров.</span><span class="sxs-lookup"><span data-stu-id="22154-134">Some commands have lots of examples.</span></span>
<span data-ttu-id="22154-135">Вы можете прокрутить экран до следующей странице примеров с помощью `CTRL-N`, а до предыдущей страницы — с помощью `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="22154-135">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![Примеры](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="22154-137">Можно также изучить конкретный пример с помощью `::#`.</span><span class="sxs-lookup"><span data-stu-id="22154-137">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
