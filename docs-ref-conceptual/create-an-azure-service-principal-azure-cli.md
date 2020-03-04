---
title: Использование субъектов-служб Azure с помощью Azure CLI
description: Сведения о том, как создать субъекты-службы и использовать их с помощью Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/15/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1bde944f1c443ef1a8d5aa918575fa09e6bb4714
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779624"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="1efc6-103">Создание субъекта-службы Azure с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="1efc6-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="1efc6-104">Разрешения для автоматизированных средств, которые используют службы Azure, всегда должны быть ограничены.</span><span class="sxs-lookup"><span data-stu-id="1efc6-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="1efc6-105">В качестве замены входу в приложения с использованием учетной записи пользователя с полными правами Azure предлагает субъекты-службы.</span><span class="sxs-lookup"><span data-stu-id="1efc6-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="1efc6-106">Субъект-служба Azure — это удостоверение, созданное для использования с приложениями, размещенными службами и автоматизированными средствами с целью получения доступа к ресурсам Azure.</span><span class="sxs-lookup"><span data-stu-id="1efc6-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="1efc6-107">Такой доступ ограничен ролями, которые назначены субъекту-службе, что позволяет управлять разрешениями доступа к ресурсам, в том числе на разных уровнях.</span><span class="sxs-lookup"><span data-stu-id="1efc6-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="1efc6-108">По соображениям безопасности мы рекомендуем всегда использовать субъекты-службы с автоматизированными средствами, чтобы не допускать их входа с помощью удостоверения пользователя.</span><span class="sxs-lookup"><span data-stu-id="1efc6-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="1efc6-109">В этой статье описано, как создать субъект-службу, получить сведения о нем и сбросить учетные данные с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="1efc6-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="1efc6-110">Создание субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1efc6-110">Create a service principal</span></span>

