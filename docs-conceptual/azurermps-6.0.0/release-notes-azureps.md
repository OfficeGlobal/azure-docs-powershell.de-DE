---
title: Azure PowerShell-Änderungsprotokoll | Microsoft-Dokumentation
description: Hierbei handelt es sich um einen Verlauf der Änderungen, die in der neuesten Version an Azure PowerShell vorgenommen wurden.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/08/2018
---
# <a name="release-notes"></a>Versionshinweise

Hierbei handelt es sich um eine Liste der Änderungen, die in dieser Version an Azure PowerShell vorgenommen wurden.

---

## <a name="600---may-2018"></a>6.0.0 – Mai 2018

### <a name="general"></a>Allgemein
* Festlegung der Mindestabhängigkeit von Modulen auf PowerShell 5.0

### <a name="azurestorage"></a>Azure.Storage
* Unterstützung als Storage-Blobcontainername
    - New-AzureStorageBlobContainer
    - Remove-AzureStorageBlobContainer
    - Set-AzureStorageBlobContent
    - Get-AzureStorageBlobContent
* Behebung des Problems, bei dem einige Fehlerausgaben von Storage-Cmdlets keine ausführlichen Informationen zum Fehler enthalten

### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermautomation"></a>AzureRM.Automation
* Entfernung des veralteten „Tags“-Alias aus Cmdlets
    - „Set-AzureRmAutomationRunbook“

### <a name="azurermbatch"></a>AzureRM.Batch
* Aktualisierung der Dokumentation zu „New-AzureBatchPool“ mit Entfernung des veralteten Beispiels

### <a name="azurermcdn"></a>AzureRM.Cdn
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermcompute"></a>AzureRM.Compute
* Unterstützung der ausführlichen Ausgabe von Parametern durch „New-AzureRmVm“ und „New-AzureRmVmss“
* Unterstützung der Zuweisung von benutzer- bzw. systemdefinierten Identitäten zu VMs durch „New-AzureRmVm“ und „New-AzureRmVmss“
* Erneute VMSS-Bereitstellung (Redeploy) und PerformMaintenance-Feature
    -  Hinzufügung der neuen Switchparameter „-Redeploy“ und „-PerformMaintenance“ zu „Set-AzureRmVmss“ und „Set-AzureRmVmssVM“
* Hinzufügung des Switchparameters „Add DisableVMAgent“ zum Set-AzureRmVMOperatingSystem-Cmdlet
* Unterstützung eines „Win10“-Images durch „New-AzureRmVm“ und „New-AzureRmVmss“ (einfacher Parametersatz)
* Hinzufügung des Repair-AzureRmVmssServiceFabricUpdateDomain-Cmdlets
* Einführung mehrerer grundlegender Änderungen
    - Ausführlichere Informationen im Migrationsleitfaden
* AAD-Parameter werden durch „Set-AzureRmVmDiskEncryptionExtension“ optional

### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Entfernung des veralteten „Tags“-Alias aus Cmdlets
    - New-AzureRmDataFactory

### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Aktualisierung des ADF-.Net SDK auf Vorschauversion 0.7.0 mit den folgenden Änderungen:
    - Hinzufügung von Ausführungsparametern und der Verbindungs-Manager-Eigenschaft zur ExecuteSSISPackage-Aktivität
    - Aktualisierung des verknüpften PostgreSql-/MySql-Diensts auf die Nutzung der vollständigen Verbindungszeichenfolge anstelle von Server, Datenbank, Schema, Benutzername und Kennwort
    - Entfernung des Schemas aus dem verknüpften DB2-Dienst
    - Entfernung der Schemaeigenschaft aus dem verknüpften Teradata-Dienst
    - Hinzufügung von LinkedService, Dataset und CopySource für Responsys

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Entfernung des veralteten „Tags“-Alias aus Cmdlets
    - „New-AzureRmDataLakeAnalyticsAccount“
    - „Set-AzureRmDataLakeAnalyticsAccount“

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Hinzufügung des neuen Features für die rekursive ACL-Änderung zu „Remove-AzureRmDataLakeStoreItemAclEntry“, „Set-AzureRmDataLakeStoreItemAclEntry“ und „Set-AzureRmDataLakeStoreItemAcl“
* Hinzufügung eines neuen Cmdlets zum Abrufen der Inhaltszusammenfassung unter einem Verzeichnis
* Hinzufügung eines neuen Cmdlets zu Abrufen der Datenträgerauslastung und eines ACL-Abbilds
* Korrektur des Rückgabetyps von „Set-AzureRmDataLakeStoreItemAcl“ von „Bool“ in „IEnumerable<DataLakeStoreItemAce>“
* Korrektur des Rückgabetyps von „Set-AzureRmDataLakeStoreItemAclEntry“ von „Bool“ in „IEnumerable<DataLakeStoreItemAce>“
* Grundlegende Änderungen in „Export-AzureRmDataLakeStoreItem“, „Import-AzureRmDataLakeStoreItem“ und „Remove-AzureRmDataLakeStoreItem“

