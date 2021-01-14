---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 31b6a6e1c4c987ea351ccebc5d5bf23313ed856f
ms.sourcegitcommit: 547d3db8a1469f11d33e738a82d96cb51de61bd6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "98147468"
---
## <a name="overview"></a>Обзор

Диспетчер пакетов `apt` содержит пакет x86_64 для Azure CLI, протестированный в следующих дистрибутивах.

| Distribution | Версия |
|:-------------|:--------|
| Ubuntu       | 14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla) |
| Debian       | Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster) |

> [!WARNING]
> Для Ubuntu 20.04 (Focal Fossa) и 20.10 (Groovy Gorilla) доступен пакет `azure-cli` с версией `2.0.81`, предоставляемый репозиторием `universe`. Этот пакет устарел и не рекомендуется к использованию. Если этот пакет установлен, удалите его, прежде чем продолжать работу, выполнив команду `sudo apt remove azure-cli -y && sudo apt autoremove -y`.

## <a name="installation-options"></a>Варианты установки

Есть два варианта установки Azure CLI в системе.  Во-первых, вы можете выполнить одну команду, которая скачает скрипт установки и выполнит команды установки.  Или же вы можете выполнить пошаговый процесс установки самостоятельно.  Оба метода описаны ниже.

## <a name="option-1-install-with-one-command"></a>Вариант 1. Установка с помощью одной команды

Команда Azure CLI предоставляет скрипт для выполнения всех команд установки за один шаг.  Этот скрипт скачивается с помощью `curl` и передается непосредственно в `bash` для установки CLI.

Если вы хотите проверить содержимое скрипта перед выполнением, просто скачайте скрипт с помощью `curl` и откройте его в любом текстовом редакторе.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a>Вариант 2. Пошаговые инструкции по установке

Если вы предпочитаете пошаговый процесс установки, выполните следующие действия, чтобы установить Azure CLI.

1. Получение пакетов, необходимых для процесса установки:

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. Скачайте и установите ключ подписывания (Майкрософт):

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/>Добавьте репозиторий программного обеспечения Azure CLI (пропустите этот шаг для дистрибутивов Linux ARM64):

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Обновите сведения о репозитории и установите пакет `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a>Вход с помощью Azure CLI

Обновите Azure CLI с помощью команды `az`. Чтобы войти, используйте команду [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](interactive-login.md)]

Дополнительные сведения о различных методах проверки подлинности см. в статье [Вход с помощью Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Устранение неполадок

Ниже описаны некоторые распространенные проблемы при установке с помощью `apt`. Если у вас возникла проблема, не описанная здесь, [сообщите об этом на сайте GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a>Проблема с отсутствием модуля в Ubuntu 20.04 (Focal)/WSL

Если вы установили `azure-cli` в выпуске `Focal`, не добавив репозиторий программного обеспечения Azure CLI, как предписывает [шаг 3](#set-release) инструкций по установке вручную, или с помощью нашего [скрипта](#option-1-install-with-one-command), могут возникнуть проблемы, например с отсутствием модуля с именем decorator или antlr4, так как установленный вами пакет является устаревшим пакетом `azure-cli 2.0.81` из репозитория `focal/universe`. Сначала удалите его с помощью команды `sudo apt remove azure-cli -y && sudo apt autoremove -y`, а затем выполните приведенные выше [инструкции](#install), чтобы установить последнюю версию пакета `azure-cli`.

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a>Команда lsb_release не возвращает правильную версию базового дистрибутива

Некоторые производные от Ubuntu или Debian дистрибутивы, например Linux Mint, могут возвращать неправильную версию при использовании команды `lsb_release`. Это значение используется при установке для определения устанавливаемого пакета. Если вы знаете кодовое имя версии Ubuntu или Debian, на основе которой создан ваш дистрибутив, можно установить значение параметра `AZ_REPO` вручную при [добавлении репозитория](#set-release). В противном случае найдите информацию о том, как определить кодовое имя основного дистрибутива, и задайте для `AZ_REPO` правильное значение.

### <a name="no-package-for-your-distribution"></a>Для вашего дистрибутива отсутствует пакет

Иногда между выпуском дистрибутива и выпуском пакета Azure CLI для этого дистрибутива может пройти некоторое время. Azure CLI использует минимально возможный набор зависимостей и разработан таким образом, чтобы свести к минимуму вероятность нарушения работы при обновлении зависимостей. Если для вашего базового дистрибутива отсутствует пакет, попробуйте установить пакет для более ранней версии дистрибутива.

Для этого вручную установите значение `AZ_REPO` при [добавлении репозитория](#set-release). Для дистрибутивов Ubuntu используйте репозиторий `bionic`, а для дистрибутивов Debian используйте репозиторий `stretch`. Более ранние версии дистрибутивов, чем Ubuntu Trusty и Debian Wheezy, не поддерживаются.

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a>В Elementary OS (EOS) не удалось установить Azure CLI

В EOS не удалось установить Azure CLI, так как `lsb_release` возвращает `HERA`, то есть имя выпуска EOS.  Чтобы устранить проблему, нужно исправить файл `/etc/apt/sources.list.d/azure-cli.list` и изменить `hera main` на `bionic main`.

Исходное содержимое файла:

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

Измененное содержимое файла:

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a>Прокси-сервер блокирует подключения

[!INCLUDE[configure-proxy](configure-proxy.md)]

Вы также можете явным образом настроить `apt`, чтобы использовать этот прокси-сервер все время. Убедитесь, что следующие строки отображаются в файле конфигурации `apt` в `/etc/apt/apt.conf.d/`. Мы рекомендуем использовать существующий файл глобальной конфигурации или существующий файл конфигурации прокси-сервера (`40proxies` или `99local`), но вам следует учитывать требования системного администратора.

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

Если прокси-сервер не использует обычную аутентификацию, __удалите__ часть `[username]:[password]@` URI прокси-сервера. См. подробнее о конфигурации прокси-сервера в официальной документации по Ubuntu:

* [apt.conf manpage](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [Вики-сайт, посвященный Ubuntu (справочник по команде apt-get)](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

Чтобы вы могли получить ключ подписывания (Майкрософт) и получить пакет из нашего репозитория, ваш прокси-сервер должен разрешать HTTPS-подключения по следующему адресу:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Update
[!INCLUDE [az-upgrade](az-upgrade.md)]

Вы также можете обновить пакет CLI с помощью команды `apt-get upgrade`.

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

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Выполите удаление с помощью команды `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Если вы не планируете переустанавливать CLI, удалите сведения о репозитории Azure CLI:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Если вы не используете другие пакеты от корпорации Майкрософт, удалите ключ подписывания.

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. Удалите все ненужные пакеты:

   ```bash
   sudo apt autoremove
   ```
