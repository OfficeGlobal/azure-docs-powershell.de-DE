---
title: Anmelden mit Azure PowerShell
description: Anmelden mit Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 71a2554052f5a25ea86fe44b6dcf5d9343c81f3e
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/04/2018
ms.locfileid: "47424682"
---
# <a name="log-in-with-azure-powershell"></a>Anmelden mit Azure PowerShell

Azure PowerShell unterstützt mehrere Anmeldemethoden. Die einfachste Möglichkeit ist die interaktive Anmeldung über die Befehlszeile.

## <a name="interactive-log-in"></a>Interaktive Anmeldung

1. Geben Sie `Login-AzureRmAccount`ein. Im daraufhin erscheinenden Dialogfeld werden Sie zur Eingabe Ihrer Azure-Anmeldeinformationen aufgefordert.

2. Geben Sie die dem Konto zugeordnete E-Mail-Adresse und das zugehörige Kennwort ein. Die Anmeldeinformationen werden von Azure authentifiziert und gespeichert, dann wird das Fenster geschlossen.

## <a name="log-in-with-a-service-principal"></a>Anmeldung mit einem Dienstprinzipal

Dienstprinzipale ermöglichen die Erstellung nicht interaktiver Konten für die Ressourcenbearbeitung. Dienstprinzipale sind vergleichbar mit Benutzerkonten, auf die Sie mithilfe von Azure Active Directory Regeln anwenden können. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

1. Falls Sie noch nicht über einen Dienstprinzipal verfügen, [erstellen Sie einen](create-azure-service-principal-azureps.md).

2. Melden Sie sich mit dem Dienstprinzipal an.

    ```powershell
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    Wenn Sie Ihre Mandanten-ID ermitteln möchten, melden Sie sich interaktiv an, und rufen Sie anschließend die Mandanten-ID aus Ihrem Abonnement ab.

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
    ```

### <a name="log-in-using-managed-identities-for-azure-resources"></a>Anmelden mit verwalteten Identitäten für Azure-Ressourcen

Verwaltete Identitäten für Azure-Ressourcen ist eine Funktion von Azure Active Directory. Sie können den Dienstprinzipal einer verwalteten Identität für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen.

Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer zum Abrufen eines Zugriffstokens](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).

## <a name="log-in-to-another-cloud"></a>Anmelden bei einer anderen Cloud

Azure-Clouddienste bieten unterschiedliche Umgebungen, die den Datenverarbeitungsvorschriften verschiedener Staaten entsprechen. Wenn Ihr Azure-Konto in einer dieser staatsspezifischen Clouds enthalten ist, müssen Sie die Umgebung angeben, wenn Sie sich anmelden. Wenn Ihr Konto beispielsweise in der Cloud für China enthalten ist, melden Sie sich mit dem folgenden Befehl an:

```powershell
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

Verwenden Sie den folgenden Befehl, um eine Liste der verfügbaren Umgebungen zu erhalten:

```powershell
Get-AzureRmEnvironment | Select-Object Name
```

```output
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Weitere Informationen zum Verwalten des rollenbasierten Zugriffs in Azure

Weitere Informationen zur Authentifizierung und Abonnementverwaltung in Azure finden Sie unter [Verwalten von Konten, Abonnements und Administratorrollen](/azure/active-directory/role-based-access-control-configure).

Azure PowerShell-Cmdlets für die Rollenverwaltung

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