### <a name="azurermdns"></a>AzureRM.Dns
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermeventhub"></a>AzureRM.EventHub
* Aktualisierung der Hilfe für Cmdlets mit fehlenden Beispielen

### <a name="azurerminsights"></a>AzureRM.Insights
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermiothub"></a>AzureRM.IotHub
* Aktivierung von Tags und Basic-SKU für IotHub

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Grundlegende Änderungen zur Unterstützung von Pipingszenarien
* Neu hinzugefügte Cmdlets: „Backup/Restore-AzureKeyVaultManagedStorageAccount“, „Backup/Restore-AzureKeyVaultCertificate“, „Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval“ und „Undo-AzureKeyVaultManagedStorageAccountRemoval“

### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* Entfernung des veralteten „Tags“-Alias aus Cmdlets
    - Update-AzureRmMlCommitmentPlan

### <a name="azurermmedia"></a>AzureRM.Media
* Entfernung des veralteten „Tags“-Alias aus Cmdlets
    - „Set-AzureRmMediaService“

### <a name="azurermnetwork"></a>AzureRM.Network
* Hinzufügung von Unterstützung für DDoS-Schutzplanressource
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermprofile"></a>AzureRM.Profile
* Standardmäßige Aktivierung der automatischen Kontextspeicherung
* Hinzufügung der Eigenschaften „USGovernmentOperationalInsightsEndpoint“ und „USGovernmentOperationalInsightsEndpointResourceId“ zur Azure-Umgebung für US Gov

### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Feste Authentifizierungsheader in SiteRecovery-Szenarien

### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermresources"></a>AzureRM.Resources
* Entfernung des veralteten Parameters „-AtScopeAndBelow“ aus dem Get-AzureRmRoledefinition-Aufruf
* Einbindung von Zuweisungen zu gelöschten Users/Groups/ServicePrincipals in das Get-AzureRmRoleAssignment-Ergebnis
* Hinzufügung von Registerkarten-Completern für Scope und ResourceType
* Hinzufügung des convenience-Cmdlets für die Erstellung von ServicePrincipals
* Zusammenführung der „Get-“- und „Find-“-Funktionalität in „Get-AzureRmResource“
* Hinzugefügte AD-Cmdlets:
  - Remove-AzureRmADGroupMember
  - Get-AzureRmADGroup
  - New-AzureRmADGroup
  - Remove-AzureRmADGroup
  - Remove-AzureRmADUser
  - Update-AzureRmADApplication
  - Update-AzureRmADServicePrincipal
  - Update-AzureRmADUser

### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Aktualisierung der Standard-SKU für die Linux-Imageversion
  - „NewAzureServiceFabricCluster.cs“ – UbuntuServer1604-SKU-Standardupdate

### <a name="azurermstorage"></a>AzureRM.Storage
* Einführung mehrerer grundlegender Änderungen
    - Weitere Informationen im Migrationsleitfaden

### <a name="azurermwebsites"></a>AzureRM.Websites
* Upgrade auf die aktuelle Version des Websites-SDK
* Hinzufügung der Eigenschaften „-AssignIdentity“ und „-Httpsonly“ für „Set-AzureRmWebApp“ und „Set-AzureRmWebAppSlot“
* Hinzufügung von zwei neuen Cmdlets: „Get-AzureRmWebAppSnapshots“ und „Restore-AzureRmWebAppSnapshot“
