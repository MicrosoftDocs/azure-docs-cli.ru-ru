---
title: "Создание субъекта-службы Azure с помощью Azure CLI 2.0"
description: "Узнайте, как создать субъект-службу для приложения или службы с помощью Azure CLI 2.0."
keywords: "Azure CLI 2.0, Azure Active Directory, Azure Active Directory, AD, RBAC"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: 0ee794d5a732c6e8d2d52fca5810a874827930ae
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="1f135-104">Создание субъекта-службы Azure с помощью Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="1f135-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="1f135-105">Если вы планируете управлять приложением или службой с помощью Azure CLI 2.0, вы должны запустить это приложение или службу с помощью субъекта-службы Azure Active Directory (AAD), а не своих учетных данных.</span><span class="sxs-lookup"><span data-stu-id="1f135-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="1f135-106">В этой статье объясняется, как создать субъект безопасности с помощью Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="1f135-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="1f135-107">Можно также создать субъект-службу на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1f135-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="1f135-108">Дополнительные сведения см. в статье [Создание приложения Azure Active Directory и субъекта-службы с доступом к ресурсам с помощью портала](/azure/azure-resource-manager/resource-group-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="1f135-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="1f135-109">Что такое субъект-служба?</span><span class="sxs-lookup"><span data-stu-id="1f135-109">What is a 'service principal'?</span></span>

<span data-ttu-id="1f135-110">Субъект-служба Azure — это идентификатор безопасности, который используют созданные пользователем приложения, службы и средства автоматизации для доступа к определенным ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="1f135-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="1f135-111">Это что-то вроде удостоверения пользователя (имя для входа и пароль или сертификат) с определенной ролью и строго контролируемыми разрешениями на доступ к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="1f135-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="1f135-112">Субъект-служба должен выполнять только конкретные задачи, в отличие от удостоверений пользователей.</span><span class="sxs-lookup"><span data-stu-id="1f135-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="1f135-113">Для повышения безопасности следует предоставить ему только минимально необходимый уровень разрешений для выполнения задач управления.</span><span class="sxs-lookup"><span data-stu-id="1f135-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="1f135-114">Сейчас Azure CLI 2.0 поддерживает только создание учетных данных с проверкой подлинности на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="1f135-114">Right now, Azure CLI 2.0 only supports the creation of password-based authentication credentials.</span></span> <span data-ttu-id="1f135-115">В этой статье мы рассмотрим создание субъекта-службы с определенным паролем и дополнительное назначение ему конкретных ролей.</span><span class="sxs-lookup"><span data-stu-id="1f135-115">In this topic, we cover creating a service principal with a specific password, and optionally assigning specific roles to it.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="1f135-116">Проверка вашего уровня разрешений</span><span class="sxs-lookup"><span data-stu-id="1f135-116">Verify your own permission level</span></span>

<span data-ttu-id="1f135-117">Во-первых, у вас должен быть достаточный уровень разрешений в Azure Active Directory и подписке Azure.</span><span class="sxs-lookup"><span data-stu-id="1f135-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="1f135-118">В частности, у вас должно быть право создавать приложения в Active Directory и назначать роли субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="1f135-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="1f135-119">Проверить, есть ли у вас соответствующие разрешения, проще всего на портале.</span><span class="sxs-lookup"><span data-stu-id="1f135-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="1f135-120">Ознакомьтесь с [проверкой наличия необходимых разрешений на портале](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="1f135-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="1f135-121">Создание субъекта-службы для приложения</span><span class="sxs-lookup"><span data-stu-id="1f135-121">Create a service principal for your application</span></span>

<span data-ttu-id="1f135-122">Необходимо иметь один из следующих параметров для определения приложения, которое нужно создать для субъекта-службы:</span><span class="sxs-lookup"><span data-stu-id="1f135-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="1f135-123">уникальное имя или URI развернутого приложения (например, MyDemoWebApp в следующих примерах);</span><span class="sxs-lookup"><span data-stu-id="1f135-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="1f135-124">идентификатор приложения — глобальный уникальный идентификатор, связанный с развернутым приложением, службой или объектом.</span><span class="sxs-lookup"><span data-stu-id="1f135-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="1f135-125">Эти значения идентифицируют ваше приложение при создании субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1f135-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="1f135-126">Получение сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="1f135-126">Get information about your application</span></span>

<span data-ttu-id="1f135-127">Получить сведения для идентификации приложения можно с помощью команды `az ad app list`.</span><span class="sxs-lookup"><span data-stu-id="1f135-127">Get identity information about your application with the `az ad app list`.</span></span>

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

<span data-ttu-id="1f135-128">Параметр `--display-name` фильтрует возвращаемый список приложений, чтобы показать те, которые содержат `displayName`, начиная с MyDemoWebApp.</span><span class="sxs-lookup"><span data-stu-id="1f135-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-the-service-principal"></a><span data-ttu-id="1f135-129">Создание субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1f135-129">Create the service principal</span></span>

<span data-ttu-id="1f135-130">Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="1f135-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) to create the service principal.</span></span> 

