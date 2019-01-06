---
title: Verwalten von Azure-Abonnements mit Azure PowerShell
description: Verwalten von Azure-Abonnements mit Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 41cf9b06f736f22eb3c2a9e2fbe1f047534cc09d
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594751"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="83dbc-103">Verwalten mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="83dbc-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="83dbc-104">Falls Sie noch keine Erfahrung mit Azure haben, verfügen Sie wahrscheinlich nur über ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="83dbc-104">If you're brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="83dbc-105">Wenn Sie Azure hingegen schon eine Weile verwenden, haben Sie möglicherweise bereits mehrere Azure-Abonnements erstellt.</span><span class="sxs-lookup"><span data-stu-id="83dbc-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="83dbc-106">Sie können Azure PowerShell so konfigurieren, dass Befehle für ein bestimmtes Abonnement ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="83dbc-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="83dbc-107">Rufen Sie eine Liste mit allen Abonnements in Ihrem Konto ab.</span><span class="sxs-lookup"><span data-stu-id="83dbc-107">Get a list of all subscriptions in your account.</span></span>

    ```azurepowershell-interactive
    Get-AzSubscription
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

2. <span data-ttu-id="83dbc-108">Legen Sie das Standardabonnement fest.</span><span class="sxs-lookup"><span data-stu-id="83dbc-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzSubscription -Subscription "My Demos"
    ```

3. <span data-ttu-id="83dbc-109">Überprüfen Sie die Änderung durch Ausführen des Cmdlets `Get-AzContext`.</span><span class="sxs-lookup"><span data-stu-id="83dbc-109">Verify the change by running the `Get-AzContext` cmdlet.</span></span>

    ```azurepowershell-interactive
    Get-AzContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="83dbc-110">Nachdem Sie Ihr Standardabonnement festgelegt haben, werden alle Azure PowerShell-Befehle für dieses Abonnement ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="83dbc-110">Once you set your default subscription, all Azure PowerShell commands run against this subscription.</span></span>