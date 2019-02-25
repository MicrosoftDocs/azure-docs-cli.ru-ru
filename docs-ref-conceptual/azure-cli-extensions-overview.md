---
title: Расширения Azure CLI
description: Использование расширений с Azure CLI
keywords: Azure CLI, расширения
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4f203f94e9b26e1219bfe69ec0ddd73228d30b64
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158876"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="ed339-104">Использование расширений с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ed339-104">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="ed339-105">В Azure CLI можно загружать расширения.</span><span class="sxs-lookup"><span data-stu-id="ed339-105">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="ed339-106">Расширения — это пакеты Python wheel, которые не поставляются вместе с CLI, но выполняются в виде команд CLI.</span><span class="sxs-lookup"><span data-stu-id="ed339-106">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="ed339-107">Расширения позволяют получить доступ к экспериментальным командам и предварительным выпускам команд. Кроме того, расширения позволяют создавать собственные интерфейсы командной строки.</span><span class="sxs-lookup"><span data-stu-id="ed339-107">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="ed339-108">В этой статье описано, как управлять расширениями, и описаны распространенные сценарии их использования.</span><span class="sxs-lookup"><span data-stu-id="ed339-108">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="ed339-109">Поиск расширений</span><span class="sxs-lookup"><span data-stu-id="ed339-109">Find extensions</span></span>

