---
title: Einführung in das Az-Modul von Azure PowerShell
description: Hier finden Sie eine Einführung in das neue Az-Modul von Azure PowerShell, das das AzureRM-Modul ersetzt.
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: d08bca962b6ff65d25135150824b7c24fbd20103
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56144822"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>Einführung in das neue Azure PowerShell Az-Modul

Ab Dezember 2018 ist das Az-Modul von Azure PowerShell allgemein verfügbar und jetzt das beabsichtigte PowerShell-Modul für die Interaktion mit Azure. Az verfügt über kürzere Befehle, verbesserte Stabilität und plattformübergreifende Unterstützung. Darüber hinaus bietet Az die gleichen Features wie AzureRM sowie einen einfachen Migrationspfad.

Az verwendet die .NET Standard-Bibliothek und kann somit unter PowerShell 5.x und PowerShell 6.x ausgeführt werden.
Da PowerShell 6.x unter Linux, macOS und Windows ausgeführt werden kann, ist Azure PowerShell jetzt für alle Plattformen verfügbar.
Die Verwendung von .NET Standard ermöglicht die Vereinheitlichung der Codebasis von Azure PowerShell mit minimalen Auswirkungen für die Benutzer.

Da es sich bei Az um ein neues Modul handelt, wurde die Version auf 1.0.0 zurückgesetzt.

## <a name="upgrade-to-az"></a>Upgraden auf Az

Allen Benutzern wird empfohlen, ein Upgrade auf das neue Az-Modul durchzuführen. Gehen Sie dazu wie folgt vor:

* __EMPFOHLEN__: [Deinstallieren Sie das AzureRM-Modul von Azure PowerShell.](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
* [Installieren Sie das Az-Modul von Azure PowerShell.](/powershell/azure/install-az-ps)
* Aktivieren Sie den Kompatibilitätsmodus, um Aliase für AzureRM-Cmdlets mit `Enable-AzureRMAlias` hinzuzufügen, während Sie sich mit den neuen Befehlen vertraut machen. Aktivieren Sie die Aliase __nur__, wenn Sie AzureRM nicht installiert haben.

## <a name="migrate-existing-scripts-to-az"></a>Migrieren bereits vorhandener Skripts zu Az

Größere Updates können unangenehm sein. Das Az-Modul verfügt aber über einen Kompatibilitätsmodus, der Ihnen die Verwendung bereits vorhandener Skripts ermöglicht, während Sie sich um die Umstellung auf die neue Syntax kümmern. Verwenden Sie das Cmdlet `Enable-AzureRmAlias`, um den AzureRM-Kompatibilitätsmodus zu aktivieren. Dieses Cmdlet definiert Namen von AzureRM-Cmdlets als Aliase für die neuen Namen von Az-Cmdlets.

Die neuen Cmdlet-Namen sind ganz einfach zu lernen. Verwenden Sie in Cmdlet-Namen nicht mehr `AzureRm` oder `Azure`, sondern `Az`. Der alte Befehl `New-AzureRMVm` lautet nun also beispielsweise `New-AzVm`.

Eine umfassende Beschreibung des Migrationsprozesses finden Sie unter [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).

## <a name="the-future-of-support-for-azurerm"></a>Die Zukunft der AzureRM-Unterstützung

Für das vorhandene AzureRM-Modul werden keine neuen Cmdlets oder Features mehr bereitgestellt. AzureRM wird bis Dezember 2020 aber weiterhin offiziell gepflegt und mit Fehlerbehebungen versehen. Es ist ratsam, auf das Az-Modul umzusteigen, damit Sie die neuesten Azure-Dienste und -Features nutzen können.
