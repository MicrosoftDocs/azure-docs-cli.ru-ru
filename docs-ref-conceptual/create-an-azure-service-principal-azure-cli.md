---
title: Использование субъекта-службы Azure с помощью Azure CLI 2.0
description: Использование субъекта-службы Azure с помощью Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: role-based-access-control
ms.openlocfilehash: 5f98fd8d3897b11a9b37eefa6295b8b25b2b1c95
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388445"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Создание субъекта-службы Azure с помощью Azure CLI 2.0

Если вы хотите создать отдельную процедуру входа с ограничениями доступа, это можно сделать с помощью субъекта-службы. Субъекты-службы — это отдельные удостоверения, которые можно связывать с учетной записью. Субъекты-службы используются при работе с приложениями и задачами, которые должны выполняться автоматически. В этой статье описывается, как создать субъект-службу.

## <a name="create-the-service-principal"></a>Создание субъекта-службы

Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac). Имя субъекта-службы не привязано к существующему приложению или имени пользователя. Можно создать субъект-службу, указав нужный способ аутентификации.

* `--password` используется для аутентификации на основе пароля. Создайте надежный пароль, учитывая [правила и ограничения для паролей в Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). Если вы не укажете пароль, он будет создан автоматически.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* `--cert` используется для аутентификации на основе существующего сертификата в формате PEM или DER. Также можно использовать `@{file}` для загрузки файла.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  Вы можете добавить аргумент `--keyvault`, чтобы указать, что сертификат хранится в Azure Key Vault. В этом случае значение `--cert` ссылается на имя сертификата в Key Vault.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* `--create-cert` создает _самозаверяющий_ сертификат для аутентификации. Если аргумент `--cert` не указан, создается произвольное имя сертификата.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  Вы можете добавить аргумент `--keyvault`, чтобы сохранить сертификат в Azure Key Vault. При использовании `--keyvault` аргумент `--cert` также необходим.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

Если аргумент, указывающий способ аутентификации, не будет включен, по умолчанию используется `--password`.

Выходные данные команды `create-for-rbac` имеют следующий формат:

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Значения `appId`, `tenant` и `password` используются для аутентификации. `displayName` используется при поиске существующего субъекта-службы.

> [!NOTE]
> Если у учетной записи нет достаточных прав на создание субъекта-службы, вы увидите сообщение об ошибке, уведомляющее о "недостаточности привилегий для выполнения операции". Чтобы получить возможность создавать субъекты-службы, обратитесь к администратору Azure Active Directory.

## <a name="manage-service-principal-roles"></a>Управление ролями субъекта-службы

В Azure CLI 2.0 доступны следующие команды для управления назначением ролей:

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list);
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create);
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete).

По умолчанию субъекту-службе назначена роль **участника**. Эта роль имеет полные разрешения на чтение из учетной записи Azure и записи в нее, поэтому она не подходит для приложений. Роль **читателя** имеет больше ограничений, предоставляя права доступа только на чтение.  См. дополнительные сведения о [встроенных возможностях управления доступом на основе ролей](/azure/active-directory/role-based-access-built-in-roles).

В этом примере мы добавим роль **читателя** и удалим роль **участника**.

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

Добавление роли _не_ изменяет назначенные ранее разрешения. Ограничивая разрешения субъекта-службы, роль __участника__ всегда следует удалять.

Проверить изменения можно, отобразив назначенные роли.

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> Если ваша учетная запись не позволяет назначать роли, вы увидите сообщение об ошибке о том, что ваша учетная запись "не авторизована выполнять действие Microsoft.Authorization/roleAssignments/write для /subscriptions/{guid}". Чтобы получить возможность управлять ролями, обратитесь к администратору Azure Active Directory.

## <a name="sign-in-using-the-service-principal"></a>Вход с помощью субъекта-службы

Вы можете протестировать разрешения и учетные данные для входа с помощью субъекта-службы, выполнив вход в Azure CLI. Войдите с использованием нового субъекта-службы, указав значения `appId`, `tenant` и учетные данные. Используйте тип аутентификации, с которым создан субъект-служба.

Чтобы войти с использованием пароля, предоставьте его как параметр аргумента.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Чтобы войти с использованием сертификата, он должен быть доступен локально как PEM- или DER-файл.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>Сброс учетных данных

Если вы забыли учетные данные субъекта-службы, их можно сбросить с помощью команды [az ad sp reset-credentials](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). Здесь применяются те же параметры и ограничения, как и при создании нового субъекта-службы.

```azurecli-interactive
az ad sp credential reset --name APP_ID --password NEW_PASSWORD
```
