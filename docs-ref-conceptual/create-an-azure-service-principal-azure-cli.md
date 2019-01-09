---
title: Использование субъектов-служб Azure с помощью Azure CLI
description: Сведения о том, как использовать субъект-службу Azure с помощью Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6cce8fb47dd2b57180487441055333343fff8330
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805879"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="da3d1-103">Создание субъекта-службы Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="da3d1-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="da3d1-104">Если вы хотите создать отдельную процедуру входа с ограничениями доступа, это можно сделать с помощью субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="da3d1-104">If you want to create a separate sign-in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="da3d1-105">Субъекты-службы — это отдельные удостоверения, которые можно связывать с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="da3d1-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="da3d1-106">Субъекты-службы используются при работе с приложениями и задачами, которые должны выполняться автоматически.</span><span class="sxs-lookup"><span data-stu-id="da3d1-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="da3d1-107">В этой статье описывается, как создать субъект-службу.</span><span class="sxs-lookup"><span data-stu-id="da3d1-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="da3d1-108">Создание субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="da3d1-108">Create the service principal</span></span>

<span data-ttu-id="da3d1-109">Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="da3d1-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="da3d1-110">Имя субъекта-службы не привязано к существующему приложению или имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="da3d1-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="da3d1-111">Можно создать субъект-службу, указав нужный способ аутентификации.</span><span class="sxs-lookup"><span data-stu-id="da3d1-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="da3d1-112">`--password` используется для аутентификации на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="da3d1-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="da3d1-113">Если аргумент, указывающий тип аутентификации, не указан, по умолчанию используется аргумент --password и пароль создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="da3d1-113">If an argument indicating the authentication type isn't included, --password is used by default, and one is created for you.</span></span> <span data-ttu-id="da3d1-114">Если вы хотите использовать аутентификацию на основе пароля, мы рекомендуем использовать приведенную ниже команду (пароль будет создан автоматически).</span><span class="sxs-lookup"><span data-stu-id="da3d1-114">If you want to use password-based authentication, we recommend using this command, so the password is created for you.</span></span>  

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName 
  ```
  <span data-ttu-id="da3d1-115">Если вы хотите выбрать пароль самостоятельно (не рекомендуется из соображений безопасности), используйте команду, приведенную ниже.</span><span class="sxs-lookup"><span data-stu-id="da3d1-115">If you want to choose the password, instead of it being created for you (which is not recommended, for security reasons), you can use this command.</span></span> <span data-ttu-id="da3d1-116">Создайте надежный пароль, учитывая [правила и ограничения для паролей в Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="da3d1-116">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="da3d1-117">При самостоятельном выборе пароля существует вероятность выбора ненадежного пароля или использования пароля, который уже используется.</span><span class="sxs-lookup"><span data-stu-id="da3d1-117">The option to choose password leaves the chance of a weak password being chosen or password being re-used.</span></span> <span data-ttu-id="da3d1-118">В будущих версиях Azure CLI такая возможность будет исключена.</span><span class="sxs-lookup"><span data-stu-id="da3d1-118">This option is planned to be deprecated in a future version of Azure CLI.</span></span> 

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

* <span data-ttu-id="da3d1-119">`--cert` используется для аутентификации на основе существующего сертификата в формате PEM или DER. Также можно использовать `@{file}` для загрузки файла.</span><span class="sxs-lookup"><span data-stu-id="da3d1-119">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="da3d1-120">Вы можете добавить аргумент `--keyvault`, чтобы указать, что сертификат хранится в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="da3d1-120">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="da3d1-121">В этом случае значение `--cert` ссылается на имя сертификата в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="da3d1-121">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="da3d1-122">`--create-cert` создает _самозаверяющий_ сертификат для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="da3d1-122">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="da3d1-123">Если аргумент `--cert` не указан, создается произвольное имя сертификата.</span><span class="sxs-lookup"><span data-stu-id="da3d1-123">If the `--cert` argument isn't provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="da3d1-124">Вы можете добавить аргумент `--keyvault`, чтобы сохранить сертификат в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="da3d1-124">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="da3d1-125">При использовании `--keyvault` аргумент `--cert` также необходим.</span><span class="sxs-lookup"><span data-stu-id="da3d1-125">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="da3d1-126">Если аргумент, указывающий способ аутентификации, не будет включен, по умолчанию используется `--password`.</span><span class="sxs-lookup"><span data-stu-id="da3d1-126">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="da3d1-127">Выходные данные JSON команды `create-for-rbac` имеют следующий формат:</span><span class="sxs-lookup"><span data-stu-id="da3d1-127">The JSON output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="da3d1-128">Значения `appId`, `tenant` и `password` используются для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="da3d1-128">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="da3d1-129">`displayName` используется при поиске существующего субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="da3d1-129">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="da3d1-130">Если у учетной записи нет достаточных прав на создание субъекта-службы, вы увидите сообщение об ошибке, уведомляющее о "недостаточности привилегий для выполнения операции".</span><span class="sxs-lookup"><span data-stu-id="da3d1-130">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="da3d1-131">Чтобы получить возможность создавать субъекты-службы, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="da3d1-131">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="da3d1-132">Управление ролями субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="da3d1-132">Manage service principal roles</span></span>

<span data-ttu-id="da3d1-133">В Azure CLI доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="da3d1-133">The Azure CLI provides the following commands to manage role assignments.</span></span>

* <span data-ttu-id="da3d1-134">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list);</span><span class="sxs-lookup"><span data-stu-id="da3d1-134">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)</span></span>
* <span data-ttu-id="da3d1-135">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create);</span><span class="sxs-lookup"><span data-stu-id="da3d1-135">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)</span></span>
* <span data-ttu-id="da3d1-136">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete).</span><span class="sxs-lookup"><span data-stu-id="da3d1-136">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)</span></span>

<span data-ttu-id="da3d1-137">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="da3d1-137">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="da3d1-138">Эта роль имеет полные разрешения на чтение из учетной записи Azure и записи в нее, поэтому она не подходит для приложений.</span><span class="sxs-lookup"><span data-stu-id="da3d1-138">This role has full permissions to read and write to an Azure account, and is not appropriate for applications.</span></span> <span data-ttu-id="da3d1-139">Роль **читателя** имеет больше ограничений, предоставляя права доступа только на чтение.</span><span class="sxs-lookup"><span data-stu-id="da3d1-139">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="da3d1-140">Дополнительные сведения об управлении доступом на основе ролей см. в статье [Встроенные роли для ресурсов Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="da3d1-140">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="da3d1-141">В этом примере мы добавим роль **читателя** и удалим роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="da3d1-141">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="da3d1-142">Добавление роли _не_ изменяет назначенные ранее разрешения.</span><span class="sxs-lookup"><span data-stu-id="da3d1-142">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="da3d1-143">Ограничивая разрешения субъекта-службы, роль __участника__ всегда следует удалять.</span><span class="sxs-lookup"><span data-stu-id="da3d1-143">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="da3d1-144">Проверить изменения можно, отобразив назначенные роли.</span><span class="sxs-lookup"><span data-stu-id="da3d1-144">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="da3d1-145">Если ваша учетная запись не позволяет назначать роли, вы увидите сообщение об ошибке о том, что ваша учетная запись "не авторизована выполнять действие Microsoft.Authorization/roleAssignments/write для /subscriptions/{guid}". Чтобы получить возможность управлять ролями, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="da3d1-145">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="da3d1-146">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="da3d1-146">Sign in using the service principal</span></span>

<span data-ttu-id="da3d1-147">Вы можете протестировать разрешения и учетные данные для входа с помощью субъекта-службы, выполнив вход в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="da3d1-147">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="da3d1-148">Войдите с использованием нового субъекта-службы, указав значения `appId`, `tenant` и учетные данные.</span><span class="sxs-lookup"><span data-stu-id="da3d1-148">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="da3d1-149">Используйте тип аутентификации, с которым создан субъект-служба.</span><span class="sxs-lookup"><span data-stu-id="da3d1-149">Use the authentication type that the service principal was created with.</span></span>

<span data-ttu-id="da3d1-150">Чтобы войти с использованием пароля, предоставьте его как параметр аргумента.</span><span class="sxs-lookup"><span data-stu-id="da3d1-150">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="da3d1-151">Чтобы войти с использованием сертификата, он должен быть доступен локально как PEM- или DER-файл.</span><span class="sxs-lookup"><span data-stu-id="da3d1-151">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="da3d1-152">Сброс учетных данных</span><span class="sxs-lookup"><span data-stu-id="da3d1-152">Reset credentials</span></span>

<span data-ttu-id="da3d1-153">Если вы забыли учетные данные субъекта-службы, их можно сбросить с помощью команды [az ad sp reset-credentials](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="da3d1-153">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) command.</span></span> <span data-ttu-id="da3d1-154">Здесь применяются те же параметры и ограничения, как и при создании нового субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="da3d1-154">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID 
```
