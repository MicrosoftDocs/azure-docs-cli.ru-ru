---
title: Установка Azure CLI 2.0 в Linux с помощью apt
description: Как установить Azure CLI 2.0 с помощью apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/06/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 86d601fdc375ec59c4f7cbf0881bc67a08e24b19
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="6f3d9-103">Установка Azure CLI 2.0 с помощью apt</span><span class="sxs-lookup"><span data-stu-id="6f3d9-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="6f3d9-104">Если вы используете дистрибутив, который поставляется с `apt`, например Ubuntu или Debian, можно применить 64-разрядный пакет для Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="6f3d9-105">Этот пакет протестирован со следующими версиями:</span><span class="sxs-lookup"><span data-stu-id="6f3d9-105">This package has been tested with:</span></span>

* <span data-ttu-id="6f3d9-106">Ubuntu wheezy, xenial и artful</span><span class="sxs-lookup"><span data-stu-id="6f3d9-106">Ubuntu trusty, xenial, and artful</span></span>
* <span data-ttu-id="6f3d9-107">Debian wheezy, jessie и stretch</span><span class="sxs-lookup"><span data-stu-id="6f3d9-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="6f3d9-108">Install</span><span class="sxs-lookup"><span data-stu-id="6f3d9-108">Install</span></span>

1. <span data-ttu-id="6f3d9-109">Измените список источников.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-109">Modify your sources list:</span></span>

     ```bash
     AZ_REPO=$(lsb_release -cs)
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="6f3d9-110">Получите ключ подписывания Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
   ```

  > [!WARNING]
  > <span data-ttu-id="6f3d9-111">Этот ключ подписывания больше не рекомендуется использовать. Он будет заменен в конце мая 2018 года.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-111">This signing key is deprecated, and will be replaced at the end of May 2018.</span></span> <span data-ttu-id="6f3d9-112">Чтобы и дальше получать обновления с помощью `apt`, установите новый ключ.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-112">In order to keep getting updates with `apt`, make sure that you also install the new key:</span></span>
  > 
  > ```bash
  > curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  > ``` 

3. <span data-ttu-id="6f3d9-113">Установите интерфейс командной строки.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

<span data-ttu-id="6f3d9-114">Запустите Azure CLI с помощью команды `az`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6f3d9-115">Для входа выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-115">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="6f3d9-116">Дополнительные сведения о различных методах входа см. в статье [Вход с помощью Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6f3d9-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6f3d9-117">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="6f3d9-117">Troubleshooting</span></span>

<span data-ttu-id="6f3d9-118">Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="6f3d9-119">Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6f3d9-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="6f3d9-120">Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)</span><span class="sxs-lookup"><span data-stu-id="6f3d9-120">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="6f3d9-121">При выполнении команды `apt-key` может появиться примерно такая ошибка:</span><span class="sxs-lookup"><span data-stu-id="6f3d9-121">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="6f3d9-122">Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-122">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="6f3d9-123">Ошибку можно устранить, установив пакет `dirmngr`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-123">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="6f3d9-124">Зависает apt-key</span><span class="sxs-lookup"><span data-stu-id="6f3d9-124">apt-key hangs</span></span>

<span data-ttu-id="6f3d9-125">Если при использовании брандмауэра блокируются исходящие подключения к порту 11371, команда `apt-key` может перестать работать на неопределенное время.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-125">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="6f3d9-126">Возможно, брандмауэр требует использовать для исходящих подключений прокси-сервер HTTP:</span><span class="sxs-lookup"><span data-stu-id="6f3d9-126">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="6f3d9-127">Если вы не знаете, есть ли у вас прокси-сервер, обратитесь к своему системному администратору.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-127">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="6f3d9-128">Если для прокси-сервера не требуется имя для входа, не указывайте имя пользователя, пароль и маркер `@`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-128">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="6f3d9-129">Блокировка изменений</span><span class="sxs-lookup"><span data-stu-id="6f3d9-129">Update</span></span>

<span data-ttu-id="6f3d9-130">Используйте `apt-get upgrade`, чтобы обновить пакет CLI.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-130">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="6f3d9-131">Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-131">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="6f3d9-132">Чтобы обновить только CLI, используйте `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-132">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="6f3d9-133">Удаление</span><span class="sxs-lookup"><span data-stu-id="6f3d9-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="6f3d9-134">Удалите CLI с помощью команды `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-134">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="6f3d9-135">Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-135">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="6f3d9-136">Удалите все ненужные пакеты.</span><span class="sxs-lookup"><span data-stu-id="6f3d9-136">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```
