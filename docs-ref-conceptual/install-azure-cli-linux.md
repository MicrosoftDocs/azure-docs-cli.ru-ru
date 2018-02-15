---
title: "Установка Azure CLI 2.0 для Linux вручную"
description: "Как установить Azure CLI 2.0 в Linux вручную"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 4ab1f70308810e045b9a1d923fd809ad9848f6c6
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Установка Azure CLI 2.0 в Linux вручную

Если в вашем диспетчере пакетов нет доступного пакета для Azure CLI, вы всегда можете установить CLI вручную, запустив скрипт установки.

> [!NOTE]
> Настоятельно рекомендуем использовать для CLI диспетчер пакетов. Диспетчер пакетов гарантирует, что вы получите последние обновления, и обеспечит стабильность компонентов CLI. Перед установкой вручную проверьте, есть ли пакет для вашего дистрибутива.

## <a name="prerequisites"></a>предварительным требованиям

Для установки CLI в системе должно быть следующее программное обеспечение:

* [Python 2.7 или Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Установка или обновление

При установке или обновлении CLI необходимо выполнить полную установку. При наличии необходимых компонентов установите CLI, выполнив команду `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Либо же вы можете скачать скрипт и запустить его локально. Чтобы изменения вступили в силу, может потребоваться перезапустить оболочку. Когда установка будет завершена, запустите CLI с помощью команды `az`.

## <a name="troubleshooting"></a>Устранение неполадок

Ниже указаны некоторые распространенные проблемы, возникающие при установке вручную. Если ваш случай не описан в этом разделе, сообщите о проблеме на [сайте GitHub](https://github.com/Azure/azure-cli/issues).
### <a name="curl-object-moved-error"></a>Ошибка "Объект перемещен" при выполнении команды curl

Если при выполнении команды `curl` появляется сообщение об ошибке относительно параметра `-L` или сообщение об ошибке "Объект перемещен", попробуйте использовать полный URL-адрес вместо URL-адреса перенаправления `aka.ms`:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Команда `az` не найдена

Если не удается выполнить эту команду после установки и используется `bash` или `zsh`, очистите кэш хэша команд в оболочке. Выполнить

```bash
hash -r
```

и проверьте, будет ли устранена проблема.

Кроме того, проблема может возникнуть, если вы не перезапустили оболочку после установки. Убедитесь, что команда `az` добавлена в переменную `$PATH`. Расположение команды `az`:

```bash
<install path>/bin
```

## <a name="uninstall"></a>Удаление

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Удалите CLI, удалив файлы непосредственно из расположения, выбранного при установке. Расположение установки по умолчанию — `$HOME`.

1. Удалите установленные файлы CLI.

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. Измените файл `$HOME/.bash_profile`, чтобы удалить следующую строку:

  ```
  <install location>/lib/azure-cli/az.completion
  ```

3. При использовании `bash` или `zsh` перезагрузите кэш команд в оболочке.

  ```bash
  hash -r
  ```
