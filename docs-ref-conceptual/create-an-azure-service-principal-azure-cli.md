---
title: Использование субъекта-службы Azure с помощью Azure CLI 2.0
description: Использование субъекта-службы Azure с помощью Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: role-based-access-control
ms.openlocfilehash: 3f20892e846bd07f8e97ccf788d05c4305fe3301
ms.sourcegitcommit: 83826ca154c9f32c6091c63ce4b3e480694ba8d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/09/2018
ms.locfileid: "43144890"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="32aa9-103">Создание субъекта-службы Azure с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="32aa9-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="32aa9-104">Если нужно создать отдельную процедуру входа с ограничениями доступа, это можно сделать с помощью субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="32aa9-104">If you want to create a separate sign in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="32aa9-105">Субъекты-службы — это отдельные удостоверения, которые можно связывать с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="32aa9-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="32aa9-106">Субъекты-службы используются при работе с приложениями и задачами, которые должны выполняться автоматически.</span><span class="sxs-lookup"><span data-stu-id="32aa9-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="32aa9-107">В этой статье описывается, как создать субъект-службу.</span><span class="sxs-lookup"><span data-stu-id="32aa9-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="32aa9-108">Создание субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="32aa9-108">Create the service principal</span></span>

<span data-ttu-id="32aa9-109">Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="32aa9-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="32aa9-110">Имя субъекта-службы не привязано к существующему приложению или имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="32aa9-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="32aa9-111">Можно создать субъект-службу, указав нужный способ аутентификации.</span><span class="sxs-lookup"><span data-stu-id="32aa9-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="32aa9-112">`--password` используется для аутентификации на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="32aa9-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="32aa9-113">Создайте надежный пароль, учитывая [правила и ограничения для паролей в Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="32aa9-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="32aa9-114">Если вы не укажете пароль, он будет создан автоматически.</span><span class="sxs-lookup"><span data-stu-id="32aa9-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="32aa9-115">`--cert` используется для аутентификации на основе существующего сертификата в формате PEM или DER. Также можно использовать `@{file}` для загрузки файла.</span><span class="sxs-lookup"><span data-stu-id="32aa9-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="32aa9-116">Вы можете добавить аргумент `--keyvault`, чтобы указать, что сертификат хранится в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="32aa9-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="32aa9-117">В этом случае значение `--cert` ссылается на имя сертификата в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="32aa9-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="32aa9-118">`--create-cert` создает _самозаверяющий_ сертификат для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="32aa9-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="32aa9-119">Если аргумент `--cert` не указан, создается произвольное имя сертификата.</span><span class="sxs-lookup"><span data-stu-id="32aa9-119">If the `--cert` argument is not provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="32aa9-120">Вы можете добавить аргумент `--keyvault`, чтобы сохранить сертификат в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="32aa9-120">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="32aa9-121">При использовании `--keyvault` аргумент `--cert` также необходим.</span><span class="sxs-lookup"><span data-stu-id="32aa9-121">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="32aa9-122">Если аргумент, указывающий способ аутентификации, не будет включен, по умолчанию используется `--password`.</span><span class="sxs-lookup"><span data-stu-id="32aa9-122">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="32aa9-123">Выходные данные команды `create-for-rbac` имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="32aa9-123">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="32aa9-124">Значения `appId`, `tenant` и `password` используются для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="32aa9-124">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="32aa9-125">`displayName` используется при поиске существующего субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="32aa9-125">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="32aa9-126">Если у учетной записи нет достаточных прав на создание субъекта-службы, вы увидите сообщение об ошибке, уведомляющее о "недостаточности привилегий для выполнения операции".</span><span class="sxs-lookup"><span data-stu-id="32aa9-126">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="32aa9-127">Чтобы получить возможность создавать субъекты-службы, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32aa9-127">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="32aa9-128">Управление ролями субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="32aa9-128">Manage service principal roles</span></span>

<span data-ttu-id="32aa9-129">В Azure CLI 2.0 доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="32aa9-129">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* <span data-ttu-id="32aa9-130">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list);</span><span class="sxs-lookup"><span data-stu-id="32aa9-130">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)</span></span>
* <span data-ttu-id="32aa9-131">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create);</span><span class="sxs-lookup"><span data-stu-id="32aa9-131">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)</span></span>
* <span data-ttu-id="32aa9-132">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete).</span><span class="sxs-lookup"><span data-stu-id="32aa9-132">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)</span></span>

<span data-ttu-id="32aa9-133">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="32aa9-133">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="32aa9-134">Эта роль предоставляет полные права доступа на чтение и запись для учетной записи Azure. Как правило, она не используется для приложений.</span><span class="sxs-lookup"><span data-stu-id="32aa9-134">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="32aa9-135">Роль **читателя** имеет больше ограничений, предоставляя права доступа только на чтение.</span><span class="sxs-lookup"><span data-stu-id="32aa9-135">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="32aa9-136">См. дополнительные сведения о [встроенных возможностях управления доступом на основе ролей](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="32aa9-136">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="32aa9-137">В этом примере мы добавим роль **читателя** и удалим роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="32aa9-137">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="32aa9-138">Добавление роли _не_ изменяет назначенные ранее разрешения.</span><span class="sxs-lookup"><span data-stu-id="32aa9-138">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="32aa9-139">Ограничивая разрешения субъекта-службы, роль __участника__ всегда следует удалять.</span><span class="sxs-lookup"><span data-stu-id="32aa9-139">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="32aa9-140">Проверить изменения можно, отобразив назначенные роли.</span><span class="sxs-lookup"><span data-stu-id="32aa9-140">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="32aa9-141">Если ваша учетная запись не позволяет назначать роли, вы увидите сообщение об ошибке о том, что ваша учетная запись "не авторизована выполнять действие Microsoft.Authorization/roleAssignments/write для /subscriptions/{guid}". Чтобы получить возможность управлять ролями, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32aa9-141">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="32aa9-142">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="32aa9-142">Sign in using the service principal</span></span>

<span data-ttu-id="32aa9-143">Вы можете протестировать разрешения и учетные данные для входа с помощью субъекта-службы, выполнив вход в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="32aa9-143">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="32aa9-144">Войдите с использованием нового субъекта-службы, указав значения `appId`, `tenant` и учетные данные.</span><span class="sxs-lookup"><span data-stu-id="32aa9-144">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="32aa9-145">Предоставляемые сведения для аутентификации будут зависеть от того, на основе чего был создан субъект-служба — пароля или сертификата.</span><span class="sxs-lookup"><span data-stu-id="32aa9-145">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="32aa9-146">Чтобы войти с использованием пароля, предоставьте его как параметр аргумента.</span><span class="sxs-lookup"><span data-stu-id="32aa9-146">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="32aa9-147">Чтобы войти с использованием сертификата, он должен быть доступен локально как PEM- или DER-файл.</span><span class="sxs-lookup"><span data-stu-id="32aa9-147">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="32aa9-148">Сброс учетных данных</span><span class="sxs-lookup"><span data-stu-id="32aa9-148">Reset credentials</span></span>

<span data-ttu-id="32aa9-149">Если вы забыли учетные данные субъекта-службы, вы можете сбросить их с помощью команды [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="32aa9-149">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) command.</span></span> <span data-ttu-id="32aa9-150">Здесь применяются те же параметры и ограничения, как и при создании нового субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="32aa9-150">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID --password NEW_PASSWORD
```
