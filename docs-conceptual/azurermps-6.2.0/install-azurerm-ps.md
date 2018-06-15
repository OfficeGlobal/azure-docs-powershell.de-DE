---
title: Installieren von Azure PowerShell mit PowerShellGet
description: Anleitung für die Installation von Azure PowerShell mit PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323100"
---
# <a name="install-azure-powershell-with-powershellget"></a>Installieren von Azure PowerShell mit PowerShellGet

In diesem Artikel erfahren Sie, wie Sie die Azure PowerShell-Module in einer Windows-Umgebung unter Verwendung von PowerShellGet installieren.  Dies ist die bevorzugte Installationsmethode für Azure PowerShell. Sie können aber auch den Webplattform-Installer oder das MSI-Paket verwenden. Entsprechende Informationen finden Sie unter [Andere Installationsmethoden](other-install.md).

Wenn Sie Azure PowerShell unter macOS oder Linux verwenden möchten, lesen Sie den folgenden Artikel: [Installieren und Konfigurieren von Azure PowerShell unter macOS und Linux](install-azurermps-maclinux.md).

## <a name="system-requirements"></a>Systemanforderungen

Für die Azure PowerShell-Version 6.1.0 wird mindestens die Version 5.0 von PowerShell benötigt. Informationen zum Upgraden auf PowerShell 5.0 finden Sie unter [Aktualisieren einer vorhandenen Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).

PowerShellGet ist automatisch in PowerShell 5.0 enthalten.

## <a name="install-or-update-the-azure-powershell-module"></a>Installieren oder Aktualisieren des Azure PowerShell-Moduls

Für die Installation von Azure PowerShell aus dem PowerShell-Katalog sind erhöhte Rechte erforderlich. Führen Sie den folgenden Befehl in einer PowerShell-Sitzung mit erhöhten Rechten aus:

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> Mit diesem Befehl werden alle vorhandenen Installationen von Azure PowerShell in Ihrem System aktualisiert. Sollten Sie mehrere installierte Versionen benötigen, sehen Sie sich die Antwort auf die häufig gestellte Frage [Kann ich mehrere Versionen von Azure PowerShell installieren?](#multiple-versions) an.

Standardmäßig ist der PowerShell-Katalog nicht als vertrauenswürdiges Repository für PowerShellGet konfiguriert. Bei der ersten Verwendung des PowerShell-Katalogs wird die folgende Meldung angezeigt:

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Antworten Sie mit „Ja“ oder „Ja zu allen“, um die Installation fortzusetzen.

> [!NOTE]
> Wenn Sie eine ältere NuGet-Version als 2.8.5.201 haben, werden Sie aufgefordert, die aktuelle NuGet-Version herunterzuladen und zu installieren.

Das AzureRM-Modul ist ein Rollupmodul für die Azure Resource Manager-Cmdlets. Bei der Installation des AzureRM-Moduls werden alle noch nicht installierten Azure PowerShell-Module aus dem PowerShell-Katalog heruntergeladen.

## <a name="load-the-azure-powershell-module"></a>Laden des Azure PowerShell-Moduls

Nach der Installation des Moduls müssen Sie das Modul in der PowerShell-Sitzung laden. Dies muss in einer normalen PowerShell-Sitzung (ohne erhöhte Rechte) erfolgen. Module werden wie folgt mit dem Cmdlet `Import-Module` geladen:

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a>Melden von Problemen und Bereitstellen von Feedback

Sollten bei Ihnen Probleme mit dem Tool auftreten, können Sie [hier](https://github.com/Azure/azure-powershell/issues) ein Problem auf GitHub melden. Zum Senden von Feedback zur Befehlszeile verwenden Sie das Cmdlet `Send-Feedback`.

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen zur Verwendung von Azure PowerShell finden Sie in den folgenden Artikeln:

* [Erste Schritte mit Azure PowerShell](get-started-azureps.md)

## <a name="frequently-asked-questions"></a>Häufig gestellte Fragen

### <a id="helpmechoose"></a>Wie überprüfe ich die Version von Azure PowerShell?

Obwohl empfohlen wird, möglichst bald ein Upgrade auf die neueste Version auszuführen, werden verschiedene Azure PowerShell-Versionen unterstützt. Führen Sie zum Ermitteln der installierten Azure PowerShell-Version `Get-Module AzureRM` in der Befehlszeile aus:

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a>Kann ich Azure PowerShell für klassische Azure-Bereitstellungen verwenden?

Bei Bereitstellungen mit dem klassischen Bereitstellungsmodell können Sie die Dienstverwaltungsversion von Azure PowerShell installieren. Weitere Informationen finden Sie unter [Installing the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps) (Installieren des Azure PowerShell-Dienstverwaltungsmoduls). Das Azure- und das AzureRM-Modul nutzen gemeinsame Abhängigkeiten. Wenn Sie sowohl die Azure- als auch die AzureRM-Module verwenden, müssen Sie die gleiche Version der einzelnen Pakete installieren.

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><a name="multiple-versions"/>Kann ich mehrere Versionen von Azure PowerShell installieren?

PowerShellGet ist die einzige Installationsmethode, die mehrere Versionen unterstützt. Wenn Sie mehrere Versionen installieren möchten, können Sie dem Cmdlet `Install-Module` den Parameter `-RequiredVersion` hinzufügen. Beispiel für die Installation der Versionen 6.1.0 und 1.2.9:

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

Nur eine Version des Moduls kann in einer PowerShell-Sitzung geladen werden. Sie müssen ein neues PowerShell-Fenster öffnen und `Import-Module` verwenden, um eine bestimmte Version des Azure PowerShell-Moduls zu importieren.

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> Version 2.1.0 und Version 1.2.6 sind die ersten Modulversionen, die parallel installiert und genutzt werden können. Beim Laden einer früheren Version von Azure PowerShell werden inkompatible Versionen des **AzureRM.Profile**-Moduls geladen. Dies führt dazu, dass Sie, immer wenn Sie ein Cmdlet ausführen, zum Anmelden aufgefordert werden.
