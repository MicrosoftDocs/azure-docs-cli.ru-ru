---
title: Расширения Azure CLI 2.0
description: Использование расширений с Azure CLI 2.0
keywords: Azure CLI, расширения
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1b983faef4c1678763b3483192e94a6c96e24f32
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2018
ms.locfileid: "34479487"
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="e75d9-104">Использование расширений с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e75d9-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="e75d9-105">Расширения — это отдельные модули, которые не входят в состав Azure CLI. Они позволяют добавлять функциональные возможности с помощью новых команд.</span><span class="sxs-lookup"><span data-stu-id="e75d9-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="e75d9-106">Это могут быть предложения в экспериментальной или предварительной версии, специализированные средства от Майкрософт или пользовательские решения, которые вы написали самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="e75d9-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="e75d9-107">Расширения повышают гибкость работы с CLI, позволяя адаптировать интерфейс для определенных целей. При этом не требуется передавать большое число дополнительных пакетов, которые не входят в набор основных компонентов.</span><span class="sxs-lookup"><span data-stu-id="e75d9-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="e75d9-108">Из этой статьи вы узнаете, как устанавливать, обновлять и удалять расширения для CLI.</span><span class="sxs-lookup"><span data-stu-id="e75d9-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="e75d9-109">Кроме того, здесь содержатся ответы на часто задаваемые вопросы о поведении расширений.</span><span class="sxs-lookup"><span data-stu-id="e75d9-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="e75d9-110">Поиск расширений</span><span class="sxs-lookup"><span data-stu-id="e75d9-110">Find extensions</span></span>

