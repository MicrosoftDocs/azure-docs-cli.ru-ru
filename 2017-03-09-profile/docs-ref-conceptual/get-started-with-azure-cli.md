---
title: "Начало работы с Azure CLI 2.0"
description: "Начало работы с Azure CLI 2.0 на платформах Windows, Mac или Linux."
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 5d6d7abb34fa2be571a9a49f0f84380538592807
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2017
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="91851-104">Начало работы с Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="91851-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="91851-105">Azure CLI 2.0 — это новый интерфейс командной строки Azure для управления ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="91851-105">The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.</span></span>
<span data-ttu-id="91851-106">Его можно использовать в браузере с [Azure Cloud Shell](/azure/cloud-shell/overview) или [установить](install-azure-cli.md) в macOS, Linux или Windows и запускать из командной строки.</span><span class="sxs-lookup"><span data-stu-id="91851-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="91851-107">Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="91851-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span>
<span data-ttu-id="91851-108">Эта статья поможет приступить к работе с модулем и объяснит основные принципы его работы.</span><span class="sxs-lookup"><span data-stu-id="91851-108">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

<span data-ttu-id="91851-109">Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="91851-109">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

## <a name="connect"></a><span data-ttu-id="91851-110">Подключение</span><span class="sxs-lookup"><span data-stu-id="91851-110">Connect</span></span>

<span data-ttu-id="91851-111">Самый простой способ начать работу — [запустить службу Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="91851-111">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="91851-112">Запустите Cloud Shell с верхней панели навигации портала Azure.</span><span class="sxs-lookup"><span data-stu-id="91851-112">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Значок оболочки](media/get-started-with-azure-cli/shell-icon.png)

2. <span data-ttu-id="91851-114">Выберите нужную подписку и создайте учетную запись хранения.</span><span class="sxs-lookup"><span data-stu-id="91851-114">Choose the subscription you want to use and create a storage account.</span></span>

   ![Создайте учетную запись хранения.](media/get-started-with-azure-cli/storage-prompt.png)

<span data-ttu-id="91851-116">Вы также можете [установить](install-azure-cli.md) интерфейс командной строки и запускать его локально из командной строки.</span><span class="sxs-lookup"><span data-stu-id="91851-116">You can also [install](install-azure-cli.md) the CLI and run it locally from the command line.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="91851-117">Создание группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="91851-117">Create a Resource Group</span></span>

<span data-ttu-id="91851-118">После выполнения всех настроек можно приступить к созданию ресурсов в Azure с помощью Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="91851-118">Now that we've got everything set up, let's use the Azure CLI to create resources within Azure.</span></span>

<span data-ttu-id="91851-119">Сначала создайте группу ресурсов.</span><span class="sxs-lookup"><span data-stu-id="91851-119">First, create a Resource Group.</span></span>  <span data-ttu-id="91851-120">Группы ресурсов в Azure позволяют управлять разными ресурсами, которые вы хотите логически сгруппировать.</span><span class="sxs-lookup"><span data-stu-id="91851-120">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group.</span></span>  <span data-ttu-id="91851-121">Например, вы можете создать группу ресурсов для приложения или проекта, а затем добавить в эту группу виртуальную машину, базу данных и службу CDN.</span><span class="sxs-lookup"><span data-stu-id="91851-121">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="91851-122">Создайте группу ресурсов с именем MyResourceGroup в регионе Azure *westus2*.</span><span class="sxs-lookup"><span data-stu-id="91851-122">Let's create a resource group named "MyResourceGroup" in the *westus2* region of Azure.</span></span>  <span data-ttu-id="91851-123">Используйте для этого следующую команду:</span><span class="sxs-lookup"><span data-stu-id="91851-123">To do so type the following command:</span></span>

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

<span data-ttu-id="91851-124">После создания группы ресурсов команда `az group create` выводит несколько свойств только что созданного ресурса:</span><span class="sxs-lookup"><span data-stu-id="91851-124">Once the resource group has been created, the `az group create` command outputs several properties of the newly created resource:</span></span>

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="91851-125">Создание виртуальной машины Linux</span><span class="sxs-lookup"><span data-stu-id="91851-125">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="91851-126">Теперь, когда у вас есть группа ресурсов, создайте в ней виртуальную машину Linux.</span><span class="sxs-lookup"><span data-stu-id="91851-126">Now that we have our resource group, let's create a Linux VM within it.</span></span>

