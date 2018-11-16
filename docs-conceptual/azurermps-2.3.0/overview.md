---
title: Übersicht über Azure Stack PowerShell | Microsoft-Dokumentation
description: Enthält eine Übersicht über Azure Stack PowerShell und eine Anleitung zur Installation und Konfiguration.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: cd415e862bfaa2b767cce108689ebaf34ef74305
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/15/2018
ms.locfileid: "51575415"
---
# <a name="azurerm-module-230"></a>AzureRM-Modul 2.3.0

## <a name="requirements"></a>Anforderungen:
Die niedrigste unterstützte Azure Stack-Version ist 1808.

Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.


## <a name="install"></a>Installieren
```powershell-interactive
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

## <a name="release-notes"></a>Versionsinformationen
* Das Release 2.3.0 verfügt über eine Liste mit Breaking Changes. Für das Upgrade von Version 1.2.11 haben wir unter https://aka.ms/azspowershellmigration einen Migrationsleitfaden erstellt.
* Dieses Release entspricht dem Azure Stack-spezifischen API-Profil 2018-03-01-hybrid
* Alle Module sind mindestens vom AzureRm.Profile-Modul abhängig.
* Die von den einzelnen Modulen unterstützten API-Versionen werden aktualisiert. 
    * Compute – 2017-03-30
    * Netzwerk – 2017-10-01
    * Storage – 2016-01-01
    * Ressourcen – 2018-02-01
    * Key Vault – 2016-10-01
    * DNS – 2016-04-01
* Die vollständige Zuordnung aller API-Versionen für die einzelnen Ressourcentypen finden Sie unter https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json.

## <a name="content"></a>Inhalt:
### <a name="azure-bridge"></a>Azure-Bridge
Vorschauversion des AzureBridge-Administratormoduls von Azure Stack, mit dem Sie Images aus Azure syndizieren können.

### <a name="backup"></a>Backup
Vorschauversion des Backup-Administratormoduls, das Administratoren Folgendes ermöglicht:
- Konfigurieren des Speicherorts von Sicherungen
- Durchführen von Sicherungen
- Auflisten und Wiederherstellen abgeschlossener Sicherungen

### <a name="commerce"></a>Commerce
Vorschauversion des Commerce-Administratormoduls von Azure Stack, mit dem die aggregierte Datennutzung für das gesamte Azure Stack-System angezeigt werden kann.

### <a name="compute"></a>Compute
Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages, verwalteten Datenträgern und VM-Erweiterungen.

### <a name="fabric"></a>Fabric
Vorschauversion des Fabric-Administratormoduls von Azure Stack, mit dem Administratoren Infrastrukturkomponenten anzeigen und verwalten können:
- Beenden, Starten und Herunterfahren von Skalierungseinheitknoten
- Entladen und Fortsetzen von Skalierungseinheitknoten für FRU-bezogene Aktivitäten
- Reparieren von Skalierungseinheitknoten
- Neustarten der Infrastrukturrolle
- Beenden, Starten und Herunterfahren von Instanzen der Infrastrukturrolle
- Erstellen neuer IP-Pools


### <a name="gallery"></a>Gallery
Vorschauversion des Gallery-Administratormoduls von Azure Stack mit Funktionen zum Verwalten von Katalogelementen im Azure Stack-Marketplace.

### <a name="infrastructure-insights"></a>Infrastructure Insights
Vorschauversion des Infrastructure Insights-Administratormoduls, das Administratoren Folgendes ermöglicht:
- Anzeigen der Integrität ihrer Azure Stack-Stempelressourcen
- Anzeigen und Verwalten von Warnungen

### <a name="keyvault"></a>KeyVault
Vorschauversion des KeyVault-Administratormoduls von Azure Stack, mit dem Administratoren KeyVault-Kontingente anzeigen können.

### <a name="network"></a>Netzwerk
Vorschauversion des Network-Administratormoduls, das Folgendes ermöglicht:
- Verwalten von Netzwerkkontingenten
- Anzeigen zugeordneter Netzwerkressourcen (beispielsweise öffentliche IP-Adressen, virtuelle Netzwerke oder Lastenausgleichsmodule)
- Stellt ein Cmdlet zum Anzeigen einer Administratorübersicht bereit.

### <a name="storage"></a>Speicher
Vorschauversion des Storage-Administratormoduls von Azure Stack.  Dieses Release bietet Funktionen für Folgendes:
- Verwalten von Speicherkontingenten
- Durchführen der Garbage Collection für gelöschte Speicherressourcen
- Wiederherstellen gelöschter Speicherkonten
- Migrieren von Containern zwischen Freigaben
- Anzeigen von Informationen zu den einzelnen Speicherkomponenten
- Anzeigen von Nutzungs- und Leistungsinformationen

### <a name="subscription-admin"></a>Abonnementadministrator
Vorschauversion des Subscription-Administratormoduls von Azure Stack.  Dieses Modul bietet Administratorfunktionen für Folgendes:
- Verwalten von Plänen und Angeboten
- Anzeigen von Nutzungs- und Leistungsinformationen
- Verwalten der RBAC

### <a name="subscription"></a>Abonnement
Vorschauversion des Subscription-Moduls von Azure Stack.  Dieses Modul bietet Benutzerfunktionen für Folgendes:
- Erstellen, Löschen und Aktualisieren von Abonnements

### <a name="update"></a>Aktualisieren
Vorschauversion des Update-Administratormoduls von Azure Stack.  Dieses Modul ermöglicht Administratoren Folgendes:
- Auflisten und Installieren verfügbarer Updates
- Fortsetzen unterbrochener Updates
- Anzeigen installierter Updates
