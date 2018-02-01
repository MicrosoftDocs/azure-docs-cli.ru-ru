---
title: "Создание субъекта-службы Azure с помощью Azure CLI 2.0"
description: "Узнайте, как создать субъект-службу для приложения или службы с помощью Azure CLI 2.0."
keywords: "Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 10/12/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: e473b7289f3b72dc23a1f747e15cea1b88aa89e9
ms.sourcegitcommit: dd5b2c7b0b56608ef9ea8730c7dc76e6c532d5ea
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2018
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="016fb-104">Создание субъекта-службы Azure с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="016fb-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="016fb-105">Если вы планируете управлять приложением или службой с помощью Azure CLI 2.0, вы должны запустить это приложение или службу с помощью субъекта-службы Azure Active Directory (AAD), а не своих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="016fb-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="016fb-106">В этой статье объясняется, как создать субъект безопасности с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="016fb-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="016fb-107">Можно также создать субъект-службу на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="016fb-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="016fb-108">Дополнительные сведения см. в статье [Создание приложения Azure Active Directory и субъекта-службы с доступом к ресурсам с помощью портала](/azure/azure-resource-manager/resource-group-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="016fb-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="016fb-109">Что такое субъект-служба?</span><span class="sxs-lookup"><span data-stu-id="016fb-109">What is a 'service principal'?</span></span>

<span data-ttu-id="016fb-110">Субъект-служба Azure — это идентификатор безопасности, который используют созданные пользователем приложения, службы и средства автоматизации для доступа к определенным ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="016fb-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="016fb-111">Это что-то вроде удостоверения пользователя (имя для входа и пароль или сертификат) с определенной ролью и строго контролируемыми разрешениями на доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="016fb-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="016fb-112">Субъект-служба должен выполнять только конкретные задачи, в отличие от удостоверений пользователей.</span><span class="sxs-lookup"><span data-stu-id="016fb-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="016fb-113">Это решение повышает безопасность, если вы предоставите ему минимальный уровень разрешений для выполнения задач управления.</span><span class="sxs-lookup"><span data-stu-id="016fb-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span>

<span data-ttu-id="016fb-114">Azure CLI 2.0 поддерживает создание учетных данных для аутентификации на основе пароля и учетных данных сертификата.</span><span class="sxs-lookup"><span data-stu-id="016fb-114">Azure CLI 2.0 supports the creation of password-based authentication credentials and certificate credentials.</span></span> <span data-ttu-id="016fb-115">В этой статье рассматриваются оба типа учетных данных.</span><span class="sxs-lookup"><span data-stu-id="016fb-115">In this topic, we cover both types of credentials.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="016fb-116">Проверка уровня разрешений</span><span class="sxs-lookup"><span data-stu-id="016fb-116">Verify your own permission level</span></span>

<span data-ttu-id="016fb-117">Во-первых, у вас должен быть достаточный уровень разрешений в Azure Active Directory и подписке Azure.</span><span class="sxs-lookup"><span data-stu-id="016fb-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="016fb-118">В частности, у вас должно быть право создавать приложения в Active Directory и назначать роли субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="016fb-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span>

<span data-ttu-id="016fb-119">Проверить, есть ли у вас соответствующие разрешения, проще всего на портале.</span><span class="sxs-lookup"><span data-stu-id="016fb-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="016fb-120">Ознакомьтесь с [проверкой наличия необходимых разрешений на портале](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="016fb-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="016fb-121">Создание субъекта-службы для приложения</span><span class="sxs-lookup"><span data-stu-id="016fb-121">Create a service principal for your application</span></span>

<span data-ttu-id="016fb-122">Необходимо иметь один из следующих параметров для определения приложения, которое нужно создать для субъекта-службы:</span><span class="sxs-lookup"><span data-stu-id="016fb-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="016fb-123">уникальное имя или URI развернутого приложения (например, MyDemoWebApp в следующих примерах);</span><span class="sxs-lookup"><span data-stu-id="016fb-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="016fb-124">идентификатор приложения — глобальный уникальный идентификатор, связанный с развернутым приложением, службой или объектом.</span><span class="sxs-lookup"><span data-stu-id="016fb-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="016fb-125">Эти значения идентифицируют ваше приложение при создании субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="016fb-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="016fb-126">Получение сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="016fb-126">Get information about your application</span></span>

<span data-ttu-id="016fb-127">Получить сведения для идентификации приложения можно с помощью команды `az ad app list`.</span><span class="sxs-lookup"><span data-stu-id="016fb-127">Get identity information about your application with the `az ad app list`.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

<span data-ttu-id="016fb-128">Параметр `--display-name` фильтрует возвращаемый список приложений, чтобы показать те, которые содержат `displayName`, начиная с MyDemoWebApp.</span><span class="sxs-lookup"><span data-stu-id="016fb-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-a-service-principal-with-a-password"></a><span data-ttu-id="016fb-129">Создание субъекта-службы с паролем</span><span class="sxs-lookup"><span data-stu-id="016fb-129">Create a service principal with a password</span></span>

<span data-ttu-id="016fb-130">Чтобы создать субъект-службу с паролем, используйте команду [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) и параметр `--password`.</span><span class="sxs-lookup"><span data-stu-id="016fb-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--password` parameter to create the service principal with a password.</span></span> <span data-ttu-id="016fb-131">Если роль или область не указаны, по умолчанию используется роль **участника** для текущей подписки.</span><span class="sxs-lookup"><span data-stu-id="016fb-131">When you do not provide a role or scope, it defaults to the **Contributor** role for the current subscription.</span></span> <span data-ttu-id="016fb-132">При создании субъекта-службы без использования параметра `--password` или `--cert` используется проверка подлинности на основе пароля, а сам пароль создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="016fb-132">If you create a service principal without using either the `--password` or `--cert` parameter, password authentication is used and a password is generated for you.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name {appName} --password "{strong password}"
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING]
 > <span data-ttu-id="016fb-133">Не используйте ненадежный пароль.</span><span class="sxs-lookup"><span data-stu-id="016fb-133">Don't create an insecure password.</span></span>  <span data-ttu-id="016fb-134">Следуйте руководству по [правилам и ограничениям для паролей Azure AD](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="016fb-134">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="create-a-service-principal-with-a-self-signed-certificate"></a><span data-ttu-id="016fb-135">Создание субъекта-службы с самозаверяющим сертификатом</span><span class="sxs-lookup"><span data-stu-id="016fb-135">Create a service principal with a self-signed certificate</span></span>

