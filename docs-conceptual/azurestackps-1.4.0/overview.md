---
title: Übersicht über Azure Stack PowerShell mit Administratorrechten | Microsoft-Dokumentation
description: Enthält eine Übersicht über Azure Stack PowerShell mit Administratorrechten und eine Anleitung zur Installation und Konfiguration.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: 72d147f5bc9c882083dda6b33b1c89663fd2eb34
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001676"
---
# <a name="azure-stack-module-140"></a>Azure Stack-Modul 1.4.0

## <a name="requirements"></a>Anforderungen:
Die niedrigste unterstützte Azure Stack-Version ist 1804.

Hinweis: Falls Sie eine niedrigere Version verwenden, installieren Sie die Version 1.2.11.

## <a name="known-issues"></a>Bekannte Probleme:

- Zum Schließen einer Warnung wird die Azure Stack-Version 1803 benötigt.
- Mit „New-AzsOffer“ können keine öffentlichen Angebote erstellt werden. Das Cmdlet „Set-AzsOffer“ muss hinterher aufgerufen werden, um den Zustand zu ändern.
- Ein IP-Pool kann nicht ohne erneute Bereitstellung entfernt werden.

## <a name="breaking-changes"></a>Wichtige Änderungen
Für die Folgeversion von Version 1.3.0 wurden keine Breaking Changes vorgenommen. Alle Breaking Changes, die aus der Version 1.2.11 migriert werden, sind hier dokumentiert: https://aka.ms/azspowershellmigration

## <a name="install"></a>Installieren
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a>Versionsinformationen
    * Zwischen der Vorgängerversion 1.3.0 und der Azure Stack-Version 1.4.0 wurden keine Breaking Changes eingeführt.
    * Azs.AzureBridge.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Backup.Admin
        - Die neuen Parameter „BackupFrequencyInHours“, „IsBackupSchedulerEnabled“ und „BackupRetentionPeriodInDays“ wurden im Cmdlet „Set-AzsBackupShare“ hinzugefügt.
        - Cmdlet „New-EncyptionKeyBase64“ hinzugefügt, um die Erstellung eines Verschlüsselungsschlüssels zu erleichtern
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Commerce.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Fabric.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
        - Cmdlet „Add-AzsScaleUnitNode“ hinzugefügt, um dem Administrator das Hinzufügen neuer Skalierungseinheitknoten azurestack-Stempel zu ermöglichen
        - Cmdlet „New-AzsScaleUnitNodeObject“ hinzugefügt, um die Erstellung von Skalierungseinheit-Parameterobjekten zu erleichtern
    * Azs.Gallery.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.InfrastructureInsights.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Network.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Update.Admin
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Subscriptions
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde
    * Azs.Subscriptions.Admin
        - Cmdlet „Move-AzsSubscription“ hinzugefügt, um Abonnements zwischen Angeboten delegierter Anbieter zu verschieben
        - Cmdlet „Test-AzsMoveSubscription“ hinzugefügt, um zu überprüfen, ob Benutzerabonnements zwischen Angeboten delegierter Anbieter verschoben werden können
        - Korrektur des Fehlers, aufgrund dessen nur eine einzelne Seite in paginierten Ergebnissen zurückgegeben wurde

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
Vorschauversion des Compute-Administratormoduls von Azure Stack mit Funktionen zur Verwaltung von Computekontingenten, Plattformimages und VM-Erweiterungen.

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
