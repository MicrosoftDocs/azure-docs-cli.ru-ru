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
ms.openlocfilehash: cd9a41b66d18410afa091ede50ca24e7d4b5e9ed
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439964"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="5f5e8-103">Создание субъекта-службы Azure с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="5f5e8-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="5f5e8-104">Если вы хотите создать возможность отдельного входа с ограничениями доступа, это можно сделать с помощью субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="5f5e8-105">Субъекты-службы — это отдельные удостоверения, которые можно связывать с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="5f5e8-106">Субъекты-службы используются при работе с приложениями и задачами, которые должны выполняться автоматически.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="5f5e8-107">В этой статье описывается, как создать субъект-службу.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="5f5e8-108">Создание субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="5f5e8-108">Create the service principal</span></span>

<span data-ttu-id="5f5e8-109">Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="5f5e8-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="5f5e8-110">Имя субъекта-службы не привязано к существующему приложению или имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="5f5e8-111">Можно создать субъект-службу, указав нужный способ аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="5f5e8-112">`--password` используется для аутентификации на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="5f5e8-113">Создайте надежный пароль, учитывая [правила и ограничения для паролей в Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="5f5e8-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="5f5e8-114">Если вы не укажете пароль, он будет создан автоматически.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="5f5e8-115">`--cert` используется для аутентификации на основе существующего сертификата в формате PEM или DER. Также можно использовать `@{file}` для загрузки файла.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="5f5e8-116">Вы можете добавить аргумент `--keyvault`, чтобы указать, что сертификат хранится в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="5f5e8-117">В этом случае значение `--cert` ссылается на имя сертификата в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="5f5e8-118">`--create-cert` создает _самозаверяющий_ сертификат для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="5f5e8-119">Если аргумент `--cert` не указан, создается произвольное имя сертификата.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-119">If the `--cert` argument is not provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="5f5e8-120">Вы можете добавить аргумент `--keyvault`, чтобы сохранить сертификат в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-120">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="5f5e8-121">При использовании `--keyvault` аргумент `--cert` также необходим.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-121">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="5f5e8-122">Если аргумент, указывающий способ аутентификации, не будет включен, по умолчанию используется `--password`.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-122">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="5f5e8-123">Выходные данные команды `create-for-rbac` имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="5f5e8-123">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="5f5e8-124">Значения `appId`, `tenant` и `password` используются для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-124">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="5f5e8-125">`displayName` используется при поиске существующего субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-125">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="5f5e8-126">Если у учетной записи нет достаточных прав на создание субъекта-службы, вы увидите сообщение об ошибке, уведомляющее о "недостаточности привилегий для выполнения операции".</span><span class="sxs-lookup"><span data-stu-id="5f5e8-126">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="5f5e8-127">Чтобы получить возможность создавать субъекты-службы, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-127">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="5f5e8-128">Управление ролями субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="5f5e8-128">Manage service principal roles</span></span> 

<span data-ttu-id="5f5e8-129">В Azure CLI 2.0 доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="5f5e8-129">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* <span data-ttu-id="5f5e8-130">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list);</span><span class="sxs-lookup"><span data-stu-id="5f5e8-130">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)</span></span>
* <span data-ttu-id="5f5e8-131">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create);</span><span class="sxs-lookup"><span data-stu-id="5f5e8-131">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)</span></span>
* <span data-ttu-id="5f5e8-132">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete).</span><span class="sxs-lookup"><span data-stu-id="5f5e8-132">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)</span></span>

<span data-ttu-id="5f5e8-133">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-133">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="5f5e8-134">Эта роль предоставляет полные права доступа на чтение и запись для учетной записи Azure. Как правило, она не используется для приложений.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-134">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="5f5e8-135">Роль **читателя** имеет больше ограничений, предоставляя права доступа только на чтение.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-135">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="5f5e8-136">См. дополнительные сведения о [встроенных возможностях управления доступом на основе ролей](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="5f5e8-136">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="5f5e8-137">В этом примере мы добавим роль **читателя** и удалим роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-137">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="5f5e8-138">Добавление роли _не_ изменяет назначенные ранее разрешения.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-138">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="5f5e8-139">Ограничивая разрешения субъекта-службы, роль __участника__ всегда следует удалять.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-139">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="5f5e8-140">Проверить изменения можно, отобразив назначенные роли.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-140">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="5f5e8-141">Если ваша учетная запись не позволяет назначать роли, вы увидите сообщение об ошибке о том, что ваша учетная запись "не авторизована выполнять действие Microsoft.Authorization/roleAssignments/write для /subscriptions/{guid}". Чтобы получить возможность управлять ролями, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-141">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="5f5e8-142">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="5f5e8-142">Sign in using the service principal</span></span>

<span data-ttu-id="5f5e8-143">Вы можете протестировать разрешения и возможность входа с помощью субъекта-службы, выполнив вход в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-143">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="5f5e8-144">Войдите с использованием нового субъекта-службы с помощью значений `appId`, `tenant` и учетных данных.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-144">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="5f5e8-145">Предоставляемые сведения для аутентификации будут зависеть от того, на основе чего был создан субъект-служба — пароля или сертификата.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-145">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="5f5e8-146">Чтобы войти с использованием пароля, предоставьте его как параметр аргумента.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-146">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="5f5e8-147">Чтобы войти с использованием сертификата, он должен быть доступен локально как PEM или DER.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-147">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="5f5e8-148">Сброс учетных данных</span><span class="sxs-lookup"><span data-stu-id="5f5e8-148">Reset credentials</span></span>

<span data-ttu-id="5f5e8-149">Если вы забыли учетные данные субъекта-службы, вы можете сбросить их с помощью команды [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="5f5e8-149">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials) command.</span></span> <span data-ttu-id="5f5e8-150">Здесь применяются те же параметры и ограничения, как и при создании нового субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="5f5e8-150">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
