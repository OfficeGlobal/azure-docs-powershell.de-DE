---
title: Verwalten von Azure-Abonnements mit Azure PowerShell | Microsoft-Dokumentation
description: Verwalten von Azure-Abonnements mit Azure PowerShell
keywords: Azure PowerShell, Abonnement
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 00f346c2e90fb6615dd9eac96e13f4cfc243d204
ms.sourcegitcommit: cb1fd248920d7efca67bd6c738a3b47206df7890
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/13/2018
ms.locfileid: "39024476"
---
# <a name="manage-multiple-azure-subscriptions"></a>Verwalten mehrerer Azure-Abonnements

Falls Sie noch keine Erfahrung mit Azure haben, verfügen Sie wahrscheinlich nur über ein einzelnes Abonnement. Wenn Sie Azure hingegen schon eine Weile verwenden, haben Sie möglicherweise bereits mehrere Azure-Abonnements erstellt. Sie können Azure PowerShell so konfigurieren, dass Befehle für ein bestimmtes Abonnement ausgeführt werden.

1. Rufen Sie eine Liste mit allen Abonnements in Ihrem Konto ab.

    ```powershell
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

    ```powershell
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. Überprüfen Sie die Änderung durch Ausführen des Cmdlets `Get-AzureRmContext`.

    ```powershell
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
