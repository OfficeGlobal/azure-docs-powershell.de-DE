---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: c4af07816aaa6713d67e3349a45880f8cc22c80a
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574497"
---
# <a name="install-azure-powershell-with-powershellget"></a>Installieren von Azure PowerShell mit PowerShellGet

In diesem Artikel erfahren Sie, wie Sie mithilfe von „PowerShellGet“ die Azure PowerShell-Module installieren. Für die Vorschauversion von Az werden keine anderen Installationsmethoden unterstützt. 

## <a name="requirements"></a>Requirements (Anforderungen)

Azure PowerShell kann mit PowerShell 5.x unter Windows und mit PowerShell 6.x auf einer beliebigen Plattform verwendet werden. Führen Sie den folgenden Befehl aus, um die Version von PowerShell zu prüfen, die auf Ihrem Computer ausgeführt wird:

```powershell-interactive
$PSVersionTable.PSVersion
```

Falls Sie eine veraltete Version verwenden oder PowerShell installieren müssen, lesen Sie den Artikel [Installieren verschiedener Versionen von PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6). Auf dieser Seite finden Sie einen Link zu den Installationsinformationen für Ihre Plattform.

## <a name="install-the-azure-powershell-module"></a>Installieren des Azure PowerShell-Moduls

> [!IMPORTANT]
>
> Die Module `AzureRM` und `Az` dürfen nicht gleichzeitig auf einem System installiert sein. Um das Modul `Az` installieren zu können, muss `AzureRM` deinstalliert werden. Eine entsprechende Anleitung finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md) (AzureRM).

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

Das Modul `Az` ist ein Rollupmodul für die Azure PowerShell-Cmdlets. Wenn Sie es installieren, werden alle verfügbaren Azure Resource Manager-Module heruntergeladen und die zugehörigen Cmdlets für die Nutzung zur Verfügung gestellt.

## <a name="sign-in"></a>Anmelden

Damit Sie Azure PowerShell verwenden können, müssen Sie `Az` mit dem [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module)-Cmdlet in Ihre aktuelle PowerShell-Sitzung laden und sich dann mit Ihren Azure-Anmeldeinformationen anmelden.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

Sie müssen diese Schritte für jede neue PowerShell-Sitzung wiederholen, die Sie starten. Für den automatischen Import des Moduls `Az` muss ein PowerShell-Profil eingerichtet werden. Informationen hierzu finden Sie unter [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles) (Informationen zu Profilen).
Informationen zum sitzungsübergreifenden Speichern der Azure-Anmeldung finden Sie unter [Persisting user credentials across PowerShell sessions](context-persistence.md) (Speichern von Benutzeranmeldeinformationen zwischen PowerShell-Sitzungen).

## <a name="update-the-azure-powershell-module"></a>Aktualisieren des Azure PowerShell-Moduls

Sie können Ihre Azure PowerShell-Installation aktualisieren, indem Sie [Update-Module](/powershell/module/powershellget/update-module) ausführen. Mit diesem Befehl werden __keine__ früheren Versionen deinstalliert.

```powershell-interactive
Update-Module -Name Az
```

Wenn Sie ältere Versionen von Azure PowerShell von Ihrem System entfernen möchten, helfen Ihnen die Informationen unter [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md) (Deinstallieren des Azure PowerShell-Moduls) weiter.

## <a name="use-multiple-versions-of-azure-powershell"></a>Verwenden von mehreren Versionen von Azure PowerShell

Es ist möglich, mehr als eine Version von Azure PowerShell zu installieren. Verwenden Sie den folgenden Befehl zum Überprüfen, ob Sie mehrere Versionen von Azure PowerShell installiert haben:

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

Anweisungen zum Entfernen einer Version von Azure PowerShell finden Sie unter [Deinstallieren des Azure PowerShell-Moduls](uninstall-azurerm-ps.md).

Wenn Sie eine bestimmte Version des `Az`-Moduls laden möchten, verwenden Sie das Argument `-RequiredVersion` mit `Install-Module` oder `Import-Module`:

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

Sind mehrere Versionen des Moduls installiert, wird beim Importieren standardmäßig die neueste Version geladen.

## <a name="provide-feedback"></a>Feedback geben

[Melden Sie auf GitHub ein Problem](https://github.com/Azure/azure-powershell/issues), wenn Sie bei der Nutzung von Azure PowerShell einen Fehler finden.
Verwenden Sie das [Send-Feedback](/powershell/module/az.profile/send-feedback)-Cmdlet, um über die Befehlszeile Feedback zu senden.

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zum Modul und zu den zugehörigen Features als Einstieg in die Nutzung von Azure PowerShell finden Sie unter [Get started with Azure PowerShell](get-started-azureps.md) (Erste Schritte mit Azure PowerShell).