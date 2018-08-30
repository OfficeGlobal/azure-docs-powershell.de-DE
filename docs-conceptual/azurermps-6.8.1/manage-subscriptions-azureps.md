---
title: Verwalten von Azure-Abonnements mit Azure PowerShell
description: Verwalten von Azure-Abonnements mit Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: e1606ddb02adf1de2cb5496917d61755ac3dad23
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250554"
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

Nachdem Sie Ihr Standardabonnement festgelegt haben, werden alle weiteren Azure PowerShell-Befehle für dieses Abonnement ausgeführt.
