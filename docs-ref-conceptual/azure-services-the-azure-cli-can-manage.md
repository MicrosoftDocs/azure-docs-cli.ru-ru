---
title: Службы Azure, которыми можно управлять с помощью Azure CLI
description: Ссылки на службы с доступными справочниками по Azure CLI, Конфигурация приложений, Служба приложений, Active Directory (AD), резервное копирование, Когнитивный поиск, Cosmos DB, Data Lake Storage, база данных, MariaDB, MySQL, PostgreSQL, PostgreSQL, DevOps, DevTest Labs, DNS, Функции, IoT, IoT Central, IoT Edge, Центр Интернета вещей, Служба Azure Kubernetes (AKS), Службы лабораторий, Машинное обучение, Управляемые приложения, Приватный канал, Resource Manager, Spring Cloud, База данных SQL, пакетная служба, Cognitive Services, Экземпляры контейнеров, Реестр контейнеров, Data Lake Analytics, Сетка событий, Центры событий, HDInsight, Key Vault, Load Balancer, Управляемые диски, Службы мультимедиа, Центры уведомлений, Служебная шина, Service Fabric, учетные записи хранения, Диспетчер трафика, Масштабируемые наборы виртуальных машин, виртуальная сеть, Вычислительная среда, Сеть, Интернет вещей, Средства для разработчиков, базы данных, аналитика, управление и система управления, гибридная среда, хранилище, безопасность, ИИ, искусственный интеллект и машинное обучение
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/01/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9f754e5223da0c2d2d9e4b0714ff09f8b900e361
ms.sourcegitcommit: 93d8137f37e974f7d314a0b1deb65ac563c2e2c5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "80075973"
---
# <a name="azure-services-the-azure-cli-can-manage"></a><span data-ttu-id="189e3-103">Службы Azure, которыми можно управлять с помощью Azure CLI</span><span class="sxs-lookup"><span data-stu-id="189e3-103">Azure services the Azure CLI can manage</span></span>

<span data-ttu-id="189e3-104">Azure CLI предоставляется во многих службах Azure и является гибким и мощным инструментом для создания ресурсов Azure и управления ими.</span><span class="sxs-lookup"><span data-stu-id="189e3-104">The Azure CLI is available across many Azure services, and is a flexible yet powerful tool to create and manage Azure resources.</span></span>  <span data-ttu-id="189e3-105">В этой статье представлен список служб Azure, которыми можно управлять с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="189e3-105">This article provides the list of Azure services the Azure CLI can manage.</span></span>

<span data-ttu-id="189e3-106">Справочники по Azure CLI доступны для следующих служб.</span><span class="sxs-lookup"><span data-stu-id="189e3-106">Azure CLI references are available for the following:</span></span>  