<span data-ttu-id="91851-127">Вы можете создать виртуальную машину Linux из популярного образа UbuntuLTS с двумя подключенными дисками объемом от 10 до 20 ГБ с помощью следующей команды:</span><span class="sxs-lookup"><span data-stu-id="91851-127">You can create a Linux VM using the popular UbuntuLTS image, with two attached storage disks of 10 GB and 20 GB, with the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

<span data-ttu-id="91851-128">Во время выполнения предыдущей команды Azure CLI 2.0 ищет пару ключей SSH, которые хранятся в каталоге ~/.ssh.</span><span class="sxs-lookup"><span data-stu-id="91851-128">When you run the preceding command, the Azure CLI 2.0 looks for an SSH key pair stored under your ~/.ssh directory.</span></span>  <span data-ttu-id="91851-129">Если в этом каталоге нет пары ключей SSH, вы можете автоматически создать ее с помощью Azure CLI. Для этого передайте параметр --generate-ssh-keys:</span><span class="sxs-lookup"><span data-stu-id="91851-129">If you don't already have an SSH key pair stored there, you can ask the Azure CLI to automatically create one for you by passing the --generate-ssh-keys parameter:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

<span data-ttu-id="91851-130">Команда `az vm create` возвращает результаты, когда виртуальная машина создана, доступна и готова к использованию.</span><span class="sxs-lookup"><span data-stu-id="91851-130">The `az vm create` command returns output once the VM has been fully created and is ready to be accessed and used.</span></span> <span data-ttu-id="91851-131">Результат содержит несколько свойств только что созданной виртуальной машины, в том числе ее общедоступный IP-адрес:</span><span class="sxs-lookup"><span data-stu-id="91851-131">The output includes several properties of the newly created VM including its public IP address:</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="91851-132">Вы можете войти на созданную виртуальную машину Linux, используя **SSH** и общедоступный IP-адрес этой виртуальной машины:</span><span class="sxs-lookup"><span data-stu-id="91851-132">Now that the VM has been created, you can log on to your new Linux VM using **SSH** with the public IP address of the VM you created:</span></span>

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a><span data-ttu-id="91851-133">Создание виртуальной машины Windows Server</span><span class="sxs-lookup"><span data-stu-id="91851-133">Create a Windows Server Virtual Machine</span></span>

<span data-ttu-id="91851-134">Теперь создадим виртуальную машину на основе центра обработки данных Windows Server 2016 с помощью команды `az vm create` и добавим ее в ту же группу ресурсов MyResourceGroup, которую мы использовали для виртуальной машины Linux.</span><span class="sxs-lookup"><span data-stu-id="91851-134">Let's now create a Windows Server 2016 Datacenter-based VM using the `az vm create` command and add it to the same "MyResourceGroup" resource group that we used for our Linux VM.</span></span>  <span data-ttu-id="91851-135">Как и в примере с виртуальной машиной Linux, мы подключим два диска хранилища с помощью параметра `--data-disk-sizes-gb`.</span><span class="sxs-lookup"><span data-stu-id="91851-135">Like the Linux VM example, we'll also attach two storage disks using the `--data-disk-sizes-gb` parameter.</span></span>

<span data-ttu-id="91851-136">Не используйте в Azure имена пользователей и пароли, которые можно легко подобрать.</span><span class="sxs-lookup"><span data-stu-id="91851-136">Azure requires that you avoid using easily guessed usernames/passwords.</span></span> <span data-ttu-id="91851-137">Существуют правила, которые описывают, какие символы можно использовать, и указывают минимальную длину имени пользователя и пароля.</span><span class="sxs-lookup"><span data-stu-id="91851-137">There are specific rules for what characters can be used as well as the minimum length of both username and password.</span></span>  

> [!NOTE]
> <span data-ttu-id="91851-138">При выполнении этой команды вам будет предложено ввести имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="91851-138">You will be prompted to enter your username and password when running this command.</span></span>

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

