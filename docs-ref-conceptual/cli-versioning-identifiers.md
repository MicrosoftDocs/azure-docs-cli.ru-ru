---
title: Различия между продуктами Azure CLI
description: Сведения о наименовании, нумерации версий и обновлении продуктов Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/12/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a39f6b0fbccf937aec2b227ed4e3f4ff8d92137f
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593104"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="04abe-103">Различия между продуктами Azure CLI</span><span class="sxs-lookup"><span data-stu-id="04abe-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="04abe-104">В конце июня 2018 года из названий продуктов Azure CLI убраны указываемые явным образом номера версий.</span><span class="sxs-lookup"><span data-stu-id="04abe-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="04abe-105">Это изменение поможет избежать путаницы, которая иногда возникает в документации, когда пользователям рекомендуется использовать Azure CLI, но непонятно, о какой версии продукта идет речь.</span><span class="sxs-lookup"><span data-stu-id="04abe-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="04abe-106">Если вы знакомы со старыми названиями продуктов, ниже описано, как они изменились:</span><span class="sxs-lookup"><span data-stu-id="04abe-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="04abe-107">Azure CLI 2.0 и более поздних версий теперь называется просто "Azure CLI".</span><span class="sxs-lookup"><span data-stu-id="04abe-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="04abe-108">Старые версии Azure CLI (версия 1.х и более ранние) теперь называются "классический интерфейс командной строки Azure" (Azure classic CLI).</span><span class="sxs-lookup"><span data-stu-id="04abe-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="04abe-109">Изменение названия на "классический интерфейс командной строки Azure" призвано продемонстрировать, что этот инструмент предназначен для использования только с классической моделью развертывания.</span><span class="sxs-lookup"><span data-stu-id="04abe-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="04abe-110">Обновление и поддержка классического интерфейса командной строки Azure больше не осуществляется.</span><span class="sxs-lookup"><span data-stu-id="04abe-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="04abe-111">По этой и ряду других причин рекомендуется перевести классические развертывания на использование модели Azure Resource Manager и выполнить миграцию на последнюю доступную версию Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="04abe-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="04abe-112">Если вы по-прежнему используете классический интерфейс командной строки, сведения о процессе миграции можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="04abe-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="04abe-113">Переход с классической модели развертывания на модель Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="04abe-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="04abe-114">Установка Azure CLI</span><span class="sxs-lookup"><span data-stu-id="04abe-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* [<span data-ttu-id="04abe-115">Поддерживаемый платформой перенос ресурсов IaaS из классической модели в модель Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="04abe-115">Migrating from Azure classic CLI to Azure CLI</span></span>](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
