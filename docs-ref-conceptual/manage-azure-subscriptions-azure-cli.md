---
title: "Manage Azure subscriptions with Azure CLI 2.0 (Управление подписками Azure с помощью Azure CLI 2.0)"
description: "Manage Azure subscriptions with Azure CLI 2.0 on Linux, Mac, or Windows (Управление подписками Azure с помощью Azure CLI 2.0 на платформах Windows, Mac или Linux)."
keywords: "Azure CLI 2.0, Linux, Mac, Windows, OS X, подписка"
author: kamaljit
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 383fb6ebd90ac79f60869187b402d53d4f1791fd
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="78be8-104">Управление несколькими подписками Azure</span><span class="sxs-lookup"><span data-stu-id="78be8-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="78be8-105">Если вы только приступаете к работе с Azure, скорее всего, у вас есть только одна подписка.</span><span class="sxs-lookup"><span data-stu-id="78be8-105">If you are brand new to Azure, you probably only have a single subscription.</span></span>
<span data-ttu-id="78be8-106">Но если вы уже пользуетесь Azure какое-то время, возможно, вы уже успели создать несколько подписок.</span><span class="sxs-lookup"><span data-stu-id="78be8-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span>
<span data-ttu-id="78be8-107">Вы можете настроить Azure CLI 2.0 для выполнения команд, связанных с определенной подпиской.</span><span class="sxs-lookup"><span data-stu-id="78be8-107">If so, you can configure Azure CLI 2.0 to execute commands against a particular subscription.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

1. <span data-ttu-id="78be8-108">Получите список всех подписок в своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="78be8-108">Get a list of all subscriptions in your account.</span></span>

   ```azurecli-interactive
   az account list --output table
   ```

   ```Output
   Name                                         CloudName    SubscriptionId                        State     IsDefault
   -------------------------------------------  -----------  ------------------------------------  --------  -----------
   My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
   My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
   ```

1. <span data-ttu-id="78be8-109">Определите подписку по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78be8-109">Set the default.</span></span>
 
   ```azurecli-interactive
   az account set --subscription "My Demos"
   ```

   > [!NOTE]
   > <span data-ttu-id="78be8-110">Параметр `--subscription` принимает имя подписки или идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="78be8-110">The `--subscription` parameter takes either the subscription name or the subscription ID.</span></span>

<span data-ttu-id="78be8-111">Проверьте изменения, выполнив команду `az account list --output table` еще раз.</span><span class="sxs-lookup"><span data-stu-id="78be8-111">You can verify the change by running the `az account list --output table` command again.</span></span>

<span data-ttu-id="78be8-112">Когда вы определите подписку по умолчанию, все последующие выполняемые команды Azure CLI будут связаны с ней.</span><span class="sxs-lookup"><span data-stu-id="78be8-112">Once you set your default subscription, all subsequent Azure CLI commands run against this subscription.</span></span>