| <span data-ttu-id="189e3-107">Категория</span><span class="sxs-lookup"><span data-stu-id="189e3-107">Category</span></span> | <span data-ttu-id="189e3-108">Документация по службе</span><span class="sxs-lookup"><span data-stu-id="189e3-108">Service Documentation</span></span>
|-|-|
|<span data-ttu-id="189e3-109">Средства ИИ и машинного обучения</span><span class="sxs-lookup"><span data-stu-id="189e3-109">AI + Machine Learning</span></span>| [<span data-ttu-id="189e3-110">Машинное обучение Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-110">Azure Machine Learning</span></span>](/azure/machine-learning/)
||[<span data-ttu-id="189e3-111">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="189e3-111">Cognitive Services</span></span>](/azure/cognitive-services/)
|<span data-ttu-id="189e3-112">Analytics</span><span class="sxs-lookup"><span data-stu-id="189e3-112">Analytics</span></span>|[<span data-ttu-id="189e3-113">Хранилище озера данных Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-113">Azure Data Lake Storage</span></span>](/azure/storage/blobs/data-lake-storage-introduction/)
||[<span data-ttu-id="189e3-114">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="189e3-114">Data Lake Analytics</span></span>](/azure/data-lake-analytics/)
||[<span data-ttu-id="189e3-115">Центры событий</span><span class="sxs-lookup"><span data-stu-id="189e3-115">Event Hubs</span></span>](/azure/event-hubs/)
||[<span data-ttu-id="189e3-116">HDInsight</span><span class="sxs-lookup"><span data-stu-id="189e3-116">HDInsight</span></span>](/azure/hdinsight/)
|<span data-ttu-id="189e3-117">Блокчейн</span><span class="sxs-lookup"><span data-stu-id="189e3-117">Blockchain</span></span>|[<span data-ttu-id="189e3-118">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="189e3-118">Azure Cosmos DB</span></span>](/azure/cosmos-db/)
|<span data-ttu-id="189e3-119">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="189e3-119">Compute</span></span>|[<span data-ttu-id="189e3-120">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="189e3-120">App Service</span></span>](/azure/app-service/)
||[<span data-ttu-id="189e3-121">Функции Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-121">Azure Functions</span></span>](/azure/azure-functions/)
||[<span data-ttu-id="189e3-122">Служба Azure Kubernetes (AKS)</span><span class="sxs-lookup"><span data-stu-id="189e3-122">Azure Kubernetes Service (AKS)</span></span>](/azure/aks/)
||[<span data-ttu-id="189e3-123">Azure Spring Cloud</span><span class="sxs-lookup"><span data-stu-id="189e3-123">Azure Spring Cloud</span></span>](/azure/spring-cloud/)
||[<span data-ttu-id="189e3-124">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="189e3-124">Batch</span></span>](/azure/batch/)
||[<span data-ttu-id="189e3-125">Экземпляры контейнеров</span><span class="sxs-lookup"><span data-stu-id="189e3-125">Container Instances</span></span>](/azure/container-instances/)
||[<span data-ttu-id="189e3-126">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="189e3-126">Service Fabric</span></span>](/azure/service-fabric/)
||[<span data-ttu-id="189e3-127">Наборы для масштабирования виртуальных машин</span><span class="sxs-lookup"><span data-stu-id="189e3-127">Virtual Machine Scale Sets</span></span>](/azure/virtual-machine-scale-sets/)
|<span data-ttu-id="189e3-128">Контейнеры</span><span class="sxs-lookup"><span data-stu-id="189e3-128">Containers</span></span>|[<span data-ttu-id="189e3-129">Функции Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-129">Azure Functions</span></span>](/azure/azure-functions/)
||[<span data-ttu-id="189e3-130">Служба Azure Kubernetes (AKS)</span><span class="sxs-lookup"><span data-stu-id="189e3-130">Azure Kubernetes Service (AKS)</span></span>](/azure/aks/)
||[<span data-ttu-id="189e3-131">Экземпляры контейнеров</span><span class="sxs-lookup"><span data-stu-id="189e3-131">Container Instances</span></span>](/azure/container-instances/)
||[<span data-ttu-id="189e3-132">Реестр контейнеров</span><span class="sxs-lookup"><span data-stu-id="189e3-132">Container Registry</span></span>](/azure/container-registry/)
||[<span data-ttu-id="189e3-133">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="189e3-133">Service Fabric</span></span>](/azure/service-fabric/)
|<span data-ttu-id="189e3-134">Базы данных</span><span class="sxs-lookup"><span data-stu-id="189e3-134">Databases</span></span>|[<span data-ttu-id="189e3-135">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="189e3-135">Azure Cosmos DB</span></span>](/azure/cosmos-db/)
||[<span data-ttu-id="189e3-136">База данных Azure для MariaDB</span><span class="sxs-lookup"><span data-stu-id="189e3-136">Azure Database for MariaDB</span></span>](/azure/mariadb/)
||[<span data-ttu-id="189e3-137">База данных Azure для MySQL</span><span class="sxs-lookup"><span data-stu-id="189e3-137">Azure Database for MySQL</span></span>](/azure/mysql/)
||[<span data-ttu-id="189e3-138">База данных Azure для PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="189e3-138">Azure Database for PostgreSQL</span></span>](/azure/postgresql/)
||[<span data-ttu-id="189e3-139">База данных SQL Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-139">Azure SQL Database</span></span>](/azure/sql-database/)
|<span data-ttu-id="189e3-140">Средства для разработчиков</span><span class="sxs-lookup"><span data-stu-id="189e3-140">Developer Tools</span></span>|[<span data-ttu-id="189e3-141">Конфигурация приложений</span><span class="sxs-lookup"><span data-stu-id="189e3-141">App Configuration</span></span>](/azure/azure-app-configuration/)
||[<span data-ttu-id="189e3-142">Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="189e3-142">Azure DevOps</span></span>](/azure/devops/)
||[<span data-ttu-id="189e3-143">Azure DevTest Labs</span><span class="sxs-lookup"><span data-stu-id="189e3-143">Azure DevTest Labs</span></span>](/azure/lab-services/)
||[<span data-ttu-id="189e3-144">Службы лабораторий Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-144">Azure Lab Services</span></span>](/azure/lab-services/classroom-labs/)
|<span data-ttu-id="189e3-145">DevOps</span><span class="sxs-lookup"><span data-stu-id="189e3-145">DevOps</span></span>|[<span data-ttu-id="189e3-146">Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="189e3-146">Azure DevOps</span></span>](/azure/devops/)
||[<span data-ttu-id="189e3-147">Azure DevTest Labs</span><span class="sxs-lookup"><span data-stu-id="189e3-147">Azure DevTest Labs</span></span>](/azure/lab-services/)
|<span data-ttu-id="189e3-148">Гибридная среда</span><span class="sxs-lookup"><span data-stu-id="189e3-148">Hybrid</span></span>|[<span data-ttu-id="189e3-149">Azure Active Directory (AD)</span><span class="sxs-lookup"><span data-stu-id="189e3-149">Azure Active Directory (AD)</span></span>](/azure/active-directory/)
||[<span data-ttu-id="189e3-150">База данных Azure для PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="189e3-150">Azure Database for PostgreSQL</span></span>](/azure/postgresql/)
||[<span data-ttu-id="189e3-151">Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="189e3-151">Azure DevOps</span></span>](/azure/devops/)
||[<span data-ttu-id="189e3-152">Azure IoT Edge</span><span class="sxs-lookup"><span data-stu-id="189e3-152">Azure IoT Edge</span></span>](/azure/iot-edge/)
||[<span data-ttu-id="189e3-153">База данных SQL Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-153">Azure SQL Database</span></span>](/azure/sql-database/)
|<span data-ttu-id="189e3-154">Идентификация</span><span class="sxs-lookup"><span data-stu-id="189e3-154">Identity</span></span>|[<span data-ttu-id="189e3-155">Azure Active Directory (AD)</span><span class="sxs-lookup"><span data-stu-id="189e3-155">Azure Active Directory (AD)</span></span>](/azure/active-directory/)
|<span data-ttu-id="189e3-156">Интеграция</span><span class="sxs-lookup"><span data-stu-id="189e3-156">Integration</span></span>|[<span data-ttu-id="189e3-157">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="189e3-157">Event Grid</span></span>](/azure/event-grid/)
||[<span data-ttu-id="189e3-158">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="189e3-158">Service Bus</span></span>](/azure/service-bus/)
|<span data-ttu-id="189e3-159">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="189e3-159">Internet of Things</span></span>|[<span data-ttu-id="189e3-160">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="189e3-160">Azure Cosmos DB</span></span>](/azure/cosmos-db/)
||[<span data-ttu-id="189e3-161">Функции Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-161">Azure Functions</span></span>](/azure/azure-functions/)
||[<span data-ttu-id="189e3-162">Azure IoT Central</span><span class="sxs-lookup"><span data-stu-id="189e3-162">Azure IoT Central</span></span>](/azure/iot-central/)
||[<span data-ttu-id="189e3-163">Azure IoT Edge</span><span class="sxs-lookup"><span data-stu-id="189e3-163">Azure IoT Edge</span></span>](/azure/iot-edge/)
||[<span data-ttu-id="189e3-164">Центр Интернета вещей Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-164">Azure IoT Hub</span></span>](/azure/iot-hub/)
||[<span data-ttu-id="189e3-165">Машинное обучение Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-165">Azure Machine Learning</span></span>](/azure/machine-learning/)
||[<span data-ttu-id="189e3-166">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="189e3-166">Event Grid</span></span>](/azure/event-grid/)
|<span data-ttu-id="189e3-167">Управление</span><span class="sxs-lookup"><span data-stu-id="189e3-167">Management and Governance</span></span>|[<span data-ttu-id="189e3-168">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="189e3-168">Azure Backup</span></span>](/azure/backup/)
||[<span data-ttu-id="189e3-169">Управляемые приложения Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-169">Azure Managed Applications</span></span>](/azure/azure-resource-manager/managed-applications/)
||[<span data-ttu-id="189e3-170">Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="189e3-170">Azure Resource Manager</span></span>](/azure/azure-resource-manager/)
||[<span data-ttu-id="189e3-171">Диспетчер трафика</span><span class="sxs-lookup"><span data-stu-id="189e3-171">Traffic Manager</span></span>](/azure/traffic-manager/)
|<span data-ttu-id="189e3-172">Служба мультимедиа</span><span class="sxs-lookup"><span data-stu-id="189e3-172">Media</span></span>|[<span data-ttu-id="189e3-173">Службы мультимедиа</span><span class="sxs-lookup"><span data-stu-id="189e3-173">Media Services</span></span>](/azure/media-services/)
|<span data-ttu-id="189e3-174">Мобильные приложения</span><span class="sxs-lookup"><span data-stu-id="189e3-174">Mobile</span></span>|[<span data-ttu-id="189e3-175">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="189e3-175">App Service</span></span>](/azure/app-service/)
|<span data-ttu-id="189e3-176">Сеть</span><span class="sxs-lookup"><span data-stu-id="189e3-176">Networking</span></span>|[<span data-ttu-id="189e3-177">Azure DNS</span><span class="sxs-lookup"><span data-stu-id="189e3-177">Azure DNS</span></span>](/azure/dns/)
||[<span data-ttu-id="189e3-178">Приватный канал Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-178">Azure Private Link</span></span>](/azure/private-link/)
||[<span data-ttu-id="189e3-179">Load Balancer</span><span class="sxs-lookup"><span data-stu-id="189e3-179">Load Balancer</span></span>](/azure/load-balancer/)
||[<span data-ttu-id="189e3-180">Диспетчер трафика</span><span class="sxs-lookup"><span data-stu-id="189e3-180">Traffic Manager</span></span>](/azure/traffic-manager/)
||[<span data-ttu-id="189e3-181">Виртуальная сеть</span><span class="sxs-lookup"><span data-stu-id="189e3-181">Virtual Network</span></span>](/azure/virtual-network/)
|<span data-ttu-id="189e3-182">Безопасность</span><span class="sxs-lookup"><span data-stu-id="189e3-182">Security</span></span>|[<span data-ttu-id="189e3-183">Azure Active Directory (AD)</span><span class="sxs-lookup"><span data-stu-id="189e3-183">Azure Active Directory (AD)</span></span>](/azure/active-directory/)
||[<span data-ttu-id="189e3-184">хранилище ключей;</span><span class="sxs-lookup"><span data-stu-id="189e3-184">Key Vault</span></span>](/azure/key-vault/)
|<span data-ttu-id="189e3-185">Память</span><span class="sxs-lookup"><span data-stu-id="189e3-185">Storage</span></span>|[<span data-ttu-id="189e3-186">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="189e3-186">Azure Backup</span></span>](/azure/backup/)
||[<span data-ttu-id="189e3-187">Хранилище озера данных Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-187">Azure Data Lake Storage</span></span>](/azure/storage/blobs/data-lake-storage-introduction/)
||[<span data-ttu-id="189e3-188">Управляемые диски</span><span class="sxs-lookup"><span data-stu-id="189e3-188">Managed Disks</span></span>](/azure/virtual-machines/windows/managed-disks-overview/)
||[<span data-ttu-id="189e3-189">Учетные записи хранения</span><span class="sxs-lookup"><span data-stu-id="189e3-189">Storage Accounts</span></span>](/azure/storage/common/storage-account-overview/)
|<span data-ttu-id="189e3-190">Интернет</span><span class="sxs-lookup"><span data-stu-id="189e3-190">Web</span></span>|[<span data-ttu-id="189e3-191">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="189e3-191">App Service</span></span>](/azure/app-service/)
||[<span data-ttu-id="189e3-192">Когнитивный поиск Azure</span><span class="sxs-lookup"><span data-stu-id="189e3-192">Azure Cognitive Search</span></span>](/azure/search/)
||[<span data-ttu-id="189e3-193">Azure Spring Cloud</span><span class="sxs-lookup"><span data-stu-id="189e3-193">Azure Spring Cloud</span></span>](/azure/spring-cloud/)
||[<span data-ttu-id="189e3-194">Центры уведомлений</span><span class="sxs-lookup"><span data-stu-id="189e3-194">Notification Hubs</span></span>](/azure/notification-hubs/)

## <a name="see-also"></a><span data-ttu-id="189e3-195">См. также раздел</span><span class="sxs-lookup"><span data-stu-id="189e3-195">See also</span></span>

- [<span data-ttu-id="189e3-196">Начало работы с Azure CLI</span><span class="sxs-lookup"><span data-stu-id="189e3-196">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
- [<span data-ttu-id="189e3-197">Полный список справочников по командам Azure CLI</span><span class="sxs-lookup"><span data-stu-id="189e3-197">Full command reference list for the Azure CLI</span></span>](/cli/azure/reference-index)
- [<span data-ttu-id="189e3-198">Популярные статьи по использованию Azure CLI</span><span class="sxs-lookup"><span data-stu-id="189e3-198">Popular articles on using the Azure CLI</span></span>](popular-articles-using-the-azure-cli.md)