```azurecli-interactive
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
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
 > <span data-ttu-id="1f135-131">Не используйте ненадежный пароль.</span><span class="sxs-lookup"><span data-stu-id="1f135-131">Don't create an insecure password.</span></span>  <span data-ttu-id="1f135-132">Следуйте руководству по [правилам и ограничениям для паролей Azure AD](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="1f135-132">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="1f135-133">Получение сведений о субъекте-службе</span><span class="sxs-lookup"><span data-stu-id="1f135-133">Get information about the service principal</span></span>

```azurecli-interactive
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
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

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="1f135-134">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1f135-134">Sign in using the service principal</span></span>

<span data-ttu-id="1f135-135">Теперь вы можете войти от имени нового субъекта-службы вашего приложения, используя *идентификатор приложения* и *пароль*, указанные в команде `az ad sp show`.</span><span class="sxs-lookup"><span data-stu-id="1f135-135">You can now log in as the new service principal for your app using the *appId* and *password* from `az ad sp show`.</span></span>  <span data-ttu-id="1f135-136">Укажите значение параметра *tenant*, полученное в результате выполнения команды `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1f135-136">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

<span data-ttu-id="1f135-137">После успешного входа отобразится следующее:</span><span class="sxs-lookup"><span data-stu-id="1f135-137">You will see this output after a successful sign-on:</span></span>

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

<span data-ttu-id="1f135-138">Используйте значения `id`, `password` и `tenant` в качестве учетных данных для запуска приложения.</span><span class="sxs-lookup"><span data-stu-id="1f135-138">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="1f135-139">Управление ролями</span><span class="sxs-lookup"><span data-stu-id="1f135-139">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="1f135-140">Управление доступом на основе ролей в Azure (RBAC) — это модель для определения ролей пользователя и субъектов-служб и управления этими ролями.</span><span class="sxs-lookup"><span data-stu-id="1f135-140">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="1f135-141">Ролям назначаются связанные наборы разрешений, которые определяют ресурсы, доступные субъекту для чтения, доступа, записи или управления.</span><span class="sxs-lookup"><span data-stu-id="1f135-141">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="1f135-142">Дополнительные сведения о RBAC и ролях см. в статье [Встроенные роли для управления доступом на основе ролей в Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="1f135-142">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="1f135-143">В Azure CLI 2.0 доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="1f135-143">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* <span data-ttu-id="1f135-144">[az role assignment list](/cli/azure/role/assignment#list);</span><span class="sxs-lookup"><span data-stu-id="1f135-144">[az role assignment list](/cli/azure/role/assignment#list)</span></span>
* <span data-ttu-id="1f135-145">[az role assignment create](/cli/azure/role/assignment#create);</span><span class="sxs-lookup"><span data-stu-id="1f135-145">[az role assignment create](/cli/azure/role/assignment#create)</span></span>
* <span data-ttu-id="1f135-146">[az role assignment delete](/cli/azure/role/assignment#delete).</span><span class="sxs-lookup"><span data-stu-id="1f135-146">[az role assignment delete](/cli/azure/role/assignment#delete)</span></span>

<span data-ttu-id="1f135-147">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="1f135-147">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="1f135-148">Возможно, это не лучший выбор для взаимодействия приложения со службами Azure, учитывая широкие разрешения у этой роли.</span><span class="sxs-lookup"><span data-stu-id="1f135-148">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="1f135-149">Роль **читателя** имеет больше ограничений и отлично подходит для доступа с правами только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f135-149">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="1f135-150">Вы можете просмотреть сведения о разрешениях каждой роли или создать пользовательские разрешения на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1f135-150">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="1f135-151">В этом примере мы добавим роль **читателя** к предыдущему примеру и удалим роль **участника**:</span><span class="sxs-lookup"><span data-stu-id="1f135-151">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="1f135-152">Проверьте изменения, отобразив текущие назначенные роли:</span><span class="sxs-lookup"><span data-stu-id="1f135-152">Verify the changes by listing the currently assigned roles:</span></span>

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
> <span data-ttu-id="1f135-153">Если у вашей учетной записи нет достаточных разрешений для назначения ролей, вы получите сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="1f135-153">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="1f135-154">В нем будет указано, что ваша учетная запись не авторизована для выполнения действия "Microsoft.Authorization/roleAssignments/write в области /subscriptions/{guid}".</span><span class="sxs-lookup"><span data-stu-id="1f135-154">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="1f135-155">Изменение учетных данных субъекта безопасности</span><span class="sxs-lookup"><span data-stu-id="1f135-155">Change the credentials of a security principal</span></span>

<span data-ttu-id="1f135-156">Из соображений безопасности рекомендуется регулярно просматривать разрешения и обновлять пароли.</span><span class="sxs-lookup"><span data-stu-id="1f135-156">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="1f135-157">Можно также изменять учетные данные безопасности и управлять ими по мере изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1f135-157">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="1f135-158">Сброс пароля субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1f135-158">Reset a service principal password</span></span>

<span data-ttu-id="1f135-159">Для сброса текущего пароля субъекта-службы используйте команду `az ad sp reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="1f135-159">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

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

<span data-ttu-id="1f135-160">Интерфейс командной строки создаст надежный пароль, если не указывать параметр `--password`.</span><span class="sxs-lookup"><span data-stu-id="1f135-160">The CLI generates a secure password if you leave out the `--password` option.</span></span>