<span data-ttu-id="e75d9-111">Чтобы узнать, какие расширения доступны, вы можете использовать команду [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="e75d9-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="e75d9-112">Это команда отображает список доступных официальных расширений, которые предоставляются и обслуживаются корпорацией Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e75d9-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="e75d9-113">Мы также добавили [список расширений Microsoft](azure-cli-extensions-list.md) на сайт с документацией.</span><span class="sxs-lookup"><span data-stu-id="e75d9-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="e75d9-114">Установка расширений</span><span class="sxs-lookup"><span data-stu-id="e75d9-114">Install extensions</span></span>

<span data-ttu-id="e75d9-115">Когда вы найдете расширение для установки, используйте команду [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add), чтобы получить его.</span><span class="sxs-lookup"><span data-stu-id="e75d9-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="e75d9-116">Если расширение включено в список в `az extension list-available`, его можно установить по имени.</span><span class="sxs-lookup"><span data-stu-id="e75d9-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="e75d9-117">Если требуется расширение из внешнего ресурса или у вас есть прямая ссылка на него, можно указать URL-адрес источника или локальный путь.</span><span class="sxs-lookup"><span data-stu-id="e75d9-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="e75d9-118">Это _должен_ быть скомпилированный wheel-файл Python.</span><span class="sxs-lookup"><span data-stu-id="e75d9-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="e75d9-119">После установки расширения сведения о нем отображаются в значении переменной оболочки `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="e75d9-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="e75d9-120">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="e75d9-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="e75d9-121">Обновление расширений</span><span class="sxs-lookup"><span data-stu-id="e75d9-121">Update extensions</span></span>

<span data-ttu-id="e75d9-122">Если расширение устанавливалось по имени, его можно обновить с помощью команды [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="e75d9-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="e75d9-123">В противном случае расширение можно обновить из источника, выполнив инструкции по [установке расширений](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="e75d9-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="e75d9-124">Если имя расширения по какой-либо причине не разрешается с помощью CLI, удалите его и установите повторно.</span><span class="sxs-lookup"><span data-stu-id="e75d9-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="e75d9-125">Также есть вероятность, что расширение, которое предоставлялось в режиме предварительной версии, теперь является встроенной командой CLI.</span><span class="sxs-lookup"><span data-stu-id="e75d9-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="e75d9-126">Попробуйте обновить CLI, как описано в руководстве по [установке CLI Azure 2.0](install-azure-cli.md), и проверьте, добавлены ли команды расширения.</span><span class="sxs-lookup"><span data-stu-id="e75d9-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="e75d9-127">Удаление расширений</span><span class="sxs-lookup"><span data-stu-id="e75d9-127">Uninstall extensions</span></span>

<span data-ttu-id="e75d9-128">Если расширение больше не нужно, можно удалить его с помощью команды [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="e75d9-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="e75d9-129">Также расширение можно вручную удалить из расположения, в котором оно установлено.</span><span class="sxs-lookup"><span data-stu-id="e75d9-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="e75d9-130">Для переменной оболочки устанавливается значение `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="e75d9-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="e75d9-131">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="e75d9-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="e75d9-132">Для удаления рекомендуется использовать `az extension remove`.</span><span class="sxs-lookup"><span data-stu-id="e75d9-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="e75d9-133">Часто задаваемые вопросы</span><span class="sxs-lookup"><span data-stu-id="e75d9-133">FAQ</span></span>

<span data-ttu-id="e75d9-134">Ниже приведены ответы на некоторые часто задаваемые вопросы о расширениях CLI.</span><span class="sxs-lookup"><span data-stu-id="e75d9-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="e75d9-135">Какие форматы файлов разрешены для установки?</span><span class="sxs-lookup"><span data-stu-id="e75d9-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="e75d9-136">Сейчас в качестве расширений можно устанавливать только wheel-файлы Python.</span><span class="sxs-lookup"><span data-stu-id="e75d9-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="e75d9-137">Могут ли расширения заменить существующие команды?</span><span class="sxs-lookup"><span data-stu-id="e75d9-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="e75d9-138">Да.</span><span class="sxs-lookup"><span data-stu-id="e75d9-138">Yes.</span></span> <span data-ttu-id="e75d9-139">Расширения могут заменить существующие команды. Но перед выполнением замененной команды в CLI отобразится предупреждение.</span><span class="sxs-lookup"><span data-stu-id="e75d9-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="e75d9-140">Как понять, что расширение выпущено в предварительной версии?</span><span class="sxs-lookup"><span data-stu-id="e75d9-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="e75d9-141">Если расширение предоставляется в предварительной версии, в документации и сведениях о версии расширения должно содержаться соответствующее указание.</span><span class="sxs-lookup"><span data-stu-id="e75d9-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="e75d9-142">Кроме того, в качестве расширений корпорация Майкрософт часто выпускает предварительные версии команд, которые в дальнейшем планируется перенести в основной интерфейс CLI.</span><span class="sxs-lookup"><span data-stu-id="e75d9-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="e75d9-143">Могут ли расширения зависеть друг от друга?</span><span class="sxs-lookup"><span data-stu-id="e75d9-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="e75d9-144">Нет.</span><span class="sxs-lookup"><span data-stu-id="e75d9-144">No.</span></span> <span data-ttu-id="e75d9-145">Расширения должны быть отдельными не зависящими друг от друга пакетами.</span><span class="sxs-lookup"><span data-stu-id="e75d9-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="e75d9-146">CLI не дает гарантий относительно того, когда будет загружено то или иное расширение. Поэтому нельзя гарантировать и соблюдение зависимостей.</span><span class="sxs-lookup"><span data-stu-id="e75d9-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="e75d9-147">Устанавливается только одно конкретное расширение, и оно должно продолжать работать, даже если вы удалите другие расширения.</span><span class="sxs-lookup"><span data-stu-id="e75d9-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="e75d9-148">Обновляются ли расширения вместе с CLI?</span><span class="sxs-lookup"><span data-stu-id="e75d9-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="e75d9-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="e75d9-149">No.</span></span> <span data-ttu-id="e75d9-150">Расширения следует обновлять отдельно, как описано в разделе [Обновление расширений](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="e75d9-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
