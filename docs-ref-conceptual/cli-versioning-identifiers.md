---
title: Различия между продуктами Azure CLI
description: Сведения о наименовании, нумерации версий и обновлении продуктов Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/12/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 93dd6fd3e026713779768d1ae4b4873f658d2898
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562555"
---
# <a name="differences-between-azure-cli-products"></a>Различия между продуктами Azure CLI

В конце июня 2018 года из названий продуктов Azure CLI убраны указываемые явным образом номера версий. Это изменение поможет избежать путаницы, которая иногда возникает в документации, когда пользователям рекомендуется использовать Azure CLI, но непонятно, о какой версии продукта идет речь. Если вы знакомы со старыми названиями продуктов, ниже описано, как они изменились:

* Azure CLI 2.0 и более поздних версий теперь называется просто "Azure CLI".
* Старые версии Azure CLI (версия 1.х и более ранние) теперь называются "классический интерфейс командной строки Azure" (Azure classic CLI).

Изменение названия на "классический интерфейс командной строки Azure" призвано продемонстрировать, что этот инструмент предназначен для использования только с классической моделью развертывания. Обновление и поддержка классического интерфейса командной строки Azure больше не осуществляется. По этой и ряду других причин рекомендуется перевести классические развертывания на использование модели Azure Resource Manager и выполнить миграцию на последнюю доступную версию Azure CLI.

Если вы по-прежнему используете классический интерфейс командной строки, сведения о процессе миграции можно найти в следующих статьях:

* [Переход с классической модели развертывания на модель Azure Resource Manager](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [Установка Azure CLI](install-azure-cli.md)
* [Поддерживаемый платформой перенос ресурсов IaaS из классической модели в модель Azure Resource Manager](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)
