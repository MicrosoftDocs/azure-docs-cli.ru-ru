---
title: "Установка Azure CLI 2.0 для Linux вручную"
description: "Как установить Azure CLI 2.0 в Linux вручную"
keywords: Azure CLI,Install Azure CLI,azure linux, azure install linux
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: cf1405cae70762146f63bc6629edc0dd1d949fff
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Установка Azure CLI 2.0 в Linux вручную

Если в вашем диспетчере пакетов нет доступного пакета для Azure CLI, вы всегда можете установить CLI вручную, запустив скрипт установки. Установка с помощью доступного пакета является рекомендуемым способом.

## <a name="prerequisites"></a>Предварительные требования

Для установки CLI в системе должно быть следующее программное обеспечение:

* [Python 2.7 или Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update-manually"></a>Установка или обновление вручную

При установке или обновлении CLI необходимо выполнить полную установку. При наличии необходимых компонентов установите CLI, выполнив команду `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

При необходимости (или если вы не можете выполнить `curl` в системе) можно скачать скрипт и запустить его локально. Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку. Когда установка будет завершена, запустите CLI с помощью команды `az`.

## <a name="troubleshooting"></a>Устранение неполадок

### <a name="curl-object-moved-error"></a>Ошибка "Объект перемещен" при выполнении команды curl

Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Команда `az` не найдена

Если вы не можете выполнить эту команду после установки, может потребоваться очистить кэш хэша команд в оболочке. Выполнить

```bash
hash -r
```

и посмотрите, будет ли устранена проблема.

Это также может произойти, если вы не перезапустили оболочку после установки. Убедитесь, что команда `az` добавлена в переменную `$PATH`.

Если вы запустили сценарий установки, результат будет таким:

```bash
<install path>/bin
```

## <a name="unstinall-manually"></a>Удаление вручную

Нам будет очень жаль, если вы решите удалить Azure CLI. Перед удалением воспользуйтесь командой `az feedback`, чтобы оставить отзыв с описанием причин вашего решения и предложениями того, как мы могли бы улучшить этот продукт. Мы хотим убедиться, что Azure CLI не содержит ошибок и удобен в использовании. Вы также можете [отправить описание проблемы на GitHub](https://github.com/Azure/azure-cli/issues).

CLI можно удалить, удалив файлы непосредственно из расположения установки. Если используется скрипт `https://aka.ms/InstallAzureCLI`, расположение установки следует выбрать во время установки. Расположение установки по умолчанию — `$HOME`.

Во-первых, удалите установленные файлы CLI:

```bash
rm -r <install location>/lib/azure-cli
rm <install location>/bin/az
```

Затем измените файл `$HOME/.bash_profile`, чтобы удалить строку:

```
<install location>/lib/azure-cli/az.completion
```

И, наконец, перезагрузите кэш команд в оболочке (если он используется). Пользователям `bash` и `zsh` необходимо выполнить этот шаг:

```bash
hash -r
```
