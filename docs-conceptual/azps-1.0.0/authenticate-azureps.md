---
title: Anmelden mit Azure PowerShell
description: Es wird beschrieben, wie Sie sich mit Azure PowerShell als Benutzer, per Dienstprinzipal oder mit verwalteten Identitäten für Azure-Ressourcen anmelden.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786678"
---
# <a name="sign-in-with-azure-powershell"></a>Anmelden mit Azure PowerShell

Azure PowerShell unterstützt mehrere Authentifizierungsmethoden. Die einfachste Möglichkeit ist die interaktive Anmeldung über die Befehlszeile.

## <a name="sign-in-interactively"></a>Interaktives Anmelden

Verwenden Sie für die interaktive Anmeldung das Cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).

```azurepowershell-interactive
Connect-AzAccount
```

Bei der Ausführung wird von diesem Cmdlet eine Tokenzeichenfolge bereitgestellt. Kopieren Sie diese Zeichenfolge, und fügen Sie sie in einem Browser unter https://microsoft.com/devicelogin ein. Ihre PowerShell-Sitzung wird dann für die Verbindungsherstellung mit Azure authentifiziert. Diese Authentifizierung gilt jeweils für die aktuelle PowerShell-Sitzung.

> [!IMPORTANT]
>
> Ihre Anmeldeinformationen werden in mehreren PowerShell-Sitzungen gemeinsam verwendet, solange Sie angemeldet bleiben.
> Weitere Informationen finden Sie im Artikel zu [beständigen Anmeldeinformationen](context-persistence.md).

## <a name="sign-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind nicht interaktive Azure-Konten. Wie bei anderen Benutzerkonten auch, werden die Berechtigungen mit Azure Active Directory verwaltet. Indem für einen Dienstprinzipal nur die benötigten Berechtigungen gewährt werden, bleibt die Sicherheit Ihrer Automatisierungsskripts gewahrt.

Informationen zur Erstellung eines Dienstprinzipals für die Verwendung mit PowerShell finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure PowerShell](create-azure-service-principal-azureps.md).

Verwenden Sie für die Anmeldung mit einem Dienstprinzipal das Cmdlet `Connect-AzAccount` mit dem Argument `-ServicePrincipal`. Sie benötigen auch die Anwendungs-ID und die Anmeldeinformationen des Dienstprinzipals sowie die dem Dienstprinzipal zugeordnete Mandanten-ID. Verwenden Sie das Cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential), um die Anmeldeinformationen des Dienstprinzipals als entsprechendes Objekt abzurufen. Bei diesem Cmdlet wird eine Eingabeaufforderung für die Benutzer-ID und das Kennwort des Dienstprinzipals angezeigt.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a>Anmelden mit einer verwalteten Azure-Dienstidentität

Verwaltete Identitäten für Azure-Ressourcen ist eine Funktion von Azure Active Directory. Sie können den Dienstprinzipal einer verwalteten Identität für die Anmeldung verwenden und ein App-exklusives Zugriffstoken für den Zugriff auf andere Ressourcen beziehen. Verwaltete Identitäten stehen nur für virtuelle Computer zur Verfügung, die in einer Azure-Cloud ausgeführt werden.

Weitere Informationen zu verwalteten Identitäten für Azure-Ressourcen finden Sie unter [Verwenden von verwalteten Identitäten für Azure-Ressourcen auf einem virtuellen Azure-Computer zum Abrufen eines Zugriffstokens](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a>Anmelden als Cloud Solution Provider (CSP)

Eine Anmeldung als [(Cloud Solution Provider, CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) erfordert die Verwendung von `-TenantId`. In der Regel kann dieser Parameter entweder als Mandanten-ID oder als Domänenname angegeben werden. Für die CSP-Anmeldung muss jedoch eine **Mandanten-ID** bereitgestellt werden.

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>Anmelden bei einer anderen Cloud

Azure-Clouddienste verfügen über Umgebungen, die jeweils mit den regionalen Bestimmungen zum Umgang mit Daten konform sind.
Legen Sie die Umgebung für Konten in einer regionalen Cloud fest, wenn Sie sich mit dem Argument `-Environment` anmelden.
Beispiel für den Fall, dass sich Ihr Konto in der Cloud in China befindet:

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

Mit dem folgenden Befehl wird eine Liste mit den verfügbaren Umgebungen abgerufen:

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Weitere Informationen zum Verwalten des rollenbasierten Zugriffs in Azure

Weitere Informationen zur Authentifizierung und Abonnementverwaltung in Azure finden Sie unter [Verwalten von Konten, Abonnements und Administratorrollen](/azure/active-directory/role-based-access-control-configure).

Azure PowerShell-Cmdlets für die Rollenverwaltung:

* [Get-AzRoleAssignment](/powershell/module/az.Resources/Get-azRoleAssignment)
* [Get-AzRoleDefinition](/powershell/module/az.Resources/Get-azRoleDefinition)
* [New-AzRoleAssignment](/powershell/module/az.Resources/New-azRoleAssignment)
* [New-AzRoleDefinition](/powershell/module/az.Resources/New-azRoleDefinition)
* [Remove-AzRoleAssignment](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [Remove-AzRoleDefinition](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [Set-AzRoleDefinition](/powershell/module/az.Resources/Set-azRoleDefinition)
