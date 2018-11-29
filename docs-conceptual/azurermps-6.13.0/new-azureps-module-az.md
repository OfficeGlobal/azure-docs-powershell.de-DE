---
title: Einführung in das Az-Modul von Azure PowerShell
description: Hier finden Sie eine Einführung in das neue Az-Modul von Azure PowerShell, das das AzureRM-Modul ersetzt.
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "52587311"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>Einführung in das neue Azure PowerShell Az-Modul

Ab November 2018 ist das `Az`-Modul von Azure PowerShell als vollständige Public Preview verfügbar.
Az zeichnet sich durch kürzere Befehle und eine verbesserte Stabilität aus und unterstützt Windows, macOS und Linux. Darüber hinaus bietet Az die gleichen Features wie AzureRM sowie einen einfachen Migrationspfad.

Az verwendet die .NET Standard-Bibliothek und kann somit unter PowerShell 5.x und PowerShell 6.x ausgeführt werden.
Da PowerShell 6.x unter Linux, macOS und Windows ausgeführt werden kann, ist Az für alle Plattformen verfügbar.
Die Verwendung von .NET Standard ermöglicht die Vereinheitlichung der Codebasis von Azure PowerShell mit minimalen Auswirkungen für die Benutzer.

Da es sich bei Az um ein neues Modul handelt, wurde die Version zurückgesetzt. Die erste stabile Version hat die Nummer 1.0, das Modul bietet jedoch die gleichen Features wie AzureRM im November 2018.

## <a name="upgrade-to-az"></a>Upgraden auf Az

Benutzern wird empfohlen, ein Upgrade auf das neue `Az`-Modul durchzuführen. Gehen Sie dazu wie folgt vor:

* [Deinstallieren Sie das AzureRM-Modul von Azure PowerShell.](/powershell/azure/uninstall-azurerm-ps)
* [Installieren Sie das Az-Modul von Azure PowerShell.](/powershell/azure/install-az-ps)
* Aktivieren Sie den Kompatibilitätsmodus für AzureRM mit `Enable-AzureRMAlias`, während Sie sich mit den neuen Befehlen vertraut machen.

## <a name="migrate-existing-scripts-to-az"></a>Migrieren bereits vorhandener Skripts zu Az

Größere Updates können unangenehm sein. Das `Az`-Modul verfügt jedoch über einen Kompatibilitätsmodus, der Ihnen die Verwendung bereits vorhandener Skripts ermöglicht, während Sie sich um die Umstellung auf die neue Syntax kümmern. Verwenden Sie das Cmdlet `Enable-AzureRmAlias`, um den `AzureRM`-Kompatibilitätsmodus zu aktivieren. Dieses Cmdlet definiert Cmdlet-Namen von `AzureRM` als Aliase für die neuen Cmdlet-Namen von `Az`.

Die neuen Cmdlet-Namen sind ganz einfach zu lernen. Verwenden Sie in Cmdlet-Namen nicht mehr `AzureRm` oder `Azure`, sondern `Az`. Der alte Befehl `New-AzureRmVm` lautet nun also beispielsweise `New-AzVm`.

Eine umfassende Beschreibung des Migrationsprozesses finden Sie unter [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).

## <a name="the-future-of-support-for-azurerm"></a>Die Zukunft der AzureRM-Unterstützung

Nach Veröffentlichung der Version 1.0 von `Az` im Dezember 2018 werden für das vorhandene `AzureRM`-Modul keine neuen Cmdlets oder Features mehr bereitgestellt. `AzureRM` wird jedoch weiterhin offiziell gepflegt, und es werden weiterhin Fehlerbehebungen bereitgestellt. Es empfiehlt sich allerdings, auf das `Az`-Modul umzusteigen, um die neuesten Azure-Dienste und -Features nutzen zu können.