<span data-ttu-id="016fb-136">Чтобы создать самозаверяющий сертификат, используйте команду [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) и параметр `--create-cert`.</span><span class="sxs-lookup"><span data-stu-id="016fb-136">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) and the `--create-cert` parameter to create a self-signed certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name {appName} --create-cert
```

```json
{
  "appId": "c495db57-82e0-4e2e-9369-069dff176858",
  "displayName": "azure-cli-2017-10-12-22-15-38",
  "fileWithCertAndPrivateKey": "<path>/<file-name>.pem",
  "name": "http://MyDemoWebApp",
  "password": null,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="016fb-137">Скопируйте значение ответа `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="016fb-137">Copy the value of the `fileWithCertAndPrivateKey` response.</span></span> <span data-ttu-id="016fb-138">Это файл сертификата, который будет использоваться для аутентификации.</span><span class="sxs-lookup"><span data-stu-id="016fb-138">This is the certificate file which will be used for authentication.</span></span>

<span data-ttu-id="016fb-139">Дополнительные параметры для сертификатов см. в разделе [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="016fb-139">For more options when using certificates, see [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="016fb-140">Получение сведений о субъекте-службе</span><span class="sxs-lookup"><span data-stu-id="016fb-140">Get information about the service principal</span></span>

```azurecli-interactive
az ad sp show --id {appID}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="016fb-141">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="016fb-141">Sign in using the service principal</span></span>

<span data-ttu-id="016fb-142">Теперь вы можете войти от имени нового субъекта-службы для приложения с использованием *appId* из `az ad sp show`, а также *пароля* либо пути к созданному сертификату.</span><span class="sxs-lookup"><span data-stu-id="016fb-142">You can now log in as the new service principal for your app using the *appId* from `az ad sp show`, and either the *password* or the path to the created certificate.</span></span>  <span data-ttu-id="016fb-143">Укажите значение параметра *tenant*, полученное в результате выполнения команды `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="016fb-143">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u {appID} --password {password-or-path-to-cert} --tenant {tenant}
```

<span data-ttu-id="016fb-144">После успешного входа отобразится следующее:</span><span class="sxs-lookup"><span data-stu-id="016fb-144">You will see this output after a successful sign-on:</span></span>

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

<span data-ttu-id="016fb-145">Используйте значения `id`, `password` и `tenant` в качестве учетных данных для запуска приложения.</span><span class="sxs-lookup"><span data-stu-id="016fb-145">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span>

## <a name="managing-roles"></a><span data-ttu-id="016fb-146">Управление ролями</span><span class="sxs-lookup"><span data-stu-id="016fb-146">Managing roles</span></span>

> [!NOTE]
> <span data-ttu-id="016fb-147">Управление доступом на основе ролей в Azure (RBAC) — это модель для определения ролей пользователя и субъектов-служб и управления этими ролями.</span><span class="sxs-lookup"><span data-stu-id="016fb-147">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="016fb-148">Ролям назначаются связанные наборы разрешений, которые определяют ресурсы, доступные субъекту для чтения, доступа, записи или управления.</span><span class="sxs-lookup"><span data-stu-id="016fb-148">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="016fb-149">Дополнительные сведения о RBAC и ролях см. в статье [Встроенные роли для управления доступом на основе ролей в Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="016fb-149">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="016fb-150">В Azure CLI 2.0 доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="016fb-150">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* <span data-ttu-id="016fb-151">[az role assignment list](/cli/azure/role/assignment#list);</span><span class="sxs-lookup"><span data-stu-id="016fb-151">[az role assignment list](/cli/azure/role/assignment#list)</span></span>
* <span data-ttu-id="016fb-152">[az role assignment create](/cli/azure/role/assignment#create);</span><span class="sxs-lookup"><span data-stu-id="016fb-152">[az role assignment create](/cli/azure/role/assignment#create)</span></span>
* <span data-ttu-id="016fb-153">[az role assignment delete](/cli/azure/role/assignment#delete).</span><span class="sxs-lookup"><span data-stu-id="016fb-153">[az role assignment delete](/cli/azure/role/assignment#delete)</span></span>

<span data-ttu-id="016fb-154">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="016fb-154">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="016fb-155">Возможно, это не лучший выбор для взаимодействия приложения со службами Azure, учитывая широкие разрешения у этой роли.</span><span class="sxs-lookup"><span data-stu-id="016fb-155">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="016fb-156">Роль **читателя** имеет больше ограничений и отлично подходит для доступа с правами только для чтения.</span><span class="sxs-lookup"><span data-stu-id="016fb-156">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="016fb-157">Вы можете просмотреть сведения о разрешениях каждой роли или создать пользовательские разрешения на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="016fb-157">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="016fb-158">В этом примере мы добавим роль **читателя** к предыдущему примеру и удалим роль **участника**:</span><span class="sxs-lookup"><span data-stu-id="016fb-158">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="016fb-159">Проверьте изменения, отобразив текущие назначенные роли:</span><span class="sxs-lookup"><span data-stu-id="016fb-159">Verify the changes by listing the currently assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE]
> <span data-ttu-id="016fb-160">Если у вашей учетной записи нет достаточных разрешений для назначения ролей, вы получите сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="016fb-160">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="016fb-161">В нем будет указано, что ваша учетная запись не авторизована для выполнения действия "Microsoft.Authorization/roleAssignments/write в области /subscriptions/{guid}".</span><span class="sxs-lookup"><span data-stu-id="016fb-161">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>

## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="016fb-162">Изменение учетных данных субъекта безопасности</span><span class="sxs-lookup"><span data-stu-id="016fb-162">Change the credentials of a security principal</span></span>

<span data-ttu-id="016fb-163">Из соображений безопасности рекомендуется регулярно просматривать разрешения и обновлять пароли.</span><span class="sxs-lookup"><span data-stu-id="016fb-163">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="016fb-164">Можно также изменять учетные данные безопасности и управлять ими по мере изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="016fb-164">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="016fb-165">Сброс пароля субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="016fb-165">Reset a service principal password</span></span>

<span data-ttu-id="016fb-166">Для сброса текущего пароля субъекта-службы используйте команду `az ad sp reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="016fb-166">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

```azurecli-interactive
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="016fb-167">Интерфейс командной строки создаст надежный пароль, если не указывать параметр `--password`.</span><span class="sxs-lookup"><span data-stu-id="016fb-167">The CLI generates a secure password if you leave out the `--password` option.</span></span>
