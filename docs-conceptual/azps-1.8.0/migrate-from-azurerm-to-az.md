---
title: Migrieren von Azure PowerShell-Skripts von AzureRM zu Az
description: Hier lernen Sie die Schritte und Tools kennen, mit denen Sie Skripts vom AzureRM-Modul zum neuen Az-Modul migrieren können.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: 43f4bdf2a59dd82fd881512aa9761bf72eb5703c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "63068862"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>Migrieren von AzureRM zum Az-Modul von Azure PowerShell

Das Az-Modul bietet die gleichen Features wie AzureRM, verwendet aber kürzere und konsistentere Cmdlet-Namen.
Für die AzureRM-Cmdlets geschriebene Skripts funktionieren nicht automatisch auch mit dem neuen Modul. Zur Vereinfachung des Übergangs bietet Az Tools, die es Ihnen ermöglichen, Ihre bereits vorhandenen Skripts mit AzureRM auszuführen. Eine Migration zu einem neuen Befehlssatz ist immer unangenehm. Dieser Artikel hilft Ihnen jedoch dabei, den Umstieg auf das neue Modul in die Wege zu leiten.

Die vollständige Liste mit grundlegenden Änderungen zwischen AzureRM und Az finden Sie im [Migrationsleitfaden für Az 1.0.0](migrate-az-1.0.0.md).

## <a name="check-for-installed-versions-of-azurerm"></a>Durchführen einer Überprüfung auf installierte Versionen von AzureRM

Das Az-Modul kann parallel zum AzureRM-Modul installiert werden, aber diese Vorgehensweise wird nicht empfohlen. Überprüfen Sie, welche Versionen von AzureRM auf Ihrem System installiert sind, bevor Sie Migrationsschritte ausführen. So können Sie sicherstellen, dass für Skripts bereits das aktuelle Release verwendet wird, und Sie können ermitteln, ob Sie Befehlsaliase ohne Deinstallation von AzureRM aktivieren können.

Führen Sie den folgenden Befehl aus, um zu überprüfen, welche Versionen von AzureRM bei Ihnen installiert sind:

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>Vergewissern, dass Ihre vorhandenen Skripts mit der neuesten AzureRM-Version funktionieren

Das ist der wichtigste Schritt überhaupt. Führen Sie Ihre vorhandenen Skripts aus, und vergewissern Sie sich, dass diese mit der _neuesten_ Version von AzureRM (__6.13.1__) funktionieren. Sollten Ihre Skripts nicht funktionieren, lesen Sie das [AzureRM-Migrationshandbuch](/powershell/azure/azurerm/migration-guide.6.0.0).

## <a name="install-the-azure-powershell-az-module"></a>Installieren des Az-Moduls von Azure PowerShell

Der erste Schritt besteht darin, das Az-Modul auf Ihrer Plattform zu installieren. Wenn Sie Az installieren, ist es ratsam, AzureRM zu deinstallieren. In den folgenden Schritten erfahren Sie, wie Sie Ihre bereits vorhandenen Skripts weiterhin ausführen und die Kompatibilität mit älteren Cmdlet-Namen sicherstellen können.

Gehen Sie zum Installieren des Az-Moduls von Azure PowerShell wie folgt vor:

* __EMPFOHLEN__: [Deinstallieren Sie das AzureRM-Modul.](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
  Achten Sie darauf, _alle_ installierten Versionen von AzureRM zu entfernen, nicht nur die neueste Version.
* [Installieren Sie das Az-Modul.](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><a name="aliases"/>Aktivieren von AzureRM-Kompatibilitätsaliasen 

> [!IMPORTANT]
>
> Aktivieren Sie den Kompatibilitätsmodus nur, wenn Sie _alle_ Versionen von AzureRM deinstalliert haben. Wenn Sie den Kompatibilitätsmodus bei noch vorhandenen AzureRM-Cmdlets aktivieren, kann dies zu unvorhersehbarem Verhalten führen. Überspringen Sie diesen Schritt, wenn Sie sich für die Beibehaltung der AzureRM-Installation entschieden haben. Sie müssen sich dann aber darüber im Klaren sein, dass für alle AzureRM-Cmdlets die älteren Module verwendet und keine Az-Cmdlets aufgerufen werden.

Wenn Sie AzureRM deinstalliert haben und Ihre Skripts mit der neuesten Version von AzureRM funktionieren, ist der nächste Schritt das Aktivieren des Kompatibilitätsmodus für das Az-Modul. Die Kompatibilität wird mithilfe des folgenden Befehls aktiviert:

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

Aliase ermöglichen die Verwendung alter Cmdlet-Namen bei installiertem Az-Modul. Diese Aliase werden in das Benutzerprofil für den ausgewählten Bereich geschrieben. Sollte kein Benutzerprofil vorhanden sein, wird eines erstellt.

> [!WARNING]
>
> Sie können für diesen Befehl zwar einen anderen Bereich (`-Scope`) verwenden, aber dies wird nicht empfohlen. Da Aliase in das Benutzerprofil für den ausgewählten Bereich geschrieben werden, empfiehlt es sich, sie auf einen möglichst kleinen Bereich zu beschränken. Eine systemweite Aktivierung von Aliasen kann auch zu Problemen für andere Benutzer führen, die AzureRM in ihrem lokalen Bereich installiert haben.

Führen Sie Ihre Skripts nach der Aktivierung des Aliasmodus erneut aus, um sich zu vergewissern, dass sie weiterhin wie erwartet funktionieren. 

## <a name="change-module-imports-and-cmdlet-names"></a>Ändern der Modulimporte und Cmdlet-Namen

Ganz allgemein haben sich die Modulnamen geändert, sodass `AzureRM` und `Azure` zu `Az` werden. Gleiches gilt für die Cmdlets.
So wurde beispielsweise das Modul `AzureRM.Compute` in `Az.Compute` umbenannt. `New-AzureRMVM` wurde zu `New-AzVM`, und `Get-AzureStorageBlob` ist jetzt `Get-AzStorageBlob`.

Es gibt allerdings Ausnahmen für diese Namensänderung, die Sie kennen sollten. Einige Module wurden umbenannt oder mit vorhandenen Modulen zusammengeführt, ohne dass sich dies auf das Suffix der zugehörigen Cmdlets ausgewirkt hat (bis auf die Änderung von `AzureRM` oder `Azure` in `Az`). Andernfalls wurde das vollständige Suffix des Cmdlets geändert, um den neuen Modulnamen widerzuspiegeln.

| AzureRM-Modul | Az-Modul | Cmdlet-Suffix geändert? |
|----------------|-----------|------------------------|
| AzureRM.Profile | Az.Accounts | Ja |
| AzureRM.Insights | Az.Monitor | Ja |
| AzureRM.DataFactories | Az.DataFactory | Ja |
| AzureRM.DataFactoryV2 | Az.DataFactory | Ja |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices | Nein  |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices | Nein  |
| AzureRM.Tags | Az.Resources | Nein  |
| AzureRM.MachineLearningCompute | Az.MachineLearning | Nein  |
| AzureRM.UsageAggregates | Az.Billing | Nein  |
| AzureRM.Consumption | Az.Billing | Nein  |

## <a name="summary"></a>Zusammenfassung

Mithilfe dieser Schritte können Sie alle Ihre bereits vorhandenen Skripts für die Verwendung des neuen Moduls aktualisieren. Falls Sie Fragen haben oder bei Ihrer Migration Probleme aufgetreten sind, kommentieren Sie diesen Artikel, damit wir die Anweisungen verbessern können.
