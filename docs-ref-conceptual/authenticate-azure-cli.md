---
title: Вход с помощью Azure CLI 2.0
description: Интерактивный вход с помощью Azure CLI 2.0 или вход с использованием локальных учетных данных
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/13/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: db676c7d81d1ea5628ebb52f3bcead763c5527f9
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="log-in-with-azure-cli-20"></a>Вход с помощью Azure CLI 2.0

Используя Azure CLI, можно входить и выполнять проверку подлинности несколькими способами. Проще всего войти в интерактивном режиме из браузера, Azure Cloud Shell или команды `az login`.
Рекомендуется использовать субъекты-службы, которые представляют учетные записи с ограниченными разрешениями. Предоставляя только нужные разрешения, необходимые для субъекта-службы, вы можете обеспечить безопасность скриптов службы автоматизации.

Учетные данные являются конфиденциальными и не хранятся локально. Маркер проверки подлинности создается и сохраняется в Azure. После входа в систему маркер для входа остается действительным в течение 14 дней без использования. На этом этапе необходимо пройти повторную аутентификацию.

Когда вы войдете, команды интерфейса командной строки будут выполняться в вашей подписке по умолчанию. Если у вас несколько подписок, вы можете [изменить подписку по умолчанию](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Интерактивный вход

Выполните интерактивный вход из веб-браузера.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Команда

Укажите свои учетные данные пользователя Azure в командной строке.

> [!Note]
> Этот способ не работает с учетными записями Майкрософт или с учетными записями, которые используют двухфакторную проверку подлинности.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Если вы не хотите, чтобы ваш пароль отображался в консоли, и используете `az login` в интерактивном режиме, используйте команду `read -s` в `bash`.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> В PowerShell же для этого нужно использовать командлет `Read-Host -AsSecureString` и безопасное преобразование строк.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="log-in-with-a-specific-tenant"></a>Вход в определенный клиент

При работе с несколькими клиентами вы можете войти в определенный клиент с помощью аргумента `--tenant`. Значением этого аргумента может быть домен `.onmicrosoft.com` или идентификатор объекта Azure для клиента. Войти можно либо в интерактивном режиме, либо указав свои учетные данные с помощью аргументов `--user` и `--password`. 

```
az login --tenant <tenant>
```

## <a name="log-in-with-a-service-principal"></a>Вход с использованием субъекта-службы

Субъекты-службы — это учетные записи, не связаны с определенным пользователем. Они предоставляют разрешения, назначаемые с помощью предопределенных ролей. Аутентификация с помощью субъекта-службы лучше всего подходит для создания безопасных скриптов и программ, позволяя применять как ограничения разрешений, так и хранимые локально сведения о статических учетных данных. Дополнительные сведения о субъектах-службах см. в руководстве по [созданию субъекта-службы Azure с помощью Azure CLI ](create-an-azure-service-principal-azure-cli.md).

Чтобы войти с помощью субъекта-службы, укажите имя пользователя, пароль или сертификат PEM-файла, а также клиент, связанный с субъектом-службой:

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

Значение клиента — это клиент Azure Active Directory, связанный с субъектом-службой. Это может быть домен `.onmicrosoft.com` или идентификатор объекта Azure для клиента.
Узнать идентификатор объекта клиента для текущего сеанса входа можно с помощью следующей команды:

```azurecli
az account show --query 'tenantId' -o tsv
```

> [!IMPORTANT]
> Если вы не хотите, чтобы ваш пароль отображался в консоли, и используете `az login` в интерактивном режиме, используйте команду `read -s` в `bash`.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> В PowerShell же для этого нужно использовать командлет `Read-Host -AsSecureString` и безопасное преобразование строк.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```