<span data-ttu-id="91851-139">Команда `az vm create` возвращает результаты, когда виртуальная машина создана, доступна и готова к использованию.</span><span class="sxs-lookup"><span data-stu-id="91851-139">The `az vm create` command output results once the VM has been fully created and is ready to be accessed and used.</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="91851-140">Теперь войдите на созданную виртуальную машину Windows Server, используя протокол RDP и общедоступный IP-адрес этой виртуальной машины (они отображаются в результате выполнения команды `az vm create`).</span><span class="sxs-lookup"><span data-stu-id="91851-140">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM (which is returned in the output from `az vm create`).</span></span>  
<span data-ttu-id="91851-141">Если вы работаете на компьютере Windows, вы можете отобразить IP-адрес, выполнив команду `mstsc` в командной строке:</span><span class="sxs-lookup"><span data-stu-id="91851-141">If you are on a Windows-based system, you can do this from the command line using the `mstsc` command:</span></span>

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="91851-142">Для входа укажите те же учетные данные (имя пользователя и пароль), которые вы использовали при создании виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="91851-142">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="91851-143">Создание других ресурсов в Azure</span><span class="sxs-lookup"><span data-stu-id="91851-143">Creating other resources in Azure</span></span>

<span data-ttu-id="91851-144">Вы узнали, как создавать группы ресурсов, а также виртуальные машины Linux и Windows Server.</span><span class="sxs-lookup"><span data-stu-id="91851-144">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="91851-145">Но вы также можете создать в Azure много других ресурсов.</span><span class="sxs-lookup"><span data-stu-id="91851-145">You can create many other types of Azure resources as well.</span></span>  

<span data-ttu-id="91851-146">Все новые ресурсы создаются с помощью согласованного шаблона именования `az <resource type name> create`.</span><span class="sxs-lookup"><span data-stu-id="91851-146">All new resources are created using a consistent `az <resource type name> create` naming pattern.</span></span>  <span data-ttu-id="91851-147">Например, чтобы создать подсистему балансировки нагрузки Azure, которую можно затем связать с новой виртуальной машиной, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="91851-147">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

<span data-ttu-id="91851-148">Также для своей инфраструктуры вы можете создать новую частную виртуальную сеть, используя следующую команду создания:</span><span class="sxs-lookup"><span data-stu-id="91851-148">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following create command:</span></span>

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

<span data-ttu-id="91851-149">Преимущество Azure и Azure CLI заключается в том, что их можно использовать для создания как облачной инфраструктуры, так и управляемых служб платформы.</span><span class="sxs-lookup"><span data-stu-id="91851-149">What makes Azure and the Azure CLI powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span>  <span data-ttu-id="91851-150">Управляемые службы платформы также можно объединять с инфраструктурой, создавая еще более мощные решения.</span><span class="sxs-lookup"><span data-stu-id="91851-150">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="91851-151">Например, используя Azure CLI, можно создать службу приложений Azure.</span><span class="sxs-lookup"><span data-stu-id="91851-151">For example, you can use the Azure CLI to create an Azure AppService.</span></span>  <span data-ttu-id="91851-152">Служба приложений Azure — это управляемая служба платформы, на которой можно размещать веб-приложения, не беспокоясь об инфраструктуре.</span><span class="sxs-lookup"><span data-stu-id="91851-152">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span>  <span data-ttu-id="91851-153">Создав службу приложений Azure, можно создать два новых веб-приложения Azure с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="91851-153">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following create commands:</span></span>

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

<span data-ttu-id="91851-154">Ознакомившись с основами шаблона `az <resource type name> create`, вы можете легко создавать любые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="91851-154">Once you understand the basics of the `az <resource type name> create` pattern, it becomes easy to create anything.</span></span> <span data-ttu-id="91851-155">Ниже приведены некоторые популярные типы ресурсов Azure и соответствующие команды Azure CLI для их создания.</span><span class="sxs-lookup"><span data-stu-id="91851-155">Following are some popular Azure resource types and the corresponding Azure CLI create commands to create them:</span></span>

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

