---
title: Migrieren von Azure PowerShell-Skripts von AzureRM zu Az
description: Hier lernen Sie die Schritte und Tools kennen, mit denen Sie Skripts vom AzureRM-Modul zum neuen Az-Modul migrieren können.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 720387ec1b23f10ddf2b153cf0705b2b6d1b7b82
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "52587702"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>Migrieren von AzureRM zum Az-Modul von Azure PowerShell

Das Az-Modul bietet die gleichen Features wie AzureRM, verwendet aber kürzere und konsistentere Cmdlet-Namen.
Für die AzureRM-Cmdlets geschriebene Skripts funktionieren nicht automatisch auch mit dem neuen Modul. Zur Vereinfachung des Übergangs bietet Az Tools, die es Ihnen ermöglichen, Ihre bereits vorhandenen Skripts mit AzureRM auszuführen. Eine Migration zu einem neuen Befehlssatz ist immer unangenehm. Dieser Artikel hilft Ihnen jedoch dabei, den Umstieg auf das neue Modul in die Wege zu leiten.

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>Vergewissern, dass Ihre vorhandenen Skripts mit der neuesten AzureRM-Version funktionieren

Das ist der wichtigste Schritt überhaupt. Führen Sie Ihre vorhandenen Skripts aus, und vergewissern Sie sich, dass sie mit der _neuesten_ Version von AzureRM (__6.13.0__) funktionieren. Sollten Ihre Skripts nicht funktionieren, lesen Sie das [AzureRM-Migrationshandbuch](migration-guide.6.0.0.md).

## <a name="install-the-azure-powershell-az-module"></a>Installieren des Az-Moduls von Azure PowerShell

Der erste Schritt besteht darin, das Az-Modul auf Ihrer Plattform zu installieren. Um Az installieren zu können, müssen Sie AzureRM deinstallieren.
In den folgenden Schritten erfahren Sie, wie Sie Ihre bereits vorhandenen Skripts weiterhin ausführen und die Kompatibilität mit älteren Cmdlet-Namen sicherstellen können.

Gehen Sie zum Installieren des Az-Moduls von Azure PowerShell wie folgt vor:

* [Deinstallieren Sie das AzureRM-Modul.](uninstall-azurerm-ps.md) Achten Sie darauf, _alle_ installierten Versionen von AzureRM zu entfernen, nicht nur die neueste Version.
* [Installieren Sie das Az-Modul.](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><a name="aliases"/>Aktivieren des AzureRM-Aliasmodus

Wenn Sie AzureRM deinstalliert haben und Ihre Skripts mit der neuesten Version von AzureRM funktionieren, können Sie den Kompatibilitätsmodus für das Az-Modul aktivieren. Die Kompatibilität wird mithilfe des folgenden Befehls aktiviert:

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

Aliase ermöglichen die Verwendung alter Cmdlet-Namen bei installiertem `Az`-Modul. Diese Aliase werden in das Benutzerprofil für den ausgewählten Bereich geschrieben. Sollte kein Benutzerprofil vorhanden sein, wird eines erstellt.

> [!WARNING]
>
> Sie können für diesen Befehl zwar einen anderen Bereich (`-Scope`) verwenden, dies wird jedoch nicht empfohlen. Da Aliase in das Benutzerprofil für den ausgewählten Bereich geschrieben werden, empfiehlt es sich, sie auf einen möglichst kleinen Bereich zu beschränken. Eine systemweite Aktivierung von Aliasen kann auch zu Problemen für andere Benutzer führen, die `AzureRM` in ihrem lokalen Bereich installiert haben.

Führen Sie Ihre Skripts nach der Aktivierung des Aliasmodus erneut aus, um sich zu vergewissern, dass sie weiterhin wie erwartet funktionieren. 

## <a name="change-module-imports-and-cmdlet-names"></a>Ändern der Modulimporte und Cmdlet-Namen

Ganz allgemein haben sich die Modulnamen geändert, sodass `AzureRM` und `Azure` zu `Az` werden. Gleiches gilt für die Cmdlets.
So wurde beispielsweise das Modul `AzureRM.Compute` in `Az.Compute` umbenannt. `New-AzureRmVM` wurde zu `New-AzVM`, und `Get-AzureStorageBlob` ist jetzt `Get-AzStorageBlob`.

Es gibt allerdings Ausnahmen für diese Namensänderung, die Sie kennen sollten, bevor Sie etwas umbenennen:

| AzureRM-Modul | Az-Modul |
|----------------|-----------|
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |

## <a name="summary"></a>Zusammenfassung

Mithilfe dieser Schritte können Sie alle Ihre bereits vorhandenen Skripts für die Verwendung des neuen Moduls aktualisieren. Falls Sie Fragen haben oder bei Ihrer Migration Probleme aufgetreten sind, kommentieren Sie diesen Artikel, damit wir die Anweisungen verbessern können.
