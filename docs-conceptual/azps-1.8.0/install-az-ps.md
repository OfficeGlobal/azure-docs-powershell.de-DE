---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: d99265c7f156622d876d700106e2b06dd729e8b8
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365743"
---
# <a name="install-the-azure-powershell-module"></a>Installieren des Azure PowerShell-Moduls

In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren. Diese Anweisungen können für Windows-, macOS- und Linux-Plattformen verwendet werden. Für das Az-Modul werden derzeit keine anderen Installationsmethoden unterstützt.

## <a name="requirements"></a>Requirements (Anforderungen)

Azure PowerShell kann mit PowerShell 5.1 oder höher unter Windows oder mit PowerShell Core 6.x und höher auf allen Plattformen verwendet werden. Wenn Sie sich nicht sicher sind, ob Sie über PowerShell verfügen oder unter MacOS oder Linux arbeiten, [installieren Sie die neueste Version von PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).

Führen Sie den Befehl aus, um Ihre PowerShell-Version zu überprüfen:

```powershell-interactive
$PSVersionTable.PSVersion
```

So führen Sie Azure PowerShell in PowerShell 5.1 unter Windows aus

1. Führen Sie bei Bedarf ein Update auf [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) aus. Unter Windows 10 ist PowerShell 5.1 bereits installiert.
2. Installieren Sie [.NET Framework 4.7.2 oder höher](/dotnet/framework/install).

Bei Verwendung von PowerShell Core gibt es keine zusätzlichen Anforderungen an Azure PowerShell.

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

Aufgrund der Art und Weise, wie das Az-Modul gepackt ist, aktualisiert der Befehl [Update-Module](/powershell/module/powershellget/update-module) Ihre Installation nicht ordnungsgemäß. Az ist technisch gesehen ein Metamodul, das alle Untermodule umfasst, die Cmdlets zur Interaktion mit Azure-Diensten enthalten. Das bedeutet, dass zum Aktualisieren des Azure PowerShell-Moduls eine __Neuinstallation__ und keine __Aktualisierung__ erforderlich ist. Dies erfolgt auf dieselbe Weise wie bei der Installation, aber Sie müssen möglicherweise das Argument `-Force` hinzufügen:

```powershell
Install-Module -Name Az -AllowClobber -Force
```

Obwohl dadurch installierte Module überschrieben werden können, verbleiben möglicherweise noch ältere Versionen auf Ihrem System.
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
