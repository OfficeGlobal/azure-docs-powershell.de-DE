---
title: Deinstallieren von Azure PowerShell
description: Anleitung zum vollständigen Deinstallieren von Azure PowerShell
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 385dd0281185cfb9e7bdd2c98e4c557659fff384
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179223"
---
# <a name="uninstall-the-azure-powershell-module"></a>Deinstallieren des Azure PowerShell-Moduls

In diesem Artikel erfahren Sie, wie Sie eine ältere Version von Azure PowerShell deinstallieren bzw. vollständig vom System entfernen. Verwenden Sie das [Send-Feedback](/powershell/module/azurerm.profile/send-feedback)-Cmdlet, um uns Feedback zu senden, falls Sie Azure PowerShell vollständig deinstallieren möchten.
Falls ein Fehler aufgetreten ist, wären wir Ihnen dankbar, wenn Sie ein [GitHub-Problem melden](https://github.com/azure/azure-powershell/issues).

## <a name="uninstall-msi"></a>Deinstallieren einer MSI

Falls Sie Azure PowerShell mithilfe des MSI-Pakets installiert haben, müssen Sie die Deinstallation nicht über PowerShell, sondern über das Windows-System ausführen.

| Plattform | Anleitung |
|----------|--------------|
| Windows 10 | Start > Einstellungen > Apps |
| Windows 7 </br>Windows 8 | Start > Systemsteuerung > Programme > Programm deinstallieren |

Auf diesem Bildschirm sollte „Azure PowerShell“ in der Programmliste aufgeführt sein. Sie können die Anwendung dort deinstallieren.

## <a name="uninstall-from-powershell"></a>Deinstallieren über PowerShell

Falls Sie Azure PowerShell mithilfe von PowerShellGet installiert haben, können Sie das Cmdlet [Uninstall-Module](/powershell/module/powershellget/uninstall-module) verwenden. Mit `Uninstall-Module` wird jedoch nur ein Modul deinstalliert. Wenn Sie Azure PowerShell vollständig entfernen möchten, müssen Sie die Module einzeln deinstallieren. Die Deinstallation kann kompliziert sein, wenn Sie mehrere Versionen von Azure PowerShell installiert haben.

Das folgende Skript fragt den PowerShell-Katalog ab, um eine Liste mit den abhängigen Submodulen abzurufen. Anschließend wird mit dem Skript die richtige Version der einzelnen Submodule deinstalliert.

```powershell
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredversion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

Kopieren Sie zum Verwenden dieser Funktion den Code, und fügen Sie ihn in Ihre PowerShell-Sitzung ein. Das folgende Beispiel zeigt, wie Sie die Funktion ausführen, um eine ältere Version von Azure PowerShell zu entfernen.

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

Bei der Ausführung des Skripts werden jeweils der Name und die Version des Submoduls angezeigt, das gerade deinstalliert wird.

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

Führen Sie diesen Befehl für jede Azure PowerShell-Version aus, die Sie deinstallieren möchten.
