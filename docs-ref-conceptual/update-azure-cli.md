---
title: Обновление Azure CLI
description: Справочник по обновлению Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 475b58bca5ec9dca52a70416cb89860dcbd39278
ms.sourcegitcommit: e1faf297ba2cdf2ba7e821fbeedff9c9a724c975
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "97576791"
---
# <a name="update-the-azure-cli"></a>Обновление Azure CLI

Для обновления локальной установки Azure CLI в средах Windows, macOS и Linux (см. раздел `Update` в инструкциях по установке для конкретной платформы) можно использовать диспетчер пакетов. CLI также предоставляет встроенные команды для обновления вручную или автоматического обновления.

## <a name="manual-update"></a>Обновление вручную
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

`az upgrade` поддерживается в Windows, macOS и некоторых дистрибутивах Linux, если поддерживается сама установка. При этом можно выполнить только обновление до последней версии. Если вы используете Azure CLI в Azure Cloud Shell, скорее всего, вы уже используете самую последнюю установку Azure CLI. Кроме ситуаций с исправлением незначительной ошибки в дополнительной версии, необходимо дождаться выпуска следующей сборки Azure Cloud Shell, так как Azure Cloud Shell не поддерживает `az upgrade`.

Если `azure-cli` уже является последней версией, при выполнении `az upgrade` будут проверены и обновлены все установленные [расширения](azure-cli-extensions-overview.md).

## <a name="automatic-update"></a>Автоматическое обновление

По умолчанию автоматическое обновление для Azure CLI отключено. Чтобы включить автоматическое обновление до последней версии, нужно изменить [конфигурацию](/cli/azure/config).

```azurecli
az config set auto-upgrade.enable=yes
```

Azure CLI будет регулярно проверять наличие новых версий и предлагать вам обновить систему после выполнения любой команды, когда обновление станет доступным.

Появление сообщения с запросом или выходных сообщений во время обновления может привести к прерыванию выполнения команды, если она назначена переменной или выполняется в потоке автоматически. Чтобы избежать прерывания, можно использовать приведенную ниже конфигурацию. Она обеспечит автоматическое обновление без подтверждения. Во время обновления будут отображаться только предупреждения и сообщения об ошибках.

```azurecli
az config set auto-upgrade.prompt=no
```

По умолчанию все установленные расширения также будут обновлены. Вы можете отключить обновление расширений, изменив конфигурацию.

```azurecli
az config set auto-upgrade.all=no
```

> [!NOTE]
> Дождитесь завершения выполнения `az upgrade`, прежде чем переходить к следующему набору команд. Иначе новые версии CLI (и расширения) могут включать критические изменения.

Если вы решили не использовать функцию автоматического обновления (например, если вам нужно сохранить стабильное выполнение командных скриптов), ее можно отключить, изменив конфигурацию.
```azurecli
az config set auto-upgrade.enable=no
```