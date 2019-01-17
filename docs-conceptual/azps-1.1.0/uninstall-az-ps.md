---
title: Deinstallieren von Azure PowerShell
description: Anleitung zum vollständigen Deinstallieren von Azure PowerShell
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 9d1f1b6550c39b8c65662cf0150f477392747708
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342053"
---
# <a name="uninstall-the-azure-powershell-module"></a>Deinstallieren des Azure PowerShell-Moduls

In diesem Artikel erfahren Sie, wie Sie eine ältere Version von Azure PowerShell deinstallieren bzw. vollständig vom System entfernen. Verwenden Sie das [Send-Feedback](/powershell/module/az.accounts/send-feedback)-Cmdlet, um uns Feedback zu senden, falls Sie Azure PowerShell vollständig deinstallieren möchten.
Sollte ein Fehler auftreten, können Sie ein [GitHub-Problem melden](https://github.com/azure/azure-powershell/issues).

## <a name="uninstall-the-az-module"></a>Deinstallieren des Az-Moduls

Verwenden Sie zum Deinstallieren der Az-Module das Cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module). Mit `Uninstall-Module` wird jedoch nur ein Modul deinstalliert. Wenn Sie Azure PowerShell vollständig entfernen möchten, müssen Sie die Module einzeln deinstallieren. Die Deinstallation kann kompliziert sein, wenn Sie mehrere Versionen von Azure PowerShell installiert haben.

Überprüfen Sie mit dem folgenden Befehl, welche Versionen von Azure PowerShell derzeit installiert sind:

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
0.7.0               Az                             PSGallery            Azure Resource Manager Module
1.0.0               Az                             PSGallery            Azure Resource Manager Module
```

Das folgende Skript fragt den PowerShell-Katalog ab, um eine Liste mit den abhängigen Submodulen abzurufen. Anschließend wird mit dem Skript die richtige Version der einzelnen Submodule deinstalliert. Sie benötigen Administratorzugriff, um dieses Skript in einem anderen Bereich als `Process` oder `CurrentUser` auszuführen.

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force,

    [switch]$WhatIf
  )
  
  $AllModules = @()
  
  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    if ($_.requiredVersion) {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall" -f $_.name,$version)
      }
    }
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}...' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop -WhatIf:$WhatIf
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

Kopieren Sie zum Verwenden dieser Funktion den Code, und fügen Sie ihn in Ihre PowerShell-Sitzung ein. Das folgende Beispiel zeigt, wie Sie die Funktion ausführen, um eine ältere Version von Azure PowerShell zu entfernen.

```powershell-interactive
Uninstall-AllModules -TargetModule Az -Version 0.7.0 -Force
```

Bei der Ausführung des Skripts werden jeweils der Name und die Version des Submoduls angezeigt, das gerade deinstalliert wird. Wenn Sie das Skript nur ausführen möchten, um zu ermitteln, welche Elemente gelöscht werden, ohne sie jedoch tatsächlich zu löschen, verwenden Sie die Option `-WhatIf`.

```output
Creating list of dependencies...
Uninstalling Az.Profile version 0.7.0
Uninstalling Az.Aks version 0.7.0
Uninstalling Az.AnalysisServices version 0.7.0
...
```

Führen Sie diesen Befehl für jede Azure PowerShell-Version aus, die Sie deinstallieren möchten. Der Einfachheit halber werden mit dem folgenden Skript alle Versionen von Az deinstalliert, __mit Ausnahme__ der aktuellen Version.

```powershell-interactive
$versions = (Get-InstalledModule Az -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule Az -Version ($_.Version) -Force }
```

## <a name="uninstall-the-azurerm-module"></a>Deinstallieren des AzureRM-Moduls

Falls Sie das Az-Modul auf Ihrem System installiert haben und AzureRM deinstallieren möchten, haben Sie zwei Möglichkeiten, bei denen das obige `Uninstall-AllModules`-Skript nicht ausgeführt werden muss. Die Wahl der Methode richtet sich danach, wie Sie AzureRM installiert haben.
Wenn Sie nicht sicher sind, sollten Sie zuerst die Schritte zum Deinstallieren einer MSI überprüfen.

### <a name="uninstall-msi"></a>Deinstallieren einer MSI

Falls Sie die AzureRM-Module von Azure PowerShell mit dem MSI-Paket installiert haben, müssen Sie die Deinstallation nicht über PowerShell, sondern über das Windows-System durchführen.

| Plattform | Anleitung |
|----------|--------------|
| Windows 10 | Start > Einstellungen > Apps |
| Windows 7 </br>Windows 8 | Start > Systemsteuerung > Programme > Programm deinstallieren |

Auf diesem Bildschirm sollte „Azure PowerShell“ in der Programmliste aufgeführt sein. Sie können die Anwendung dort deinstallieren.

### <a name="uninstall-from-powershell"></a>Deinstallieren über PowerShell

Falls Sie AzureRM über PowerShellGet installiert haben, können Sie die Module mit dem neuen Befehl `Uninstall-AzureRM` entfernen. Hiermit werden _alle_ AzureRM-Module von Ihrem Computer entfernt, aber für diesen Vorgang werden Administratorrechte benötigt.

```powershell-interactive
Uninstall-AzureRm
```

Wenn Sie den Befehl `Uninstall-AzureRM` nicht erfolgreich ausführen können, können Sie stattdessen das in diesem Artikel enthaltene `Uninstall-AllModules`-Skript verwenden.