<span data-ttu-id="91851-156">Сведения о дополнительных параметрах для каждого ресурса, которые можно передать соответствующей команде, и типы ресурсов, которые можно создать, см. в [справочной документации](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="91851-156">Visit the [Reference documentation](/cli/azure) to learn more about the additional resource-specific parameters that you can pass to each of the preceding commands and the resource types you can create.</span></span> 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a><span data-ttu-id="91851-157">Полезный совет: оптимизируйте операции создания с помощью параметра --no-wait</span><span class="sxs-lookup"><span data-stu-id="91851-157">Useful tip: Optimizing create operations using --no-wait</span></span>

<span data-ttu-id="91851-158">По умолчанию при создании ресурсов с помощью Azure CLI 2.0 команда `az <resource type name> create` ждет, пока ресурс не будет создан и готов к использованию.</span><span class="sxs-lookup"><span data-stu-id="91851-158">By default when you create resources using the Azure CLI 2.0, the `az <resource type name> create` command waits until the resource has been created and is ready for you to use.</span></span>  <span data-ttu-id="91851-159">Например, если создать виртуальную машину, команда `az vm create` по умолчанию не возвращает результаты, пока виртуальная машина не будет создана и готова для доступа с помощью SSH или удаленного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="91851-159">For example, if you create a VM, the `az vm create` command will, by default, not return until the VM is created and is ready for you to SSH or RDP into it.</span></span>

<span data-ttu-id="91851-160">Мы используем этот подход, потому что так проще писать сценарии автоматизации, которые содержат несколько этапов с зависимостями и ждут выполнения предыдущей задачи, прежде чем перейти к следующей.</span><span class="sxs-lookup"><span data-stu-id="91851-160">We use this approach because it makes it easier to write automation scripts that contain multiple steps with dependencies (and need a prior task to have completed successfully before continuing).</span></span>

<span data-ttu-id="91851-161">Если вам для перехода к следующей задаче не нужно ждать завершения создания ресурса, можно использовать параметр `no-wait` для запуска команды создания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="91851-161">If you do not need to wait on creation of a resource before continuing, you can use the `no-wait` option to start a create action in the background.</span></span> <span data-ttu-id="91851-162">В это время вы можете использовать интерфейс командной строки для других команд.</span><span class="sxs-lookup"><span data-stu-id="91851-162">You can continue using the CLI for other commands.</span></span>

<span data-ttu-id="91851-163">Например, если использовать команду `az vm create`, как показано ниже, она запускает развертывание виртуальной машины и очень быстро возвращает результаты (еще до полной загрузки виртуальной машины):</span><span class="sxs-lookup"><span data-stu-id="91851-163">For example, the following usage of the `az vm create` starts a VM deployment and then return much more quickly (and before the VM has fully booted):</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

<span data-ttu-id="91851-164">Используя параметр `--no-wait`, можно существенно оптимизировать производительность сценариев автоматизации.</span><span class="sxs-lookup"><span data-stu-id="91851-164">Using the `--no-wait` approach can help you optimize the performance of your automation scripts considerably.</span></span>

## <a name="listing-resources-and-formatting-output"></a><span data-ttu-id="91851-165">Вывод списка ресурсов и форматирование результатов</span><span class="sxs-lookup"><span data-stu-id="91851-165">Listing resources and formatting output</span></span>

<span data-ttu-id="91851-166">С помощью команды `list` в Azure CLI можно найти и вывести список ресурсов, работающих в Azure.</span><span class="sxs-lookup"><span data-stu-id="91851-166">You can use the `list` command within the Azure CLI to find and list the resources running in Azure.</span></span> 

<span data-ttu-id="91851-167">Как и при использовании команды создания, вы можете вывести список ресурсов с помощью стандартного для Azure CLI 2.0 шаблона именования `az <resource type name> list`, одинакового для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="91851-167">Like with the create command, you can list resources using the Azure CLI 2.0 using a common `az <resource type name> list` naming pattern that is consistent across all resource types.</span></span>  <span data-ttu-id="91851-168">Используя различные доступные форматы и варианты запросов, можно фильтровать и сортировать список ресурсов, чтобы его было удобно просматривать.</span><span class="sxs-lookup"><span data-stu-id="91851-168">There are various output formats and query options available to filter and sort the list of resources in the way you prefer to see them.</span></span>

<span data-ttu-id="91851-169">Например, команда `az vm list` отображает список всех ваших виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="91851-169">For example, `az vm list` shows the list of all VMs you have.</span></span>   

```azurecli-interactive
az vm list 
```
<span data-ttu-id="91851-170">Результаты по умолчанию возвращаются в формате JSON (для краткости отображается только часть результата).</span><span class="sxs-lookup"><span data-stu-id="91851-170">The values returned are by default in JSON (only showing partial output for sake of brevity).</span></span>

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...   
]
```

<span data-ttu-id="91851-171">С помощью параметра `--output` при необходимости можно изменить формат результата.</span><span class="sxs-lookup"><span data-stu-id="91851-171">You can optionally modify the output format using the `--output` option.</span></span>  <span data-ttu-id="91851-172">Выполните команду `az vm list`, чтобы увидеть виртуальные машины Windows Server и Linux, созданные ранее, а также общие свойства виртуальной машины в удобном для чтения формате *таблицы*:</span><span class="sxs-lookup"><span data-stu-id="91851-172">Run the `az vm list` command to see both the Linux and Windows Server VMs created earlier, along with the most common properties of a VM, using the easy to read *table* format option:</span></span>

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="91851-173">Параметр *tsv* можно использовать для вывода результатов в виде текста, разделенного символами табуляции без заголовков.</span><span class="sxs-lookup"><span data-stu-id="91851-173">The *tsv* output option can be used to get a text-based, tab-separated format without any headers.</span></span>  <span data-ttu-id="91851-174">Этот формат удобен в тех случаях, когда требуется передать результат в другой текстовый инструмент, например grep.</span><span class="sxs-lookup"><span data-stu-id="91851-174">This format is useful when you want to pipe the output into another text-based tool like grep.</span></span> 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
<span data-ttu-id="91851-175">Дополнительные способы вывода списка ресурсов и форматирования выходных данных см.в [этой статье](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="91851-175">Visit the [output formats](format-output-azure-cli.md) article to learn more about the additional ways to list resources and format the output.</span></span>

## <a name="querying-resources-and-shaping-outputs"></a><span data-ttu-id="91851-176">Запрос ресурсов и предоставление доступа к результатам</span><span class="sxs-lookup"><span data-stu-id="91851-176">Querying resources and shaping outputs</span></span>

<span data-ttu-id="91851-177">Часто необходимо иметь возможность запросить только те ресурсы, которые отвечают определенному условию.</span><span class="sxs-lookup"><span data-stu-id="91851-177">Often you want to be able to query for only those resources that meet a specific condition.</span></span>  

<span data-ttu-id="91851-178">Команда `list` оснащена встроенной функцией, которая упрощает фильтрацию ресурсов по имени группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="91851-178">The `list` command has built-in support that makes it easy to filter resources by Resource Group name.</span></span>  <span data-ttu-id="91851-179">Например, вы можете передать параметр `--ResourceGroup` или `-g` в команду `list`, чтобы извлечь только эти ресурсы в определенной группе ресурсов:</span><span class="sxs-lookup"><span data-stu-id="91851-179">For example, you can pass either a `--ResourceGroup` or `-g` parameter to a `list` command to only retrieve those resources within a specific resource group:</span></span>


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="91851-180">Еще более мощные функции выполнения запросов доступны при использовании параметра `--query` для выполнения запроса JMESPath в результатах *любой* команды`az`.</span><span class="sxs-lookup"><span data-stu-id="91851-180">For even more powerful querying support, you can use the `--query` parameter to execute a JMESPath query on the results of *any* `az` command.</span></span>  <span data-ttu-id="91851-181">С помощью запросов JMESPath можно фильтровать и формировать любые возвращенные результаты.</span><span class="sxs-lookup"><span data-stu-id="91851-181">JMESPath queries can be used both to filter as well as shape the output of any returned result.</span></span>

<span data-ttu-id="91851-182">Например, выполните следующую команду, чтобы запросить любой ресурс виртуальной машины в любой группе ресурсов, который содержит буквы "My":</span><span class="sxs-lookup"><span data-stu-id="91851-182">For example, execute the following command to query for any VM resource within any resource group that contains the letters "My":</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="91851-183">Затем можно еще раз уточнить результаты с помощью функции формирования запросов JMESPath, чтобы вывести другие значения.</span><span class="sxs-lookup"><span data-stu-id="91851-183">We could then choose to further refine the output by using the shaping capability of JMESPath queries to output different values as well.</span></span>  <span data-ttu-id="91851-184">Например, следующая команда извлекает тип диска операционной системы виртуальной машины, чтобы определить, работает ли виртуальная машина на ОС Linux или Windows:</span><span class="sxs-lookup"><span data-stu-id="91851-184">For example, the following command retrieves the type of OS disk the VM is using to determine whether the OS is Linux or Windows based:</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

<span data-ttu-id="91851-185">Функция JMESPath очень эффективно работает в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="91851-185">The JMESPath support in Azure CLI is powerful.</span></span>  <span data-ttu-id="91851-186">Дополнительные сведения о том, как ее использовать, см. в статье о [выполнении запросов](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="91851-186">Learn more about how to use it in our [query](query-azure-cli.md) article.</span></span>

## <a name="deleting-resources"></a><span data-ttu-id="91851-187">Удаление ресурсов</span><span class="sxs-lookup"><span data-stu-id="91851-187">Deleting resources</span></span>

<span data-ttu-id="91851-188">Используйте в Azure CLI команду `delete` для удаления ресурсов, которые больше не нужны.</span><span class="sxs-lookup"><span data-stu-id="91851-188">You can use the `delete` command within Azure CLI to delete the resources you no longer need.</span></span> <span data-ttu-id="91851-189">Команду `delete`, как и команду `create`, можно применять к любому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="91851-189">You can use the `delete` command with any resource just like you can with the `create` command.</span></span>

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

<span data-ttu-id="91851-190">По умолчанию интерфейс командной строки попросит подтвердить удаление.</span><span class="sxs-lookup"><span data-stu-id="91851-190">By default the CLI prompts to confirm deletion.</span></span>  <span data-ttu-id="91851-191">Вы можете отключить этот запрос в автоматизированных сценариях.</span><span class="sxs-lookup"><span data-stu-id="91851-191">You can suppress this prompt for automated scripts.</span></span>

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

<span data-ttu-id="91851-192">С помощью команды `delete` можно удалить несколько ресурсов одновременно.</span><span class="sxs-lookup"><span data-stu-id="91851-192">You can also use the `delete` command to delete many resources at a time.</span></span> <span data-ttu-id="91851-193">Например, следующая команда удаляет всю группу ресурсов MyResourceGroup, которая использовалась во всех примерах в этом руководстве по началу работы.</span><span class="sxs-lookup"><span data-stu-id="91851-193">For example, the following command deletes all the resources in the "MyResourceGroup" resource group that we've used for all the samples in this Get Started tutorial.</span></span>

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a><span data-ttu-id="91851-194">Получение примеров</span><span class="sxs-lookup"><span data-stu-id="91851-194">Get samples</span></span>

<span data-ttu-id="91851-195">Дополнительные сведения о способах использования Azure CLI см. в примерах популярных сценариев для [виртуальных машин Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [виртуальных машин Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [веб-приложений](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) и [баз данных SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="91851-195">To learn more about ways to use the Azure CLI, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), and [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span></span>

## <a name="read-the-api-reference-docs"></a><span data-ttu-id="91851-196">Знакомство со справочной документацией по API</span><span class="sxs-lookup"><span data-stu-id="91851-196">Read the API reference docs</span></span>

[<span data-ttu-id="91851-197">Справочник по API</span><span class="sxs-lookup"><span data-stu-id="91851-197">API reference</span></span>](/cli/azure)

## <a name="get-help"></a><span data-ttu-id="91851-198">Получение справки</span><span class="sxs-lookup"><span data-stu-id="91851-198">Get help</span></span>

<span data-ttu-id="91851-199">Azure CLI содержит встроенную справочную документацию, которая соответствует документации на веб-сайте. Ее можно открыть из командной строки:</span><span class="sxs-lookup"><span data-stu-id="91851-199">The Azure CLI has built-in help documentation, which matches our web documentation that you can run from the command line:</span></span>

```azurecli-interactive
az [command-group [command]] -h
```

<span data-ttu-id="91851-200">Например, чтобы узнать, какие команды и подгруппы доступны для виртуальных машин, выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="91851-200">For example, to see what commands and subgroups are available for VMs, use:</span></span>

```azurecli-interactive
az vm -h
```

<span data-ttu-id="91851-201">Чтобы получить справку по команде, которая создает виртуальную машину, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="91851-201">To get help with the command to create a VM, use:</span></span>

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a><span data-ttu-id="91851-202">Переход с Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="91851-202">Switch from Azure CLI 1.0</span></span>

<span data-ttu-id="91851-203">Если вы уже знакомы с Azure CLI 1.0 (azure.js), вы могли заметить отличия в командах новой версии.</span><span class="sxs-lookup"><span data-stu-id="91851-203">If you already know how to use Azure CLI 1.0 (azure.js), you'll notice places where the commands aren't quite the same.</span></span>
<span data-ttu-id="91851-204">Некоторые команды для выполнения задач существенно отличаются.</span><span class="sxs-lookup"><span data-stu-id="91851-204">Sometimes the commands to perform a task are significantly different.</span></span>
<span data-ttu-id="91851-205">При переходе с Azure CLI 1.0 на Azure CLI 2.0 поможет этот список [сопоставления команд](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span><span class="sxs-lookup"><span data-stu-id="91851-205">To help you make the switch from Azure CLI 1.0 to Azure CLI 2.0, we've started this [command mapping](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span></span>

## <a name="send-us-your-feedback"></a><span data-ttu-id="91851-206">Отправка отзывов</span><span class="sxs-lookup"><span data-stu-id="91851-206">Send us your feedback</span></span>

```azurecli-interactive
az feedback
```
