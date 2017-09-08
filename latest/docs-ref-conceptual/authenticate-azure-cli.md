---
title: "Вход с помощью Azure CLI 2.0"
description: "Вход с помощью Azure CLI 2.0 на виртуальные машины Mac, Windows или Linux."
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
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2017
---
# <a name="log-in-with-azure-cli-20"></a>Вход с помощью Azure CLI 2.0

Используя Azure CLI, можно входить и выполнять проверку подлинности несколькими способами. Проще всего начать со входа в интерактивном режиме из браузера или командной строки. Рекомендуется использовать субъекты-службы. Они позволяют создавать неинтерактивные учетные записи, которые можно использовать для управления ресурсами. Предоставляя только нужные разрешения, необходимые для субъекта-службы, вы можете обеспечить безопасность скриптов службы автоматизации.

Команды, которые вы выполняете с помощью интерфейса командной строки, выполняются в вашей подписке по умолчанию.  Если у вас несколько подписок, может потребоваться [подтвердить подписку по умолчанию](manage-azure-subscriptions-azure-cli.md) и изменить ее соответствующим образом.

## <a name="interactive-log-in"></a>Интерактивный вход

Выполните интерактивный вход из веб-браузера.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Команда

Укажите свои учетные данные в командной строке.

> [!Note]
> Этот способ не работает с учетными записями Майкрософт или с учетными записями, которые используют двухфакторную проверку подлинности.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>Вход с использованием субъекта-службы

Субъекты-службы похожи на учетные записи пользователей, к которым можно применять правила, используя Azure Active Directory.
Проверка подлинности с помощью субъекта-службы — это самый безопасный способ использования ресурсов Azure из сценариев или приложений, которые работают с ресурсами.
Вы можете определить роли пользователей с помощью набора команд `az role`.
Дополнительные сведения и примеры ролей субъекта-службы см. в [справочных статьях о ролях az](https://docs.microsoft.com/cli/azure/role.md).

1. Если у вас еще нет субъекта-службы, [создайте](create-an-azure-service-principal-azure-cli.md) его.

1. Войдите с помощью субъекта-службы.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   Чтобы получить свой клиент, войдите в интерактивном режиме, а затем получите идентификатор из подписки.

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```