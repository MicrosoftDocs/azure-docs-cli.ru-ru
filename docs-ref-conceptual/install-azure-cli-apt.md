---
title: Установка Azure CLI в Linux с помощью apt
description: Как установить Azure CLI с помощью диспетчера пакетов apt
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c33c3e75991979a72a7b82183dd88b87715907ae
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450264"
---
# <a name="install-azure-cli-with-apt"></a>Установка Azure CLI с помощью apt

Если вы используете дистрибутив, включающий `apt`, например Ubuntu ил Debian, доступен 64-разрядный пакет Azure CLI. Этот пакет протестирован со следующими версиями:

* Ubuntu trusty, xenial, artful и bionic
* Debian wheezy, jessie и stretch

## <a name="install"></a>Install

1. <div id="install-step-1"/>Измените список источников.

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/>Получите ключ подписывания Microsoft.

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. Установите интерфейс командной строки.

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > Ключ подписывания обновлен и заменен в мае 2018 г. Если вы получаете сообщения об ошибках подписи, убедитесь, что вы используете [последний ключ подписывания](#signingKey).

Запустите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>Команда lsb_release не возвращает правильную версию базового дистрибутива

Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`. Это значение используется при установке для определения устанавливаемого пакета. Если известно, на основе какой версии создан дистрибутив, можно установить значение параметра `AZ_REPO` вручную на [первом шаге установки](#install-step-1). В противном случае найдите информацию о том, как определить имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.

### <a name="no-package-for-your-distribution"></a>Для вашего дистрибутива отсутствует пакет

Иногда между выпуском дистрибутива Ubuntu и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время. Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей. Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.

Для этого вручную установите значение `AZ_REPO` на [первом шаге установки](#install-step-1). Для дистрибутивов Ubuntu используйте репозиторий `bionic`, а для дистрибутивов Debian используйте репозиторий `stretch`. Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.

### <a name="apt-key-fails-with-no-dirmngr"></a>Команда apt-key завершается сбоем с сообщением "No dirmngr" (Нет диспетчера каталогов)

При выполнении команды `apt-key` может появиться примерно такая ошибка:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

Сбой возникает из-за отсутствия компонента, обязательного для `apt-key`. Ошибку можно устранить, установив пакет `dirmngr`.

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a>Зависает apt-key

Если при использовании брандмауэра блокируются исходящие подключения к порту 11371, команда `apt-key` может перестать работать на неопределенное время.
Ваш брандмауэр может требовать использования прокси-сервера HTTP для исходящих подключений:

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

Чтобы определить, используется ли у вас прокси-сервер, обратитесь к своему системному администратору. Если прокси-сервер не требует входа, не указывайте имя пользователя и пароль.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Блокировка изменений

Используйте `apt-get upgrade`, чтобы обновить пакет CLI.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> Ключ подписывания обновлен и заменен в мае 2018 г. Если вы получаете сообщения об ошибках подписи, убедитесь, что вы используете [последний ключ подписывания](#signingKey).
>
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
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. Удалите все ненужные пакеты:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Дальнейшие действия

Теперь вы можете пользоваться Azure CLI. Просмотрите общие сведения о его возможностях и список распространенных команд.

> [!div class="nextstepaction"]
> [Начало работы с Azure CLI](get-started-with-azure-cli.md)
