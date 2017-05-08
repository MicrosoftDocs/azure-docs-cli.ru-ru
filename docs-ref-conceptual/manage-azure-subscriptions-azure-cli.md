---
title: "Manage Azure subscriptions with Azure CLI 2.0 (Управление подписками Azure с помощью Azure CLI 2.0)"
description: "Manage Azure subscriptions with Azure CLI 2.0 on Linux, Mac, or Windows (Управление подписками Azure с помощью Azure CLI 2.0 на платформах Windows, Mac или Linux)."
keywords: "Azure CLI 2.0, Linux, Mac, Windows, OS X, подписка"
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: c3538077e05d61f3c40880bb8b804226eb99dc85
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: ru-RU
---
# <a name="manage-multiple-azure-subscriptions"></a>Управление несколькими подписками Azure

Если вы только приступаете к работе с Azure, скорее всего, у вас есть только одна подписка.
Но если вы уже пользуетесь Azure какое-то время, возможно, вы уже успели создать несколько подписок.
Вы можете настроить Azure CLI 2.0 для выполнения команд, связанных с определенной подпиской.

1. Получите список всех подписок в своей учетной записи.

   ```azurecli
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. Определите подписку по умолчанию.
 
   ```azurecli
   az account set --subscription "My Demos"
   ```

Проверьте изменения, выполнив команду `az account list --output table` еще раз.

Когда вы определите подписку по умолчанию, все последующие выполняемые команды Azure CLI будут связаны с ней.