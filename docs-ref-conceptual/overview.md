---
title: "Azure CLI 2.0"
description: "Общие сведения об Azure CLI 2.0."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 80ae9f6c-adb7-483c-bfb4-fbb958e075ba
ms.openlocfilehash: 35e754b4ecd75481bd60d95dd1545b798c2e85b3
ms.sourcegitcommit: c077bd5cbe07f7225714c41714d3981fa0d9928f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2017
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Azure CLI 2.0 — это новый интерфейс командной строки Azure для управления ресурсами Azure.  Его можно использовать в Windows, Linux и macOS. 

Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager. С помощью Azure CLI 2.0 можно легко создавать виртуальные машины в Azure простым вводом следующей команды:

```azurecli
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Ознакомьтесь со [статьей об установке](install-azure-cli.md), чтобы установить и запустить Azure CLI 2.0 в своей системе, или воспользуйтесь [Cloud Shell](/azure/cloud-shell/overview), чтобы запустить интерфейс командной строки в браузере.
Прежде чем начать использовать интерфейс командной строки, прочтите статью о [начале работы](get-started-with-azure-cli.md).
Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).

Приведенные ниже примеры помогут вам понять, как реализовать типичные сценарии с помощью Azure CLI 2.0:
- [Виртуальные машины Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Виртуальные машины Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Веб-приложения](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [База данных SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

В подробной [справочной информации](/cli/azure/) также описаны способы использования каждой отдельной команды Azure CLI 2.0.

[Начните использовать](get-started-with-azure-cli.md) Azure CLI 2.0 сейчас.


> [!NOTE]
> Если вы используете предыдущую версию интерфейса командной строки (Azure CLI), вы можете продолжать использовать ее.
> При использовании обеих версий интерфейса командной строки помните, что `azure` является старой версией, т. е. Azure CLI, а `az` — новая версия интерфейса командной строки, Azure CLI 2.0. 