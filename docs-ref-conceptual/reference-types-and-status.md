---
title: Типы ссылок Azure CLI
description: Описание типов и состояний ссылок
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/14/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2b6b3c5faef66e714cddf7b07126ba14af8c149b
ms.sourcegitcommit: fd8c3e32f0f50feb6fea33ead636a80a050bcf2a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "88714354"
---
# <a name="overview-azure-cli-reference-types-and-status"></a>Общие сведения. Типы и состояния ссылок Azure CLI

В Azure CLI используются разные типы ссылок, которые иногда называются состояниями ссылок.  В этой статье рассказывается, в чем состоит разница между типом и состоянием Azure CLI.

## <a name="azure-cli-syntax-components"></a>Компоненты синтаксиса Azure CLI

Синтаксис Azure CLI представляет собой сочетание ссылок, команд и параметров.  Часто команда полной ссылки называется просто **командой**.

| Служба Azure | Справочник | Подслужба ссылки | Get-Help | Команда полной ссылки | Примеры параметров
|-|-|-|-|-|-|
| Azure CLI | [az configure](/cli/azure/reference-index#az-configure) | | | az configure | --defaults, --list-default, --scope
| Сеть Azure | [az network](/cli/azure/network) | application-gateway | create | [az network application-gateway create](/cli/azure/network/application-gateway#az-network-application-gateway-create) | --name, --resource-group, --capacity
| Azure DevOps | [az pipelines](/cli/azure/pipelines) | агент | list | [az pipelines agent list](/cli/azure/pipelines/agent) | --pool-id, --agent-name, --demands

## <a name="reference-types"></a>Ссылочные типы

Тип ссылки указывает на то, является ли команда ссылки частью основной службы Azure CLI или необязательной надстройкой.  Есть два типа команд ссылок Azure CLI: **основные команды** и **команды расширения**.

|         | Основные сведения  | Расширение
|-|-|-|
| **Справочные материалы** | Являются частью основной службы Azure CLI. | Являются необязательными командами ссылки, которые должны быть установлены.
| **Установка** | Совместно с помощью установщика [MSI](). | Отдельно с помощью [az extension add]().|
| **Выпущено** | По расписанию. | По мере появления новых функций или обновлений.
| **Состояние** | Могут быть общедоступными, предварительными или экспериментальными. | Также могут быть общедоступными, предварительными или экспериментальными.

Все ссылки Azure CLI могут выполняться в Windows, macOS, Linux, Docker и Azure Cloud Shell.

### <a name="core"></a>Основные сведения

Ссылки Azure CLI, опубликованные как постоянная часть CLI, называются **основными ссылками**.  Все основные ссылки устанавливаются с Azure CLI. Вы не можете выбрать нужный набор ссылок.  Если вы запускаете CLI с помощью Azure Cloud Shell, основные ссылки всегда будут актуальными.  См. полный список [основных ссылок Azure CLI](/cli/azure/reference-index).

### <a name="extension"></a>Расширение

Расширения не поставляются вместе с CLI, но выполняются в виде команд CLI.  Некоторые расширения являются постоянной частью Azure CLI, но зачастую расширение предоставляет доступ к командам закрытой предварительной версии и экспериментальным командам.  Одна ссылка, например **az iot hub**, может иметь как основные команды, так и команды расширения.  Рассмотрим четыре примера.

| Команда полной ссылки | Основная команда | Команда расширения
|-|-|-|
| az iot hub list | да |
| az iot hub query | | да
| az iot hub certificate create | да |
| az iot hub device identify create | | да

> [!IMPORTANT]
> Прежде чем использовать команду [az extension add](/cli/azure/extension#az-extension-add), необходимо установить расширение.

Сведения о расширениях, включая инструкции по их установке и обновлении, см. в статье [Использование расширений с Azure CLI](azure-cli-extensions-overview.md).  Чтобы оптимизировать работу, просмотрите эту [вики-страницу с советами](https://github.com/Azure/azure-network-cli-extension/wiki/Tips).  Полный список команд расширения см. в статье [Доступные расширения для Azure CLI](azure-cli-extensions-list.md).

## <a name="reference-status"></a>Состояние ссылки

Независимо от типа ссылки Azure CLI делятся на три категории состояния: **общедоступная версия**, **общедоступная предварительная версия** и **экспериментальная версия**.  Это не тип, а состояние команды ссылки, которое определяет уровень стабильности и поддержки.

| | GA  | Общедоступная предварительная версия | Экспериментальный
|-|-|-|-|
| **Стабильность** | Постоянно | В соответствии с условиями [использования предварительных версий продуктов Microsoft Azure](/support/legal/preview-supplemental-terms/). | Становится общедоступной предварительной версией или удаляется.
| **Уровень поддержки** | Полное | Partial | Нет

Хотя большинство команд и параметров для одной ссылки имеют одно состояние, это не всегда так.  Общедоступная ссылка, которая создается для предоставления дополнительных команд, может иметь общедоступные, предварительные и экспериментальные версии команд ссылок.  Обычно в ответ на предоставляемые отзывы или при добавлении новых параметров для повышения функциональности одна команда также может иметь параметры, которые используются в разных категориях состояния.  Ниже приведены примеры ссылок с разными состояниями.

| Команда полной ссылки | Параметры | Тип | GA | Общедоступная предварительная версия | Экспериментальный
|-|-|-|-|-|-|
| az network dns zone list | Все | Основные сведения | да |
| az network dns zone create | --name, --resource-group, --if-none-match, --parent-name | Основные сведения | да |
|  | --newFutureParameter1 | Основные сведения | | да
|  | --newFutureParameter2 | Основные сведения | | | да
| az network vhub list | Все |Расширение | да
| az network vhub create | --address-prefix, --name, --resource-group, -vwan, --location, --sku |Расширение | да
|  | --newFutureParameter1 |Расширение | | да
|  | --newFutureParameter2|Расширение | | | да
| az network firewall create | Все | Расширение | | | да

> [!NOTE]
> Предупреждения, информирующие об использовании **общедоступной предварительной версии** или **экспериментальной версии**, являются частью выходных данных команды Azure CLI и не должны вызывать беспокойство.

## <a name="see-also"></a>См. также раздел

- [Список основных ссылок для Azure CLI](/cli/azure/reference-index)
- [Доступные расширения для Azure CLI](azure-cli-extensions-list.md)
