---
title: Anmelden mit Azure PowerShell
description: Hier finden Sie Informationen zur Anmeldung mit Azure PowerShell als Benutzer, mit einem Dienstprinzipal oder mit MSI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 20194ac2282d602ba61bf130791edac9f4ffae6c
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110754"
---
# <a name="sign-in-with-azure-powershell"></a>Anmelden mit Azure PowerShell

Azure PowerShell unterstützt mehrere Authentifizierungsmethoden. Die einfachste Möglichkeit ist die interaktive Anmeldung über die Befehlszeile.

## <a name="sign-in-interactively"></a>Interaktives Anmelden

Verwenden Sie für die interaktive Anmeldung das Cmdlet [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount).

```azurepowershell
Connect-AzureRmAccount
```

Wenn Sie dieses Cmdlet ausführen, wird ein Dialogfeld angezeigt, in dem Sie zur Eingabe Ihrer E-Mail-Adresse und Ihres Kennworts für Ihr Azure-Konto aufgefordert werden. Wenn Sie sich authentifizieren, werden diese Angaben für die aktuelle PowerShell-Sitzung gespeichert, das Dialogfeld wird geschlossen, und Sie haben Zugriff auf alle Azure PowerShell-Cmdlets.

> [!IMPORTANT]
> Ab Azure PowerShell 6.3.0 werden Ihre Anmeldeinformationen in mehreren PowerShell-Sitzungen gemeinsam verwendet, solange Sie bei Windows angemeldet bleiben. Weitere Informationen finden Sie im Artikel zu [beständigen Anmeldeinformationen](context-persistence.md).

## <a name="sign-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale ermöglichen die Erstellung nicht interaktiver Konten für die Ressourcenbearbeitung. Dienstprinzipale sind vergleichbar mit Benutzerkonten, auf die Sie mithilfe von Azure Active Directory Regeln anwenden können. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

Informationen zur Erstellung eines Dienstprinzipals für die Verwendung mit PowerShell finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell](create-azure-service-principal-azureps.md).

Verwenden Sie für die Anmeldung mit einem Dienstprinzipal das Cmdlet `Connect-AzureRmAccount` mit dem Argument `-ServicePrincipal`. Sie benötigen auch die Anwendungs-ID und die Anmeldeinformationen des Dienstprinzipals sowie die dem Dienstprinzipal zugeordnete Mandanten-ID. Verwenden Sie das Cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential), um die Anmeldeinformationen des Dienstprinzipals als entsprechendes Objekt abzurufen. Dieses Cmdlet zeigt ein Dialogfeld für die Eingabe der Benutzer-ID und des Kennworts des Dienstprinzipals an.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-vm-managed-service-identity"></a>Anmelden mit einer verwalteten Dienstidentität eines virtuellen Azure-Computers

Die verwaltete Dienstidentität (Managed Service Identity, MSI) ist ein Vorschaufeature für Azure Active Directory. Sie können einen MSI-Dienstprinzipal für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen. MSI steht nur für virtuelle Computer zur Verfügung, die in einer Azure-Cloud ausgeführt werden.

Weitere Informationen zu MSI finden Sie unter [How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition](/azure/active-directory/msi-how-to-get-access-token-using-msi) (Verwenden einer verwalteten Dienstidentität (Managed Service Identity, MSI) eines virtuellen Azure-Computers für Anmeldung und Tokenbezug).

## <a name="sign-in-to-another-cloud"></a>Anmelden bei einer anderen Cloud

Azure-Clouddienste bieten unterschiedliche Umgebungen, die den Datenverarbeitungsvorschriften verschiedener Regionen entsprechen. Wenn sich Ihr Azure-Konto in einer Cloud befindet, die einer dieser Regionen zugeordnet ist, müssen Sie bei der Anmeldung die Umgebung angeben. Wenn Ihr Konto beispielsweise in der Cloud für China enthalten ist, melden Sie sich mit dem folgenden Befehl an:

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

Verwenden Sie den folgenden Befehl, um eine Liste der verfügbaren Umgebungen zu erhalten:

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Weitere Informationen zum Verwalten des rollenbasierten Zugriffs in Azure

Weitere Informationen zur Authentifizierung und Abonnementverwaltung in Azure finden Sie unter [Verwalten von Konten, Abonnements und Administratorrollen](/azure/active-directory/role-based-access-control-configure).

Azure PowerShell-Cmdlets für die Rollenverwaltung:

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
