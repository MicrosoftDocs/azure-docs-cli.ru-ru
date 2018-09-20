---
title: Вход с помощью Azure CLI 2.0
description: Интерактивный вход с помощью Azure CLI 2.0 или вход с использованием локальных учетных данных
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: ef77f407284752ad4f4a1585f8a4036b32b3eb1b
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388326"
---
# <a name="sign-in-with-azure-cli-20"></a>Вход с помощью Azure CLI 2.0

Azure CLI поддерживает несколько типов аутентификации. Проще всего приступить к работе можно с помощью оболочки [Azure Cloud Shell](/azure/cloud-shell/overview), которая автоматически выполняет вход в вашу учетную запись. На локальном компьютере вы можете выполнить вход в интерактивном режиме с помощью браузера, выполнив команду `az login`. При написании скриптов рекомендуется использовать субъекты-службы. Предоставляя именно те разрешения, которые нужны субъекту-службе, можно обеспечить безопасность скрипта автоматизации.

CLI не хранит ваши сведения о входе. Маркер проверки подлинности создается и сохраняется в Azure. После входа в систему маркер аутентификации остается действительным в течение 90 дней без использования.

После входа команды CLI будут выполняться в вашей подписке по умолчанию. Если у вас есть несколько подписок, можно [изменить подписку по умолчанию](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Интерактивный вход

Метод проверки подлинности, используемый в Azure CLI по умолчанию, — вход с помощью веб-браузера и маркера доступа.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Вход с учетными данными с помощью командной строки

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

## <a name="sign-in-with-a-specific-tenant"></a>Вход в определенный клиент

С помощью аргумента `--tenant` можно выбрать клиент, от имени которого выполняется вход. Значением этого аргумента может быть домен `.onmicrosoft.com` или идентификатор объекта Azure для клиента. Аргумент `--tenant` поддерживает оба метода входа — интерактивный и с помощью командной строки.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Вход с использованием субъекта-службы

Субъекты-службы — это учетные записи, не связаны с определенным пользователем. Они предоставляют разрешения, назначаемые с помощью предопределенных ролей. Аутентификация с помощью субъекта-службы лучше всего подходит для создания безопасных скриптов и программ, позволяя применять как ограничения разрешений, так и хранимые локально сведения о статических учетных данных. Дополнительные сведения о субъектах-службах см. в руководстве по [созданию субъекта-службы Azure с помощью Azure CLI ](create-an-azure-service-principal-azure-cli.md).

Для входа с помощью субъекта-службы необходимы следующие сведения:

* URL-адрес или имя, связанное с субъектом-службой;
* пароль субъекта-службы или сертификат X509 в формате PEM, используемый для создания субъекта-службы;
* идентификатор клиента, связанного с субъектом-службой, в виде домена `.onmicrosoft.com` или идентификатора объекта Azure.

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
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
