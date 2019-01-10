---
title: Übersicht über Azure PowerShell
description: Enthält eine Übersicht über das Azure PowerShell Az-Modul und Informationen zur Installation und zum Einstieg.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736459"
---
# <a name="overview-of-azure-powershell"></a>Übersicht über Azure PowerShell

Azure PowerShell bietet eine Reihe von Cmdlets, die das [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview)-Modell für die Verwaltung von Azure-Ressourcen verwenden. Für Azure PowerShell wird .NET Standard verwendet, damit die Umgebung für Windows, macOS und Linux verfügbar ist.
Azure PowerShell steht auch über Azure Cloud Shell zur Verfügung.

Verwenden Sie [Azure Cloud Shell](/azure/cloud-shell/overview), um Azure PowerShell in Ihrem Browser auszuführen, oder führen Sie die [lokale Installation](install-az-ps.md) durch. Lesen Sie den Artikel zu den [ersten Schritten](get-started-azureps.md), um sich über die Grundlagen von Azure PowerShell zu informieren und in die Nutzung von Azure einzusteigen.

Informationen zur neuesten Azure PowerShell-Version finden Sie in den [Versionshinweisen](release-notes-azureps.md).

## <a name="about-the-new-az-module"></a>Informationen zum neuen Az-Modul

In dieser Dokumentation wird das neue Az-Modul für Azure PowerShell beschrieben. Dieses neue Modul wurde von Grund auf in .NET Standard geschrieben. Bei Verwendung von .NET Standard kann Azure PowerShell unter PowerShell 5.x auf Windows oder PowerShell 6 auf einer beliebigen Plattform ausgeführt werden. Das Az-Modul ist jetzt die bevorzugte Vorgehensweise für die Interaktion mit Azure über PowerShell.
Für AzureRM werden weiterhin Fehlerbehebungen bereitgestellt, aber keine neuen Features mehr.

Alle Details zum neuen Modul, z.B. die Umbenennung der Befehle und die Wartungspläne für AzureRM, finden Sie unter [Einführung in das Az-Modul von Azure PowerShell](new-azureps-module-az.md). Wenn Sie gleich in die Nutzung des neuen Moduls einsteigen möchten, können Sie den Artikel [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md) lesen.

Darüber hinaus ist die [AzureRM-Dokumentation](/powershell/azure/azurerm) verfügbar.

> [!IMPORTANT]
>
> Während die Azure-Dokumentation aktualisiert wird, damit die neuen Cmdlet-Namen des Moduls darin widergespiegelt werden, werden in den Artikeln unter Umständen vorerst noch die AzureRM-Befehle verwendet. Nach der Installation des Az-Moduls ist es ratsam, die Cmdlet-Aliase von AzureRM mit `Enable-AzureRmAlias` zu aktivieren. Ausführlichere Informationen finden Sie im Artikel [Migrieren von AzureRM zum Az-Modul von Azure PowerShell](migrate-from-azurerm-to-az.md).

## <a name="common-scenarios"></a>Häufige Szenarios

In den folgenden Beispielen werden gängige Szenarien mit Azure PowerShell veranschaulicht:

* [Virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [Virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [Web-Apps](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [SQL-Datenbanken](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a>PowerShell-Grundlagen erlernen

Falls Sie mit PowerShell noch nicht vertraut sind, kann es hilfreich sein, eine Einführung zu lesen.

* [Installieren von PowerShell](/powershell/scripting/setup/installing-windows-powershell)
* [Skripterstellung mit PowerShell](/powershell/scripting/powershell-scripting)

Empfehlenswert ist auch folgendes Video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1) (PowerShell-Grundlagen – Teil 1: Erste Schritte mit PowerShell)

Oder Sie sehen sich in der Microsoft Virtual Academy die Einführung [Getting Started with PowerShell](https://mva.microsoft.com/liveevents/powershell-jumpstart) (Erste Schritte mit PowerShell) an.

## <a name="build-your-skills-with-microsoft-learn"></a>Erweitern Ihrer Fähigkeiten mit Microsoft Learn

- [Automatisieren von Azure-Aufgaben mithilfe von Skripts über PowerShell](/learn/modules/automate-azure-tasks-with-powershell/)
- [Mehr interaktives Lernen...](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a>Andere Azure PowerShell-Module

* [Azure Active Directory](/powershell/azure/active-directory/)
* [Azure Information Protection](/powershell/azure/aip/)
* [Azure Service Fabric](/powershell/azure/service-fabric/)
* [Azure ElasticDB](/powershell/azure/elasticdbjobs/)
