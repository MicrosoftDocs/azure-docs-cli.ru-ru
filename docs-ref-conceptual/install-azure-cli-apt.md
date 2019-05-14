---
title: Установка Azure CLI в Linux с помощью apt
description: Как установить Azure CLI с помощью диспетчера пакетов apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476262"
---
# <a name="install-azure-cli-with-apt"></a>Установка Azure CLI с помощью apt

Если вы используете дистрибутив, включающий `apt`, например Ubuntu или Debian, доступен пакет Azure CLI x86_64. Этот пакет протестирован и поддерживается для:

* Ubuntu Trusty, Xenial, Artful, Bionic и Disco.
* Debian wheezy, jessie и stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Пакет для Azure CLI устанавливает собственный интерпретатор Python и не использует системный Python.

## <a name="install"></a>Install

Мы предлагаем два способа установки Azure CLI с дистрибутивами, которые поддерживают `apt`: комплексный скрипт, который автоматически выполняет команды установки, и инструкции, которые вы сами можете выполнять поэтапно.

### <a name="install-with-one-command"></a>Установка с помощью одной команды

Мы предлагаем и поддерживаем скрипт, который выполняет все команды установки за один шаг. Запустите его с помощью `curl` и передайте непосредственно в `bash` или скачайте скрипт в файл и проверьте его перед запуском.

> [!IMPORTANT]
> Этот скрипт протестирован только для Ubuntu 16.04+ и Debian 8+. Он может не работать в других дистрибутивах.
> Если вы используете производный дистрибутив, например Linux Mint, следуйте инструкциям по установке вручную и выполните необходимые действия для устранения неполадок.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a>Инструкции по установке вручную

Если вы не хотите запускать скрипт как суперпользователь, воспользуйтесь приведенными ниже инструкциями, чтобы установить Azure CLI вручную.

1. Получите пакеты, необходимые для установки:

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. Скачайте и установите ключ подписывания (Майкрософт):

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Добавьте репозиторий программного обеспечения Azure CLI:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Обновите сведения о репозитории и установите пакет `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

Обновите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>Команда lsb_release не возвращает правильную версию базового дистрибутива

Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`. Это значение используется при установке для определения устанавливаемого пакета. Если вы знаете кодовое имя версии Ubuntu или Debian, на основе которой создан ваш дистрибутив, можно установить значение параметра `AZ_REPO` вручную при [добавлении репозитория](#set-release). В противном случае найдите информацию о том, как определить кодовое имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.

### <a name="no-package-for-your-distribution"></a>Для вашего дистрибутива отсутствует пакет

Иногда между выпуском дистрибутива и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время. Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей. Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.

Для этого вручную установите значение `AZ_REPO` при [добавлении репозитория](#set-release). Для дистрибутивов Ubuntu используйте репозиторий `disco`, а для дистрибутивов Debian используйте репозиторий `stretch`. Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Блокировка изменений

Используйте `apt-get upgrade`, чтобы обновить пакет CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Эта команда позволяет обновить все установленные в системе пакеты, зависимости которых не были изменены.
> Чтобы обновить только CLI, используйте `apt-get install`.
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Выполите удаление с помощью команды `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Удалите ключ подписывания:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. Удалите все ненужные пакеты:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Дальнейшие действия

Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.

> [!div class="nextstepaction"]
> [Начало работы с Azure CLI](get-started-with-azure-cli.md)
