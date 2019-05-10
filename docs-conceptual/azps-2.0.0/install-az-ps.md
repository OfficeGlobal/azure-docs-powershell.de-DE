---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 269119333b2197a15ed7bb50e3e5d90588456174
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048545"
---
# <a name="install-the-azure-powershell-module"></a>Installieren des Azure PowerShell-Moduls

In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren. Diese Anweisungen können für Windows-, macOS- und Linux-Plattformen verwendet werden. Für das Az-Modul werden derzeit keine anderen Installationsmethoden unterstützt.

## <a name="requirements"></a>Requirements (Anforderungen)

Azure PowerShell kann mit PowerShell 5.1 oder höher unter Windows oder mit PowerShell 6 auf einer beliebigen Plattform verwendet werden.
Führen Sie den Befehl aus, um Ihre PowerShell-Version zu überprüfen:

```powershell-interactive
$PSVersionTable.PSVersion
```

Falls Sie eine veraltete Version verwenden oder PowerShell installieren müssen, lesen Sie den Artikel [Installieren verschiedener Versionen von PowerShell](/powershell/scripting/setup/installing-powershell). Auf dieser Seite finden Sie einen Link zu den Installationsinformationen für Ihre Plattform.

Wenn Sie PowerShell 5 unter Windows verwenden, muss auch .NET Framework 4.7.2 installiert sein. Eine Anleitung zur Aktualisierung oder Installation einer neuen Version von .NET Framework finden Sie im [.NET Framework-Installationsleitfaden](/dotnet/framework/install).

## <a name="install-the-azure-powershell-module"></a>Installieren des Azure PowerShell-Moduls

> [!IMPORTANT]
>
> Die Module AzureRM und Az können gleichzeitig installiert sein. Wenn Sie beide Module installiert haben, __aktivieren Sie keine Aliase__.
> Die Aktivierung von Aliasen verursacht Konflikte zwischen AzureRM-Cmdlets und Az-Befehlsaliasen und kann zu unerwartetem Verhalten führen.
> Es wird empfohlen, AzureRM vor der Installation des Az-Moduls zu deinstallieren. Sie können AzureRM jederzeit deinstallieren bzw. Aliase aktivieren. Weitere Informationen zu den AzureRM-Befehlsaliasen finden Sie unter [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).
> Eine Anleitung zur Deinstallation finden Sie unter [Deinstallieren des AzureRM-Moduls](uninstall-az-ps.md#uninstall-the-azurerm-module). 

Für die globale Installation von Modulen benötigen Sie erhöhte Rechte, um Module aus dem PowerShell-Katalog installieren zu können. Führen Sie zum Installieren von Azure PowerShell den folgenden Befehl in einer Sitzung mit erhöhten Rechten aus („Als Administrator ausführen“ unter Windows oder mit Superuser-Berechtigungen unter macOS/Linux):

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

Sollten Sie über keine Administratorrechte verfügen, können Sie die Installation für den aktuellen Benutzer durch Hinzufügen des Arguments `-Scope` ausführen.

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert. Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Antworten Sie mit `Yes` oder `Yes to All`, um die Installation fortzusetzen.

Das Az-Modul ist ein Rollupmodul für die Azure PowerShell-Cmdlets. Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.

## <a name="sign-in"></a>Anmelden

Melden Sie sich mit Ihren Azure-Anmeldeinformationen an, um Azure PowerShell zu verwenden.

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> Wenn Sie das automatische Laden von Modulen deaktiviert haben, müssen Sie das Modul manuell mit `Import-Module Az` importieren. Aufgrund der Modulstruktur kann dieser Vorgang einige Sekunden dauern.

Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten. Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung in PowerShell finden Sie unter [Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen](context-persistence.md).

## <a name="update-the-azure-powershell-module"></a>Aktualisieren des Azure PowerShell-Moduls

Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen. Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.

```powershell-interactive
Update-Module -Name Az
```

Wenn Sie frühere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-az-ps.md) weiter.

## <a name="use-multiple-versions-of-azure-powershell"></a>Verwenden von mehreren Versionen von Azure PowerShell

Es ist möglich, mehr als eine Version von Azure PowerShell zu installieren. Verwenden Sie den folgenden Befehl zum Überprüfen, ob Sie mehrere Versionen von Azure PowerShell installiert haben:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

Anweisungen zum Entfernen einer Version von Azure PowerShell finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-az-ps.md).

Wenn Sie eine bestimmte Version des `Az`-Moduls installieren oder laden möchten, können Sie das Argument `-RequiredVersion` verwenden:

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

Sind mehrere Versionen des Moduls installiert, wird mit der Funktion zum automatischen Laden von Modulen und mit `Import-Module` standardmäßig die neueste Version geladen.

## <a name="provide-feedback"></a>Feedback geben

[Melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie in Azure PowerShell einen Fehler finden.
Verwenden Sie das [Send-Feedback](/powershell/module/az.accounts/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zu Azure PowerShell-Modulen und den zugehörigen Features finden Sie unter [Erste Schritte mit Azure PowerShell](get-started-azureps.md).
Falls Sie mit Azure PowerShell vertraut sind und die Migration aus AzureRM durchführen möchten, hilft Ihnen der Artikel [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md) weiter.
