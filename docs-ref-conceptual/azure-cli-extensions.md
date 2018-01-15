---
title: "Расширения Azure CLI 2.0"
description: "Использование расширений с Azure CLI 2.0"
keywords: "Azure CLI, расширения"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a76e58c4430a184d133cca0ef0623f325aeb2f27
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2018
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="ea236-104">Использование расширений с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ea236-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="ea236-105">Расширения — это отдельные модули, которые не входят в состав Azure CLI. Они позволяют добавлять функциональные возможности с помощью новых команд.</span><span class="sxs-lookup"><span data-stu-id="ea236-105">Extensions are individual modules not shipped with the Azure CLI itself that allow you to add functionality through new commands.</span></span> <span data-ttu-id="ea236-106">Это могут быть предложения в экспериментальной или предварительной версии, специализированные средства, предоставляемые корпорацией Майкрософт в соответствии с вашими требованиями, или даже расширения, которые вы написали самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="ea236-106">These might be experimental or pre-release offerings, specialized tools that Microsoft has for your needs, or even extensions that you yourself have written.</span></span> <span data-ttu-id="ea236-107">Расширения повышают гибкость работы с CLI, позволяя адаптировать интерфейс для определенных целей. При этом не требуется передавать большое число дополнительных пакетов, которые не входят в набор основных компонентов.</span><span class="sxs-lookup"><span data-stu-id="ea236-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="ea236-108">Из этой статьи вы узнаете, как устанавливать, обновлять и удалять расширения для CLI.</span><span class="sxs-lookup"><span data-stu-id="ea236-108">This article will help you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="ea236-109">Кроме того, здесь содержатся ответы на часто задаваемые вопросы о поведении расширений.</span><span class="sxs-lookup"><span data-stu-id="ea236-109">It should also answer common questions about extension behavior.</span></span>

## <a name="finding-extensions"></a><span data-ttu-id="ea236-110">Поиск расширений</span><span class="sxs-lookup"><span data-stu-id="ea236-110">Finding extensions</span></span>

<span data-ttu-id="ea236-111">Чтобы узнать, какие расширения доступны, вы можете использовать `az extension list-available`.</span><span class="sxs-lookup"><span data-stu-id="ea236-111">In order to know what extensions are available, you can use `az extension list-available`.</span></span> <span data-ttu-id="ea236-112">Это команда для перечисления доступных официальных расширений, которые предоставляются и поддерживаются корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ea236-112">This command lists the available, official extensions which are provided and supported by Microsoft.</span></span>

## <a name="installing-extensions"></a><span data-ttu-id="ea236-113">Установка расширений</span><span class="sxs-lookup"><span data-stu-id="ea236-113">Installing extensions</span></span>

<span data-ttu-id="ea236-114">Когда вы найдете расширение для установки, используйте `az extension add`, чтобы получить его.</span><span class="sxs-lookup"><span data-stu-id="ea236-114">Once you have found an extension to install, use `az extension add` to get it.</span></span> <span data-ttu-id="ea236-115">Официальное расширение Майкрософт из списка `az extension list-available` можно установить по имени.</span><span class="sxs-lookup"><span data-stu-id="ea236-115">If the extension is an official Microsoft extension listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli
az extension add --name <extension-name>
```

<span data-ttu-id="ea236-116">Если требуется расширение из внешнего ресурса или у вас есть прямая ссылка на него, можно указать URL-адрес источника или локальный путь.</span><span class="sxs-lookup"><span data-stu-id="ea236-116">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="ea236-117">Это _должен_ быть скомпилированный wheel-файл Python.</span><span class="sxs-lookup"><span data-stu-id="ea236-117">This _must_ be a compiled Python wheel file.</span></span>

```azurecli
az extension add --source <URL-or-path>
```

<span data-ttu-id="ea236-118">После установки расширения сведения о нем отображаются в значении переменной оболочки `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="ea236-118">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="ea236-119">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="ea236-119">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="updating-extensions"></a><span data-ttu-id="ea236-120">Обновление расширений</span><span class="sxs-lookup"><span data-stu-id="ea236-120">Updating extensions</span></span>

<span data-ttu-id="ea236-121">Расширения можно обновлять только по имени.</span><span class="sxs-lookup"><span data-stu-id="ea236-121">Extensions can only be updated by name:</span></span>

```azurecli
az extension update --name <extension-name>
```