<span data-ttu-id="1efc6-111">Создайте субъект-службу с помощью команды [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="1efc6-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="1efc6-112">При создании субъекта-службы вы задаете используемый им тип аутентификации для входа.</span><span class="sxs-lookup"><span data-stu-id="1efc6-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span> 

> [!NOTE]
>
> <span data-ttu-id="1efc6-113">Если у вашей учетной записи нет прав на создание субъекта-службы, команда `az ad sp create-for-rbac` возвратит сообщение об ошибке, уведомляющее о том, что привилегий недостаточно для выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="1efc6-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="1efc6-114">Чтобы получить возможность создавать субъекты-службы, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1efc6-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="1efc6-115">Субъектам-службам доступно два вида аутентификации: на основе пароля и на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="1efc6-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="1efc6-116">Аутентификация на основе пароля</span><span class="sxs-lookup"><span data-stu-id="1efc6-116">Password-based authentication</span></span>

<span data-ttu-id="1efc6-117">Если параметры аутентификации не указаны, используется аутентификация на основе пароля, который генерируется случайным образом.</span><span class="sxs-lookup"><span data-stu-id="1efc6-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> <span data-ttu-id="1efc6-118">Начиная с версии Azure CLI 2.0.68, параметр `--password` для создания субъекта-службы с пользовательским паролем __больше не поддерживается__, что должно предотвратить случайное использование ненадежных паролей.</span><span class="sxs-lookup"><span data-stu-id="1efc6-118">As of Azure CLI 2.0.68, the `--password` parameter to create a service principal with a user-defined password is __no longer supported__ to prevent the accidental use of weak passwords.</span></span>

<span data-ttu-id="1efc6-119">Выходные данные для субъекта-службы с аутентификацией на основе пароля включают ключ `password`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-119">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="1efc6-120">__Обязательно__ скопируйте это значение, так как его нельзя получить повторно.</span><span class="sxs-lookup"><span data-stu-id="1efc6-120">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="1efc6-121">Если вы забыли пароль, [сбросьте учетные данные для субъекта-службы](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="1efc6-121">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="1efc6-122">Ключи `appId` и `tenant` отображаются в выходных данных команды `az ad sp create-for-rbac` и используются при аутентификации субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1efc6-122">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="1efc6-123">Запишите их значения, но при необходимости вы можете получить их в любой момент с помощью команды [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="1efc6-123">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="1efc6-124">Аутентификация на основе сертификата</span><span class="sxs-lookup"><span data-stu-id="1efc6-124">Certificate-based authentication</span></span>

<span data-ttu-id="1efc6-125">Аргумент `--cert` позволяет воспользоваться аутентификацией на основе сертификата.</span><span class="sxs-lookup"><span data-stu-id="1efc6-125">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="1efc6-126">При этом он требует указать существующий сертификат.</span><span class="sxs-lookup"><span data-stu-id="1efc6-126">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="1efc6-127">Убедитесь, что все средства, которые используют этот субъект-службу, имеют доступ к закрытому ключу сертификата.</span><span class="sxs-lookup"><span data-stu-id="1efc6-127">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="1efc6-128">Сертификаты должны иметь формат ASCII, например PEM, CER или DER.</span><span class="sxs-lookup"><span data-stu-id="1efc6-128">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="1efc6-129">Передайте сертификат в виде строки или воспользуйтесь форматом `@path`, чтобы загрузить сертификат из файла.</span><span class="sxs-lookup"><span data-stu-id="1efc6-129">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="1efc6-130">Чтобы использовать сертификат из Azure Key Vault, укажите аргумент `--keyvault`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-130">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="1efc6-131">В таком случае значение `--cert` будет именем сертификата.</span><span class="sxs-lookup"><span data-stu-id="1efc6-131">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="1efc6-132">Чтобы создать для аутентификации _самозаверяющий_ сертификат, укажите аргумент `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="1efc6-132">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="1efc6-133">Вы можете добавить аргумент `--keyvault`, чтобы сохранить сертификат в Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="1efc6-133">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="1efc6-134">Если используется аргумент `--keyvault`, аргумент `--cert`__обязателен__.</span><span class="sxs-lookup"><span data-stu-id="1efc6-134">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="1efc6-135">Выходные данные включают ключ `fileWithCertAndPrivateKey` (если только сертификат не хранится в Key Vault).</span><span class="sxs-lookup"><span data-stu-id="1efc6-135">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="1efc6-136">Значение этого ключа позволяет определить, где хранится сгенерированный сертификат.</span><span class="sxs-lookup"><span data-stu-id="1efc6-136">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="1efc6-137">__Обязательно__ скопируйте сертификат в безопасное расположение. В противном случае вы не сможете войти с помощью этого субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1efc6-137">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="1efc6-138">Для сертификатов, которые хранятся в Key Vault, получите закрытый ключ сертификата с помощью команды [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="1efc6-138">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="1efc6-139">В Key Vault имя секрета сертификата совпадает с именем самого сертификата.</span><span class="sxs-lookup"><span data-stu-id="1efc6-139">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="1efc6-140">В случае утраты доступа к закрытому ключу сертификата [сбросьте учетные данные субъекта-службы](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="1efc6-140">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="1efc6-141">Ключи `appId` и `tenant` отображаются в выходных данных команды `az ad sp create-for-rbac` и используются при аутентификации субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1efc6-141">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="1efc6-142">Запишите их значения, но при необходимости вы можете получить их в любой момент с помощью команды [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="1efc6-142">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="1efc6-143">Получение существующего субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1efc6-143">Get an existing service principal</span></span>

<span data-ttu-id="1efc6-144">Список субъектов-служб в клиенте можно получить с помощью команды [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="1efc6-144">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="1efc6-145">По умолчанию эта команда возвращает первые 100 субъектов-служб для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="1efc6-145">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="1efc6-146">Чтобы получить все субъекты-службы клиента, укажите аргумент `--all`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-146">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="1efc6-147">На получение такого списка может потребоваться длительное время, поэтому мы рекомендуем отфильтровать список с помощью одного из следующих аргументов:</span><span class="sxs-lookup"><span data-stu-id="1efc6-147">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="1efc6-148">`--display-name` — запрашивает субъекты-службы с _префиксом_, который совпадает с указанным именем.</span><span class="sxs-lookup"><span data-stu-id="1efc6-148">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="1efc6-149">Отображаемое имя субъекта-службы представляет собой значение, заданное при создании с помощью параметра `--name`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-149">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="1efc6-150">Если вы не указали параметр `--name` при создании субъекта-службы, используется префикс имени `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-150">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="1efc6-151">`--spn` — отфильтровывает точные совпадения имен субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="1efc6-151">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="1efc6-152">Имя субъекта-службы всегда начинается с `https://`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-152">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="1efc6-153">Если значение, которое вы использовали для аргумента `--name`, не было универсальным кодом ресурса (URI), им будет значение `https://` с последующим отображаемым именем.</span><span class="sxs-lookup"><span data-stu-id="1efc6-153">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="1efc6-154">`--show-mine` — запрашивает только те субъекты-службы, которые были созданы пользователем, вошедшим в систему.</span><span class="sxs-lookup"><span data-stu-id="1efc6-154">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="1efc6-155">`--filter` — выполняет фильтрацию _на стороне сервера_ с использованием фильтра OData.</span><span class="sxs-lookup"><span data-stu-id="1efc6-155">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="1efc6-156">Мы рекомендуем использовать этот метод, а не фильтрацию на стороне клиента с указанием аргумента CLI `--query`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-156">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="1efc6-157">Дополнительные сведения о фильтрах OData см. в статье [Синтаксис выражений OData для предложений фильтрации и упорядочивания в службе "Поиск Azure"](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="1efc6-157">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="1efc6-158">Для объектов субъектов-служб возвращаются подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="1efc6-158">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="1efc6-159">Чтобы получить только те сведения, которые нужны для входа, используйте строку запроса `[].{id:appId, tenant:appOwnerTenantId}`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-159">To get only the information necessary for sign-in, use the query string `[].{id:appId, tenant:appOwnerTenantId}`.</span></span> <span data-ttu-id="1efc6-160">Например, чтобы получить сведения для входа ото всех субъектов-служб, созданных пользователем, вошедшим в систему, выполните команду:</span><span class="sxs-lookup"><span data-stu-id="1efc6-160">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query "[].{id:appId, tenant:appOwnerTenantId}"
```

> [!IMPORTANT]
>
> <span data-ttu-id="1efc6-161">Команды `az ad sp list` или [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) позволяют получить данные о пользователе или клиенте, но не о секретах аутентификации _или_ способе аутентификации.</span><span class="sxs-lookup"><span data-stu-id="1efc6-161">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="1efc6-162">Секреты для сертификатов в Key Vault можно извлечь с помощью команды [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), но по умолчанию другие секреты не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="1efc6-162">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="1efc6-163">Если вы забыли способ аутентификации или секрет, [сбросьте учетные данные субъекта-службы](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="1efc6-163">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="1efc6-164">Управление ролями субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1efc6-164">Manage service principal roles</span></span>

<span data-ttu-id="1efc6-165">В Azure CLI доступны следующие команды для управления назначением ролей:</span><span class="sxs-lookup"><span data-stu-id="1efc6-165">The Azure CLI has the following commands to manage role assignments:</span></span>

* <span data-ttu-id="1efc6-166">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list);</span><span class="sxs-lookup"><span data-stu-id="1efc6-166">[az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)</span></span>
* <span data-ttu-id="1efc6-167">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create);</span><span class="sxs-lookup"><span data-stu-id="1efc6-167">[az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)</span></span>
* <span data-ttu-id="1efc6-168">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete).</span><span class="sxs-lookup"><span data-stu-id="1efc6-168">[az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)</span></span>

<span data-ttu-id="1efc6-169">По умолчанию субъекту-службе назначена роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="1efc6-169">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="1efc6-170">Эта роль имеет все разрешения на чтение из учетной записи Azure и запись в нее.</span><span class="sxs-lookup"><span data-stu-id="1efc6-170">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="1efc6-171">Роль **читателя** имеет больше ограничений, предоставляя права доступа только на чтение.</span><span class="sxs-lookup"><span data-stu-id="1efc6-171">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="1efc6-172">Дополнительные сведения об управлении доступом на основе ролей см. в статье [Встроенные роли для управления доступом на основе ролей в Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="1efc6-172">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="1efc6-173">В этом примере мы добавим роль **читателя** и удалим роль **участника**.</span><span class="sxs-lookup"><span data-stu-id="1efc6-173">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="1efc6-174">Если ваша учетная запись не позволяет назначать роли, вы увидите сообщение об ошибке о том, что ваша учетная запись не авторизована для выполнения действия Microsoft.Authorization/roleAssignments/write. Чтобы получить возможность управлять ролями, обратитесь к администратору Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1efc6-174">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="1efc6-175">Добавление роли _не_ ограничивает назначенные ранее разрешения.</span><span class="sxs-lookup"><span data-stu-id="1efc6-175">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="1efc6-176">При ограничении разрешений субъекта-службы обязательно удалите роль __участника__.</span><span class="sxs-lookup"><span data-stu-id="1efc6-176">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="1efc6-177">Чтобы проверить изменения, выведите назначенные роли:</span><span class="sxs-lookup"><span data-stu-id="1efc6-177">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="1efc6-178">Вход с помощью субъекта-службы</span><span class="sxs-lookup"><span data-stu-id="1efc6-178">Sign in using a service principal</span></span>

<span data-ttu-id="1efc6-179">Войдите, чтобы протестировать разрешения и учетные данные нового субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1efc6-179">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="1efc6-180">Для входа с использованием субъекта-службы вам потребуются `appId`, `tenant` и учетные данные.</span><span class="sxs-lookup"><span data-stu-id="1efc6-180">To sign in with a service prinicpal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="1efc6-181">Чтобы войти с использованием субъекта-службы с помощью пароля:</span><span class="sxs-lookup"><span data-stu-id="1efc6-181">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="1efc6-182">Чтобы войти с использованием сертификата, он должен быть доступен локально как PEM- или DER-файл в формате ASCII:</span><span class="sxs-lookup"><span data-stu-id="1efc6-182">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="1efc6-183">Дополнительные сведения о входе с использованием субъекта-службы см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="1efc6-183">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="1efc6-184">Сброс учетных данных</span><span class="sxs-lookup"><span data-stu-id="1efc6-184">Reset credentials</span></span>

<span data-ttu-id="1efc6-185">Если вы забыли учетные данные для субъекта-службы, воспользуйтесь командой [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="1efc6-185">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="1efc6-186">Команда сброса принимает те же аргументы, что и команда `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1efc6-186">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
