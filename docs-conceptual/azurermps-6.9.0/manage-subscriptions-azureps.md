---
title: Verwalten von Azure-Abonnements mit Azure PowerShell
description: Verwalten von Azure-Abonnements mit Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 3f1c1bab5f9903ee7df813bf1ef043c7107ebe79
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425362"
---
# <a name="manage-multiple-azure-subscriptions"></a>Verwalten mehrerer Azure-Abonnements

Falls Sie noch keine Erfahrung mit Azure haben, verfügen Sie wahrscheinlich nur über ein einzelnes Abonnement. Wenn Sie Azure hingegen schon eine Weile verwenden, haben Sie möglicherweise bereits mehrere Azure-Abonnements erstellt. Sie können Azure PowerShell so konfigurieren, dass Befehle für ein bestimmtes Abonnement ausgeführt werden.

1. Rufen Sie eine Liste mit allen Abonnements in Ihrem Konto ab.

    ```azurepowershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. Legen Sie das Standardabonnement fest.

    ```azurepowershell-interactive
    Select-AzureRmSubscription -Subscription "My Demos"
    ```

3. Überprüfen Sie die Änderung durch Ausführen des Cmdlets `Get-AzureRmContext`.

    ```azurepowershell-interactive
    Get-AzureRmContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

Nachdem Sie Ihr Standardabonnement festgelegt haben, werden alle Azure PowerShell-Befehle für dieses Abonnement ausgeführt.