<span data-ttu-id="ea236-122">Если имя расширения по какой-либо причине не разрешается CLI, повторно установите расширение, чтобы обновить его.</span><span class="sxs-lookup"><span data-stu-id="ea236-122">If an extension name cannot be resolved by the CLI for whatever reason, reinstall the extension to update it.</span></span> <span data-ttu-id="ea236-123">Также есть вероятность, что расширение, которое предоставлялось в предварительной версии, теперь является встроенной командой для CLI.</span><span class="sxs-lookup"><span data-stu-id="ea236-123">There is also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="ea236-124">В таком случае обновите CLI и удалите расширение.</span><span class="sxs-lookup"><span data-stu-id="ea236-124">In that case, update the CLI and uninstall the extension.</span></span>

## <a name="uninstalling-extensions"></a><span data-ttu-id="ea236-125">Удаление расширений</span><span class="sxs-lookup"><span data-stu-id="ea236-125">Uninstalling extensions</span></span>

<span data-ttu-id="ea236-126">Если расширение больше не требуется, можно удалить его с помощью `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="ea236-126">If you no longer need an extension, it can be removed with `az extension remove`,</span></span>

```azurecli
az extension remove --name <extension-name>
```

<span data-ttu-id="ea236-127">Также расширение можно вручную удалить из расположения, в котором оно установлено.</span><span class="sxs-lookup"><span data-stu-id="ea236-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="ea236-128">Для переменной оболочки устанавливается значение `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="ea236-128">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="ea236-129">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="ea236-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="ea236-130">Для удаления рекомендуется использовать `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="ea236-130">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="ea236-131">Часто задаваемые вопросы</span><span class="sxs-lookup"><span data-stu-id="ea236-131">FAQ</span></span>

<span data-ttu-id="ea236-132">Ниже приведены ответы на некоторые часто задаваемые вопросы о расширениях CLI.</span><span class="sxs-lookup"><span data-stu-id="ea236-132">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="ea236-133">Какие форматы файлов разрешены для установки?</span><span class="sxs-lookup"><span data-stu-id="ea236-133">What file formats are allowed for installation?</span></span>

<span data-ttu-id="ea236-134">Сейчас в качестве расширений можно устанавливать только wheel-файлы Python.</span><span class="sxs-lookup"><span data-stu-id="ea236-134">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="ea236-135">Могут ли расширения заменить существующие команды?</span><span class="sxs-lookup"><span data-stu-id="ea236-135">Can extensions replace existing commands?</span></span>

<span data-ttu-id="ea236-136">Да.</span><span class="sxs-lookup"><span data-stu-id="ea236-136">Yes.</span></span> <span data-ttu-id="ea236-137">Расширения могут заменить существующие команды. Но перед выполнением замененной команды в CLI отобразится предупреждение.</span><span class="sxs-lookup"><span data-stu-id="ea236-137">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="ea236-138">Как понять, что расширение выпущено в предварительной версии?</span><span class="sxs-lookup"><span data-stu-id="ea236-138">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="ea236-139">Если расширение предоставляется в предварительной версии, в документации и сведениях о версии расширения должно содержаться соответствующее указание.</span><span class="sxs-lookup"><span data-stu-id="ea236-139">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="ea236-140">Кроме того, в качестве расширений корпорация Майкрософт часто выпускает предварительные версии команд, которые в дальнейшем планируется перенести в основной интерфейс CLI.</span><span class="sxs-lookup"><span data-stu-id="ea236-140">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="ea236-141">Могут ли расширения зависеть друг от друга?</span><span class="sxs-lookup"><span data-stu-id="ea236-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="ea236-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea236-142">No.</span></span> <span data-ttu-id="ea236-143">Расширения должны быть отдельными не зависящими друг от друга пакетами.</span><span class="sxs-lookup"><span data-stu-id="ea236-143">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="ea236-144">CLI не дает гарантий относительно того, когда будет загружено то или иное расширение. Поэтому нельзя гарантировать и соблюдение зависимостей.</span><span class="sxs-lookup"><span data-stu-id="ea236-144">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="ea236-145">Устанавливается только одно конкретное расширение, и оно должно продолжать работать, даже если вы удалите другие расширения.</span><span class="sxs-lookup"><span data-stu-id="ea236-145">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="ea236-146">Обновляются ли расширения вместе с CLI?</span><span class="sxs-lookup"><span data-stu-id="ea236-146">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="ea236-147">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea236-147">No.</span></span> <span data-ttu-id="ea236-148">Расширения следует обновлять отдельно, как описано в разделе [Обновление расширений](#updating-extensions).</span><span class="sxs-lookup"><span data-stu-id="ea236-148">Extensions must be updated separately, as described in the [Updating extensions](#updating-extensions) section.</span></span>
