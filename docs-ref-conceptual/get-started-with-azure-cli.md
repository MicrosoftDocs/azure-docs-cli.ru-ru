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
ms.openlocfilehash: 0f8e494ffdd73c666b8361488db0966af01d6876
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2017
---
# <a name="get-started-with-azure-cli-20"></a>Начало работы с Azure CLI 2.0

Azure CLI 2.0 — это новый интерфейс командной строки Azure для управления ресурсами Azure.
Его можно использовать в Windows, Linux и macOS. 

Интерфейс Azure CLI 2.0 предназначен для администрирования ресурсов Azure из командной строки, а также для создания скриптов автоматизации, которые работают с Azure Resource Manager.
Эта статья поможет приступить к работе с модулем и объяснит основные принципы его работы.

Сведения о последнем выпуске см. в [заметках о выпуске](release-notes-azure-cli.md).

## <a name="install-azure-cli"></a>Установка Azure CLI

Сначала установите последнюю версию Azure CLI.

1. [Установите Azure CLI 2.0](install-azure-cli.md) на платформе, которую вы используете.

2. Чтобы проверить установку, выполните `az --version` в командной строке. 

Вы увидите номер версии Azure CLI и другие зависимые библиотеки, установленные на компьютере.  
  
Если появляется сообщение об ошибке, скорее всего во время установки интерфейса командной строки возникла проблема. См. раздел об устранении неполадок во время установки в [статье об установке Azure CLI 2.0](install-azure-cli.md#troubleshooting), чтобы получить рекомендации или опубликовать комментарий в нижней части страницы для получения справки.

## <a name="log-in-to-azure"></a>Вход в Azure

Теперь после установки интерфейса Azure CLI 2.0 вам нужно безопасно подключить его к своей учетной записи Azure. Для этого используйте команду `az login`.

1. Выполните следующую команду из командной строки.

   ```azurecli-interactive
   az login
   ```
   
   Эта команда выведет код, который понадобится на следующем шаге. 

2. Откройте в веб-браузере страницу [https://aka.ms/devicelogin](https://aka.ms/devicelogin) и введите код.
  
3. Когда появится окно для входа, войдите с использованием учетных данных Azure.

Теперь вы можете выполнять команды из Azure CLI 2.0 в ресурсах и службах Azure, доступных в вашей учетной записи.

## <a name="create-a-resource-group"></a>Создание группы ресурсов

После выполнения всех настроек можно приступить к созданию ресурсов в Azure с помощью Azure CLI.

Сначала создайте группу ресурсов.  Группы ресурсов в Azure позволяют управлять разными ресурсами, которые вы хотите логически сгруппировать.  Например, вы можете создать группу ресурсов для приложения или проекта, а затем добавить в эту группу виртуальную машину, базу данных и службу CDN.

Создайте группу ресурсов с именем MyResourceGroup в регионе Azure *westus2*.  Используйте для этого следующую команду:

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

После создания группы ресурсов команда `az group create` выводит несколько свойств только что созданного ресурса:

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

## <a name="create-a-linux-virtual-machine"></a>Создание виртуальной машины Linux

Теперь, когда у вас есть группа ресурсов, создайте в ней виртуальную машину Linux.

Вы можете создать виртуальную машину Linux из популярного образа UbuntuTLS с двумя подключенными дисками объемом от 10 до 20 ГБ с помощью следующей команды:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

Во время выполнения предыдущей команды Azure CLI 2.0 ищет пару ключей SSH, которые хранятся в каталоге ~/.ssh.  Если в этом каталоге нет пары ключей SSH, вы можете автоматически создать ее с помощью Azure CLI. Для этого передайте параметр --generate-ssh-keys:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --generate-ssh-keys
```

Команда `az vm create` возвращает результаты, когда виртуальная машина создана, доступна и готова к использованию. Результат содержит несколько свойств только что созданной виртуальной машины, в том числе ее общедоступный IP-адрес:

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

Вы можете войти на созданную виртуальную машину Linux, используя **SSH** и общедоступный IP-адрес этой виртуальной машины:

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

## <a name="create-a-windows-server-virtual-machine"></a>Создание виртуальной машины Windows Server

Теперь создадим виртуальную машину на основе центра обработки данных Windows Server 2016 с помощью команды `az vm create` и добавим ее в ту же группу ресурсов MyResourceGroup, которую мы использовали для виртуальной машины Linux.  Как и в примере с виртуальной машиной Linux, мы присоединим два диска хранилища с помощью параметра `--data-disk-sizes-gb`.

Не используйте в Azure имена пользователей и пароли, которые можно легко подобрать. Существуют правила, которые описывают, какие символы можно использовать, и указывают минимальную длину имени пользователя и пароля.  

> [!NOTE]
> При выполнении этой команды вам будет предложено ввести имя пользователя и пароль.

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

Команда `az vm create` возвращает результаты, когда виртуальная машина создана, доступна и готова к использованию.

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

Теперь войдите на созданную виртуальную машину Windows Server, используя протокол RDP и общедоступный IP-адрес этой виртуальной машины (они отображаются в результате выполнения команды `az vm create`).  
Если вы работаете на компьютере Windows, вы можете отобразить IP-адрес, выполнив команду `mstsc` в командной строке:

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

Для входа укажите те же учетные данные (имя пользователя и пароль), которые вы использовали при создании виртуальной машины.

## <a name="creating-other-resources-in-azure"></a>Создание других ресурсов в Azure

Вы узнали, как создавать группы ресурсов, а также виртуальные машины Linux и Windows Server. Но вы также можете создать в Azure много других ресурсов.  

Все новые ресурсы создаются с помощью согласованного шаблона именования `az <resource type name> create`.  Например, чтобы создать подсистему балансировки нагрузки Azure, которую можно затем связать с новой виртуальной машиной, выполните следующую команду:

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

Также для своей инфраструктуры вы можете создать новую частную виртуальную сеть, используя следующую команду создания:

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

Преимущество Azure и Azure CLI заключается в том, что их можно использовать для создания как облачной инфраструктуры, так и управляемых служб платформы.  Управляемые службы платформы также можно объединять с инфраструктурой, создавая еще более мощные решения.

Например, используя Azure CLI, можно создать службу приложений Azure.  Служба приложений Azure — это управляемая служба платформы, на которой можно размещать веб-приложения, не беспокоясь об инфраструктуре.  Создав службу приложений Azure, можно создать два новых веб-приложения Azure с помощью следующих команд:

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

Ознакомившись с основами шаблона `az <resource type name> create`, вы можете легко создавать любые ресурсы. Ниже приведены некоторые популярные типы ресурсов Azure и соответствующие команды Azure CLI для их создания.

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

Сведения о дополнительных параметрах для каждого ресурса, которые можно передать соответствующей команде, и типы ресурсов, которые можно создать, см. в [справочной документации](/azure/doc-ref-autogen). 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>Полезный совет: оптимизируйте операции создания с помощью параметра --no-wait

По умолчанию при создании ресурсов с помощью Azure CLI 2.0 команда `az <resource type name> create` ждет, пока ресурс не будет создан и готов к использованию.  Например, если создать виртуальную машину, команда `az vm create` по умолчанию не возвращает результаты, пока виртуальная машина не будет создана и готова для доступа с помощью SSH или удаленного рабочего стола.

Мы используем этот подход, потому что так проще писать сценарии автоматизации, которые содержат несколько этапов с зависимостями и ждут выполнения предыдущей задачи, прежде чем перейти к следующей.

Если вам для перехода к следующей задаче не нужно ждать завершения создания ресурса, можно использовать параметр `no-wait` для запуска команды создания в фоновом режиме. В это время вы можете использовать интерфейс командной строки для других команд.

Например, если использовать команду `az vm create`, как показано ниже, она запускает развертывание виртуальной машины и очень быстро возвращает результаты (еще до полной загрузки виртуальной машины):

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

Используя параметр `--no-wait`, можно существенно оптимизировать производительность сценариев автоматизации.

## <a name="listing-resources-and-formatting-output"></a>Вывод списка ресурсов и форматирование результатов

С помощью команды `list` в Azure CLI можно найти и вывести список ресурсов, работающих в Azure. 

Как и при использовании команды создания, вы можете вывести список ресурсов с помощью стандартного для Azure CLI 2.0 шаблона именования `az <resource type name> list`, одинакового для всех типов ресурсов.  Используя различные доступные форматы и варианты запросов, можно фильтровать и сортировать список ресурсов, чтобы его было удобно просматривать.

Например, команда `az vm list` отображает список всех ваших виртуальных машин.   

```azurecli-interactive
az vm list 
```
Результаты по умолчанию возвращаются в формате JSON (для краткости отображается только часть результата).

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

С помощью параметра `--output` при необходимости можно изменить формат результата.  Выполните команду `az vm list`, чтобы увидеть виртуальные машины Windows Server и Linux, созданные ранее, а также общие свойства виртуальной машины в удобном для чтения формате *таблицы*:

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Параметр *tsv* можно использовать для вывода результатов в виде текста, разделенного символами табуляции без заголовков.  Этот формат удобен в тех случаях, когда требуется передать результат в другой текстовый инструмент, например grep. 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
Дополнительные способы вывода списка ресурсов и форматирования выходных данных см.в [этой статье](format-output-azure-cli.md).

## <a name="querying-resources-and-shaping-outputs"></a>Запрос ресурсов и предоставление доступа к результатам

Часто необходимо иметь возможность запросить только те ресурсы, которые отвечают определенному условию.  

Команда `list` оснащена встроенной функцией, которая упрощает фильтрацию ресурсов по имени группы ресурсов.  Например, вы можете передать параметр `--ResourceGroup` или `-g` в команду `list`, чтобы извлечь только эти ресурсы в определенной группе ресурсов:


```azurecli
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Еще более мощные функции выполнения запросов доступны при использовании параметра `--query` для выполнения запроса JMESPath в результатах *любой* команды`az`.  С помощью запросов JMESPath можно фильтровать и формировать любые возвращенные результаты.

Например, выполните следующую команду, чтобы запросить любой ресурс виртуальной машины в любой группе ресурсов, который содержит буквы "My":

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Затем можно еще раз уточнить результаты с помощью функции формирования запросов JMESPath, чтобы вывести другие значения.  Например, следующая команда извлекает тип диска операционной системы виртуальной машины, чтобы определить, работает ли виртуальная машина на ОС Linux или Windows:

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

Функция JMESPath очень эффективно работает в Azure CLI.  Дополнительные сведения о том, как ее использовать, см. в статье о [выполнении запросов](query-azure-cli.md).

## <a name="deleting-resources"></a>Удаление ресурсов

Используйте в Azure CLI команду `delete` для удаления ресурсов, которые больше не нужны. Команду `delete`, как и команду `create`, можно применять к любому ресурсу.

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

По умолчанию интерфейс командной строки попросит подтвердить удаление.  Вы можете отключить этот запрос в автоматизированных сценариях.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

С помощью команды `delete` можно удалить несколько ресурсов одновременно. Например, следующая команда удаляет всю группу ресурсов MyResourceGroup, которая использовалась во всех примерах в этом руководстве по началу работы.

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>Получение примеров

Дополнительные сведения о способах использования Azure CLI см. в примерах популярных сценариев для [виртуальных машин Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [виртуальных машин Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [веб-приложений](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) и [баз данных SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).

## <a name="read-the-api-reference-docs"></a>Знакомство со справочной документацией по API

[Справочник по API](/cli/azure)

## <a name="get-help"></a>Получение справки

Azure CLI содержит встроенную справочную документацию, которая соответствует документации на веб-сайте. Ее можно открыть из командной строки:

```azurecli-interactive
az [command-group [command]] -h
```

Например, чтобы узнать, какие команды и подгруппы доступны для виртуальных машин, выполните следующую команду:

```azurecli-interactive
az vm -h
```

Чтобы получить справку по команде, которая создает виртуальную машину, используйте следующую команду:

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Переход с Azure CLI 1.0

Если вы уже знакомы с Azure CLI 1.0 (azure.js), вы могли заметить отличия в командах новой версии.
Некоторые команды для выполнения задач существенно отличаются.
При переходе с Azure CLI 1.0 на Azure CLI 2.0 поможет этот список [сопоставления команд](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).

## <a name="send-us-your-feedback"></a>Отправка отзывов

```azurecli-interactive
az feedback
```