<span data-ttu-id="ed339-110">Список расширений, которые предоставляет и поддерживает Майкрософт, можно просмотреть с помощью команды [az extension list-available](/cli/azure/extension#az-extension-list-available).</span><span class="sxs-lookup"><span data-stu-id="ed339-110">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="ed339-111">[Список расширений](azure-cli-extensions-list.md) также можно найти на веб-сайте с документацией.</span><span class="sxs-lookup"><span data-stu-id="ed339-111">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="ed339-112">Установка расширений</span><span class="sxs-lookup"><span data-stu-id="ed339-112">Install extensions</span></span>

<span data-ttu-id="ed339-113">Когда вы найдете расширение для установки, используйте команду [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add), чтобы получить его.</span><span class="sxs-lookup"><span data-stu-id="ed339-113">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="ed339-114">Если расширение включено в список в `az extension list-available`, его можно установить по имени.</span><span class="sxs-lookup"><span data-stu-id="ed339-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="ed339-115">Если требуется расширение из внешнего ресурса или у вас есть прямая ссылка на него, можно указать URL-адрес источника или локальный путь.</span><span class="sxs-lookup"><span data-stu-id="ed339-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="ed339-116">Расширение _должно_ представлять собой скомпилированный файл Python wheel.</span><span class="sxs-lookup"><span data-stu-id="ed339-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="ed339-117">Установленное расширение можно найти в папке, указанной в переменной среды `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="ed339-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="ed339-118">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="ed339-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="ed339-119">Обновление расширений</span><span class="sxs-lookup"><span data-stu-id="ed339-119">Update extensions</span></span>

<span data-ttu-id="ed339-120">Если расширение установлено с указанием имени, обновите его с помощью команды [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="ed339-120">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="ed339-121">В противном случае расширение можно обновить из источника, выполнив инструкции по [установке расширений](#install-extensions).</span><span class="sxs-lookup"><span data-stu-id="ed339-121">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="ed339-122">Если имя расширения по какой-либо причине не может быть разрешено CLI, удалите это расширение и установите повторно.</span><span class="sxs-lookup"><span data-stu-id="ed339-122">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="ed339-123">Расширение также может стать элементом основного пакета CLI.</span><span class="sxs-lookup"><span data-stu-id="ed339-123">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="ed339-124">Попробуйте обновить CLI, как описано в руководстве по [установке Azure CLI](install-azure-cli.md), и проверьте, добавлены ли команды расширения.</span><span class="sxs-lookup"><span data-stu-id="ed339-124">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="ed339-125">Удаление расширений</span><span class="sxs-lookup"><span data-stu-id="ed339-125">Uninstall extensions</span></span>

<span data-ttu-id="ed339-126">Если расширение больше не нужно, удалите его с помощью команды [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="ed339-126">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="ed339-127">Также расширение можно вручную удалить из расположения, в котором оно установлено.</span><span class="sxs-lookup"><span data-stu-id="ed339-127">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="ed339-128">Переменная среды `$AZURE_EXTENSION_DIR` определяет путь установки модулей.</span><span class="sxs-lookup"><span data-stu-id="ed339-128">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="ed339-129">Если эта переменная не задана, в Linux и macOS по умолчанию устанавливается значение `$HOME/.azure/cliextensions`, а в Windows — `%USERPROFILE%\.azure\cliextensions`.</span><span class="sxs-lookup"><span data-stu-id="ed339-129">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="ed339-130">Часто задаваемые вопросы</span><span class="sxs-lookup"><span data-stu-id="ed339-130">FAQ</span></span>

<span data-ttu-id="ed339-131">Ниже приведены ответы на некоторые часто задаваемые вопросы о расширениях CLI.</span><span class="sxs-lookup"><span data-stu-id="ed339-131">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="ed339-132">Какие форматы файлов разрешены для установки?</span><span class="sxs-lookup"><span data-stu-id="ed339-132">What file formats are allowed for installation?</span></span>

<span data-ttu-id="ed339-133">Сейчас в качестве расширений можно устанавливать только wheel-файлы Python.</span><span class="sxs-lookup"><span data-stu-id="ed339-133">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="ed339-134">Могут ли расширения заменить существующие команды?</span><span class="sxs-lookup"><span data-stu-id="ed339-134">Can extensions replace existing commands?</span></span>

<span data-ttu-id="ed339-135">Да.</span><span class="sxs-lookup"><span data-stu-id="ed339-135">Yes.</span></span> <span data-ttu-id="ed339-136">Расширения могут заменить существующие команды. Но перед выполнением замененной команды в CLI отобразится предупреждение.</span><span class="sxs-lookup"><span data-stu-id="ed339-136">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="ed339-137">Как понять, что расширение выпущено в предварительной версии?</span><span class="sxs-lookup"><span data-stu-id="ed339-137">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="ed339-138">В документации по расширению и формате версии будет указано, является ли оно предварительным выпуском.</span><span class="sxs-lookup"><span data-stu-id="ed339-138">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="ed339-139">Майкрософт часто выпускает предварительные версии команд в виде расширений CLI с возможностью последующего включения в основной продукт CLI.</span><span class="sxs-lookup"><span data-stu-id="ed339-139">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="ed339-140">Когда команды больше не являются расширениями, старое расширение следует удалить.</span><span class="sxs-lookup"><span data-stu-id="ed339-140">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="ed339-141">Могут ли расширения зависеть друг от друга?</span><span class="sxs-lookup"><span data-stu-id="ed339-141">Can extensions depend upon each other?</span></span>

<span data-ttu-id="ed339-142">№</span><span class="sxs-lookup"><span data-stu-id="ed339-142">No.</span></span> <span data-ttu-id="ed339-143">Так как CLI не гарантирует порядок загрузки, зависимости могут быть не удовлетворены.</span><span class="sxs-lookup"><span data-stu-id="ed339-143">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="ed339-144">Удаление одного расширения не влияет на другие.</span><span class="sxs-lookup"><span data-stu-id="ed339-144">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="ed339-145">Обновляются ли расширения вместе с CLI?</span><span class="sxs-lookup"><span data-stu-id="ed339-145">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="ed339-146">№</span><span class="sxs-lookup"><span data-stu-id="ed339-146">No.</span></span> <span data-ttu-id="ed339-147">Расширения следует обновлять отдельно, как описано в разделе [Обновление расширений](#update-extensions).</span><span class="sxs-lookup"><span data-stu-id="ed339-147">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>
